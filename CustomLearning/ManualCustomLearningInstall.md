---
author: pkrebs
ms.author: pkrebs
title: Installation manuelle du parcours d’apprentissage
ms.date: 02/18/2019
manager: bpardi
description: Installation manuelle du parcours d’apprentissage
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: 6f106b569602730f16fc2b6f8a09fa44667e32e1
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575969"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>Installation et configuration manuelles de l’apprentissage personnalisé pour Office 365

Le microsoft Custom Learning Web Part est build à [l’aide SharePoint Framework](/sharepoint/dev/spfx/sharepoint-framework-overview) version 1.7.1.

Pour installer et configurer manuellement le partie Web Et la collection de sites, vous devez effectuer les étapes suivantes :

1. Vérifier que vous avez satisfait à toutes les conditions préalables.
1. Installez le fichier customlearning.sppkg dans Office 365 catalogue d’applications client.
1. Mise en service/identification d’un site de communication moderne qui doit agir comme votre apprentissage personnalisé pour Office 365 site d’accueil.
1. Exécutez un script PowerShell qui configurera votre client avec les artefacts appropriés dont dépend l’apprentissage personnalisé.
1. Accédez à la page du site CustomLearningAdmin.aspx pour charger le site Web d’administration afin d’initialiser la configuration de contenu personnalisée.

## <a name="prerequisites"></a>Conditions préalables

Vous devez avoir configuré et configuré le catalogue d’applications à l’échelle du client. Voir [Configurer votre client Office 365 client et](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) suivre la section Créer un site de catalogue d’applications. Si votre catalogue d’applications à l’échelle du client a déjà été configuré, vous aurez besoin d’accéder à un compte qui dispose des droits nécessaires pour télécharger un package vers celui-ci pour terminer ce processus d’installation. En règle générale, ce compte a SharePoint rôle d’administrateur principal. Si un compte avec ce rôle ne fonctionne pas, allez dans le Centre d’administration SharePoint et recherchez les administrateurs de collection de sites pour la collection de sites du catalogue d’applications et connectez-vous en tant qu’administrateurs de collection de sites, ou ajoutez le compte d’administrateur SharePoint qui a échoué aux administrateurs de collection de sites. Vous aurez également besoin d’accéder à un compte qui est un administrateur SharePoint client.

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>Télécharger web dans le catalogue d’applications client

Pour configurer l’apprentissage personnalisé Office 365, chargez le fichier customlearning.sppkg dans le catalogue d’applications à l’échelle du client et déployez-le. Voir [Utiliser le catalogue d’applications](/sharepoint/use-app-catalog) pour rendre des applications métier personnalisées disponibles pour votre environnement SharePoint Online pour obtenir des instructions détaillées sur l’ajout d’une application au catalogue d’applications.

## <a name="provisionidentify-modern-communication-site"></a>Mise en service/identification d’un site de communication moderne

Identifiez un site de communication SharePoint existant ou provisionnez-en un nouveau dans votre client SharePoint Online. Pour plus d’informations sur la mise en service d’un site de communication, voir Créer un site de communication dans [SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) et suivre les étapes de création d’un site de communication.

## <a name="set-permissions-for-the-site"></a>Définir des autorisations pour le site

Vous souhaiterez ajouter toutes les personnes qui doivent être en mesure d’afficher le contenu au groupe Visiteurs et toutes les personnes qui doivent être en mesure d’administrer des playlists personnalisées au groupe Membres. Pour configurer le site pour l’apprentissage personnalisé la première fois que l’utilisateur doit être administrateur de collection de sites ou faire partie du groupe Propriétaires.

Ajoutez l’apprentissage personnalisé Office 365 app à la collection de sites.

## <a name="execute-powershell-configuration-script"></a>Exécuter un script de configuration PowerShell

Un script PowerShell est inclus, que vous devrez exécuter pour créer trois propriétés `CustomLearningConfiguration.ps1` [de client](/sharepoint/dev/spfx/tenant-properties) que la solution utilise. En outre, le script crée deux pages d’application à composant unique dans la bibliothèque de [pages](/sharepoint/dev/spfx/web-parts/single-part-app-pages) de site pour héberger les composants Web Parts d’administrateur et d’utilisateur à un emplacement connu.

### <a name="disabling-telemetry-collection"></a>Désactivation de la collection de télémétrie

Une partie de cette solution inclut l’option de suivi de télémétrie rendue anonyme, qui est définie sur la valeur par défaut. Si vous effectuez une installation manuelle et que vous souhaitez désactiver le suivi de télémétrie, modifiez le script pour définir la `CustomlearningConfiguration.ps1` variable $optInTelemetry sur $false.

Si vous n’effectuez pas une installation manuelle et souhaitez désactiver le suivi de télémétrie, un script distinct a été inclus pour désactiver le suivi de télémétrie lors de `TelemetryOptOut.ps1` l’utilisation.

## <a name="initialize-web-part-custom-configuration"></a>Initialiser la configuration personnalisée du volet Web

Une fois le script PowerShell exécuté, accédez à `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` . Cela initialise l’élément de liste CustomConfig qui définit l’apprentissage personnalisé pour sa première utilisation.

La configuration est maintenant terminée et vous pouvez passer à l’utilisation de l’apprentissage personnalisé pour Office 365. Pour plus d’informations, voir la documentation de l’utilisateur.
