---
author: pkrebs
ms.author: pkrebs
title: Configuration de composant WebPart autonome
ms.date: 02/10/2019
description: Formation personnalisée pour la configuration du composant WebPart manuel Office 365
ms.openlocfilehash: 650e6c12ebe8ca7fedc6edc107b5822c48ead99a
ms.sourcegitcommit: b6617bbbaee0784d6216e96052c2469f97cf51e9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2019
ms.locfileid: "30411874"
---
# <a name="stand-alone-web-part-setup"></a>Configuration de composant WebPart autonome

La formation personnalisée offre une configuration de composant WebPart autonome manuelle pour les organisations qui disposent déjà d'un site de communication moderne SharePoint Online dédié à la formation, ou qui souhaitent simplement configurer le composant WebPart d'apprentissage personnalisé en leur propre temps site de communication. Notez que le programme d'installation manuel nécessite l'utilisation de Windows PowerShell et de SharePoint Online Management Shell. Les étapes d'une configuration manuelle du composant WebPart d'apprentissage personnalisé comme suit:

- Vérifiez que vous remplissez toutes les conditions préalables.
- Installez le fichier customlearning. sppkg dans votre catalogue d'applications client 365 Office.
- Approvisionner/identifier un site de communication moderne qui sert de formation personnalisée pour votre site d'accueil Office 365.
- Exécutez un script PowerShell qui configurera votre client avec les artefacts appropriés dont dépend l'apprentissage personnalisé.
- Accédez à la page de site CustomLearningAdmin. aspx pour charger le composant WebPart d'administration afin d'initialiser la configuration de contenu personnalisé.

> [!NOTE]
> Si vous recherchez un moyen rapide et facile de configurer l'apprentissage personnalisé, consultez la rubrique [provision Custom Learning](installsitepackage.md).

## <a name="prerequisites"></a>Conditions préalables
Pour garantir la réussite de la configuration manuelle du composant WebPart d'apprentissage personnalisé, les conditions préalables requises doivent être satisfaites. 

- Vous devez avoir configuré et configuré le catalogue d'applications à l'échelle du client. Consultez la rubrique [configurer votre client Office 365](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) et suivez la section créer un site de catalogue d'applications. 
- Si votre catalogue d'applications à l'échelle du client a déjà été mis en service, vous aurez besoin d'accéder à un compte disposant de droits de chargement d'un package vers celui-ci pour terminer le processus d'installation. Il s'agit généralement d'un compte doté du rôle d'administrateur SharePoint. 
- Si un compte associé à ce rôle ne fonctionne pas, accédez au centre d'administration SharePoint et recherchez les administrateurs de collections de sites pour la collection de sites de catalogue d'applications, puis connectez-vous en tant qu'administrateur de collection de sites ou ajoutez le compte d'administrateur SharePoint. les administrateurs de collections de sites ont échoué. 
- Vous aurez également besoin d'un accès à un compte qui est un administrateur de client SharePoint.

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>Étape 1: obtenir le package de composants WebPart et le script de configuration à partir de GitHub
Dans le cadre du processus de configuration, vous avez besoin du package de composants WebPart de formation personnalisé et du script de configuration PowerShell.

- Accédez au [référentiel GitHub de formation personnalisée](https://github.com/pnp/custom-learning-office-365).
- Cliquez sur **Télécharger** pour enregistrer le package de composants WebPart et le script sur un lecteur local. Vous utiliserez le script et le package de composants WebPart dans les étapes ultérieures de ce processus.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Étape 2: Télécharger le composant WebPart dans le catalogue d'applications client
Pour configurer la formation personnalisée pour Office 365, téléchargez le fichier customlearning. sppkg dans le catalogue d'applications à l'échelle du client et déployez-le. Pour obtenir des instructions détaillées sur l'ajout d'une application au catalogue d'applications, voir [utiliser le catalogue d'applications pour mettre à disposition des applications d'entreprise personnalisées pour votre environnement SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) .

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>Étape 3: configurer/identifier un site de communication moderne
Identifiez un site de communication SharePoint existant ou approvisionnez-en un nouveau dans votre client SharePoint Online. Pour plus d'informations sur la mise en service d'un site de communication, voir [créer un site de communication dans SharePoint Online](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) et suivre les étapes de création d'un site de communication.

## <a name="step-4---set-permissions-for-the-site"></a>Étape 4: définir des autorisations pour le site
Assurez-vous que les autorisations suivantes sont définies pour le site:
- **Administrateur de la collection de sites ou partie du groupe propriétaires** : autorisations requises pour initialiser l'élément de liste CustomConfig qui configure la formation personnalisée pour sa première utilisation. 
- **Groupe membres** -permissons requis pour administrer l'apprentissage personnalisé, y compris le masquage et l'affichage de contenu et l'administration des sélections personnalisées
- **Groupe visiteurs** -autorisations requises pour afficher le contenu du site. 

## <a name="step-5--execute-powershell-configuration-script"></a>Étape 5-exécuter le script de configuration PowerShell
Un script `CustomLearningConfiguration.ps1` PowerShell est inclus que vous devrez exécuter pour créer trois propriétés de [client](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) utilisées par la solution. De plus, le script crée deux [pages d'application à composant unique](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) dans la bibliothèque pages de site pour héberger les composants WebPart administrateur et utilisateur à un emplacement connu.

### <a name="disabling-telemetry-collection"></a>DésActivation de la collection de télémétrie
Une partie de cette solution inclut le suivi des télémétries anonyme, qui est défini par défaut sur activé. Si vous effectuez une installation manuelle et que vous souhaitez désactiver le suivi de la télémétrie, modifiez le `CustomlearningConfiguration.ps1` script de manière à définir la variable $optInTelemetry sur $false.

Si vous n'effectuez pas une installation manuelle et souhaitez désactiver le suivi de la télémétrie, un script `TelemetryOptOut.ps1` distinct a été inclus, lorsque l'exécution désactivera le suivi de télémétrie.

## <a name="step-6---initialize-web-part-custom-configuration"></a>Étape 6: initialiser la configuration personnalisée du composant WebPart
Une fois le script PowerShell exécuté, accédez à `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. Cela initialise l'élément de liste **CustomConfig** qui configure la formation personnalisée pour sa première utilisation.

La configuration est maintenant terminée. Pour en savoir plus sur la personnalisation du site de formation personnalisé et du composant WebPart pour votre environnement, voir [personnaliser l'expérience de formation](custom_overview.md).

### <a name="next-steps"></a>Étapes suivantes
- [Personnaliser](custom_overview.md) l'expérience de formation pour votre organisation.

