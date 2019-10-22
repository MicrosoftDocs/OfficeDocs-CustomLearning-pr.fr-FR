---
author: pkrebs
ms.author: pkrebs
title: Configuration de composant WebPart autonome
ms.date: 02/10/2019
description: Installation manuelle du composant WebPart chemin d’apprentissage Microsoft 365
ms.openlocfilehash: f3271dbd75ee18db7f89fdd15ebb35c1b2bf7d97
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/21/2019
ms.locfileid: "34247869"
---
# <a name="stand-alone-web-part-setup"></a>Configuration de composant WebPart autonome

Les chemins d’apprentissage Microsoft 365 offrent une configuration de composant WebPart autonome et manuelle pour les organisations qui ont déjà un site de communication moderne SharePoint Online dédié à la formation, ou qui souhaitent simplement configurer le composant WebPart voies d’apprentissage dans son propre site de communication. Notez que le programme d’installation manuel nécessite l’utilisation de Windows PowerShell et de SharePoint Online Management Shell. Les étapes d’une configuration manuelle du composant WebPart voies d’apprentissage comme suit :

- Vérifiez que vous remplissez toutes les conditions préalables.
- Installez le fichier customlearning. sppkg dans votre catalogue d’applications client SharePoint.
- Approvisionner/identifier un site de communication moderne qui se comporte comme votre site d’accueil des chemins d’apprentissage Microsoft 365.
- Exécutez un script PowerShell qui configurera votre client avec les artefacts appropriés dont dépend le chemin d’apprentissage.
- Accédez à la page de site CustomLearningAdmin. aspx pour charger le composant WebPart d’administration afin d’initialiser la configuration de contenu personnalisé.

> [!NOTE]
> Si vous recherchez un moyen rapide et facile de configurer les voies de formation, voir [approvisionner les chemins d’apprentissage Microsoft 365](custom_provision.md).

## <a name="prerequisites"></a>Conditions préalables
Pour garantir la réussite de la configuration manuelle du composant WebPart voies d’apprentissage, les conditions préalables suivantes doivent être remplies. 

- Vous devez avoir configuré et configuré le catalogue d’applications à l’échelle du client. Consultez la rubrique [configurer votre client Office 365](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) et suivez la section créer un site de catalogue d’applications. 
- Si votre catalogue d’applications à l’échelle du client a déjà été mis en service, vous aurez besoin d’accéder à un compte disposant de droits de chargement d’un package vers celui-ci pour terminer le processus d’installation. Il s’agit généralement d’un compte doté du rôle d’administrateur SharePoint. 
- Si un compte associé à ce rôle ne fonctionne pas, accédez au centre d’administration SharePoint et recherchez les administrateurs de collections de sites pour la collection de sites de catalogue d’applications, puis connectez-vous en tant qu’administrateur de collection de sites ou ajoutez le compte d’administrateur SharePoint. les administrateurs de collections de sites ont échoué. 
- Vous aurez également besoin d’un accès à un compte qui est un administrateur de client SharePoint.

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>Étape 1 : obtenir le package de composants WebPart et le script de configuration à partir de GitHub
Dans le cadre du processus de configuration, vous avez besoin du package de composants WebPart des chemins d’apprentissage Microsoft 365 et du script de configuration de PowerShell.

- Accédez au [référentiel GitHub des voies d’apprentissage](https://github.com/pnp/custom-learning-office-365).
- Cliquez sur **Télécharger** pour enregistrer le package de composants WebPart et le script sur un lecteur local. Vous utiliserez le script et le package de composants WebPart dans les étapes ultérieures de ce processus.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Étape 2 : Télécharger le composant WebPart dans le catalogue d’applications client
Pour configurer les voies d’apprentissage de Microsoft 365, téléchargez le fichier customlearning. sppkg dans le catalogue d’applications à l’échelle du client et déployez-le. Pour obtenir des instructions détaillées sur l’ajout d’une application au catalogue d’applications, voir [utiliser le catalogue d’applications pour mettre à disposition des applications d’entreprise personnalisées pour votre environnement SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) .

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>Étape 3 : configurer/identifier un site de communication moderne
Identifiez un site de communication SharePoint existant ou approvisionnez-en un nouveau dans votre client SharePoint Online. Pour plus d’informations sur la mise en service d’un site de communication, voir [créer un site de communication dans SharePoint Online](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) et suivre les étapes de création d’un site de communication.

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>Étape 4 : ajouter l’application des chemins d’apprentissage Microsoft 365 au site

1. À partir du site SharePoint, cliquez sur le menu système, puis cliquez sur **Ajouter une application**. 
2. Sous **vos applications**, cliquez sur **à partir de votre organisation**, puis cliquez sur **parcours de formation pour Office 365**. 

## <a name="step-5---set-permissions-for-the-site"></a>Étape 5 : définir des autorisations pour le site
Assurez-vous que les autorisations suivantes sont définies pour le site :
- **Administrateur de la collection de sites ou partie du groupe propriétaires** : autorisations requises pour initialiser l’élément de liste CustomConfig qui configure les voies de formation pour sa première utilisation. 
- **Membres Group** -permissons requis pour administrer les voies de formation, y compris le masquage et l’affichage du contenu et l’administration des playlists personnalisées
- **Groupe visiteurs** -autorisations requises pour afficher le contenu du site. 

## <a name="step-6--execute-powershell-configuration-script"></a>Étape 6-exécuter le script de configuration PowerShell
Un script `CustomLearningConfiguration.ps1` PowerShell est inclus que vous devrez exécuter pour créer trois propriétés de [client](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) utilisées par la solution. De plus, le script crée deux [pages d’application à composant unique](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) dans la bibliothèque pages de site pour héberger les composants WebPart administrateur et utilisateur à un emplacement connu.

1. Si vous n’avez pas encore téléchargé SharePoint Online Management Shell, téléchargez-le maintenant. Voir [téléchargement de SharePoint Online Management Shell](https://go.microsoft.com/fwlink/p/?LinkId=255251).
2. Vous devrez peut-être définir une stratégie d’exécution PowerShell pour exécuter le script. Pour plus d’informations, consultez la rubrique [à propos des stratégies d’exécution](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).
3. Exécutez le `CustomLearningConfiguration.ps1` script. En plus de vos informations d’identification d’administrateur client, le script vous invite à indiquer le nom de votre client et le nom de votre site. Dans l’exemple suivant, pour l’URL de `https://contoso.sharepoint.com/sites/O365CL`votre `contoso` site,, est le `O365CL` nom du client et est le nom du site. 

### <a name="disabling-telemetry-collection"></a>Désactivation de la collection de télémétrie
Une partie de cette solution inclut le suivi des télémétries anonyme, qui est défini par défaut sur activé. Si vous effectuez une installation manuelle et que vous souhaitez désactiver le suivi de la télémétrie, modifiez le `CustomlearningConfiguration.ps1` script de manière à définir la variable $optInTelemetry sur $false et exécutez le script.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Valider la réussite de la mise en service et initialiser la liste CustomConfig

Une fois le script PowerShell exécuté, accédez au site, initialisez l’élément de liste **CustomConfig** qui configure les voies de formation pour sa première utilisation et validez le bon fonctionnement du site.

- Accédez à `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. L’ouverture de **CustomLearningAdmin. aspx** Initialise l’élément de liste **CustomConfig** qui configure les voies de formation pour la première utilisation. Vous devriez voir une page semblable à celle-ci :

![CG-adminapppage. png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Ajouter des propriétaires au site
En tant qu’administrateur client, il est peu probable que vous soyez la personne qui personnalise le site ; vous devrez donc affecter quelques propriétaires au site. Les propriétaires disposent de privilèges d’administrateur sur le site afin qu’ils puissent modifier les pages du site et repersonnaliser le site. Ils ont également la possibilité de masquer et d’afficher le contenu fourni via le composant WebPart voies d’apprentissage. En outre, ils auront la possibilité de créer une playlist personnalisée et de les affecter à des sous-catégories personnalisées.  

1. Dans le menu **paramètres** SharePoint, cliquez sur **autorisations de site**.
2. Cliquez sur **paramètres d’autorisation avancés**.
3. Cliquez sur **voies d’apprentissage pour les propriétaires Office 365**.
4. Cliquez sur **nouveau** > **Ajouter des utilisateurs à ce groupe**, puis ajoutez les personnes que vous souhaitez être propriétaires. 
5. Ajoutez un lien pour [Explorer le site](https://docs.microsoft.com/en-us/Office365/CustomLearning/custom_explore) dans le message de partage, puis cliquez sur **partager**.

### <a name="next-steps"></a>Étapes suivantes
- [Personnaliser](custom_overview.md) l’expérience de formation pour votre organisation.

