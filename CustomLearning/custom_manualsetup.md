---
author: pkrebs
ms.author: pkrebs
title: Configuration manuelle du parcours d’apprentissage
ms.date: 07/06/2020
description: Configuration manuelle du parcours d’apprentissage Microsoft 365
ms.service: sharepoint-online
ms.openlocfilehash: 5cc2f641884871fcb33d6cf7ea0db885fcdbd019
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999610"
---
# <a name="learning-pathways-manual-setup"></a>Configuration manuelle du parcours d’apprentissage

Le parcours d’apprentissage de Microsoft 365 offre une configuration manuelle pour les organisations qui ont besoin d’une prise en charge pour l’un des scénarios suivants : 

- Votre organisation dispose d’un site de communication moderne SharePoint Online établi dédié à la formation et vous souhaitez ajouter des parcours d’apprentissage à ce site. Dans ce scénario, le volet Web du parcours d’apprentissage n’a pas été installé sur le site.

- Vous souhaitez installer les parcours d’apprentissage pour la prise en charge multilingue dans l’un des sites de communication SharePoint de votre organisation. Le site a ou aura une langue par défaut qui n’est pas l’anglais et qui est l’une des langues pris en charge par le parcours d’apprentissage. Voici les langues prise en charge par le parcours d’apprentissage :

- Français
- Chinois (simplifié)
- Français
- Allemand
- Italien (Italie)
- Japonais (Japon)
- Portugais (Brésil)
- Russe (russe)
- Espagnol

La configuration manuelle des parcours d’apprentissage nécessite une expérience de Windows PowerShell et de SharePoint Online Management Shell. Voici une vue d’ensemble des étapes de la configuration manuelle du parcours d’apprentissage : 

- Vérifier que vous avez satisfait à toutes les conditions préalables.
- Vérifiez les paramètres de langue par défaut de votre site. Si ok, poursuivez l’installation manuelle. Si vous avez besoin d’un autre paramètre de langue par défaut, vous devez créer un site. 
- Installez le fichier customlearning.sppkg dans votre catalogue d’applications client SharePoint.
- Mettre en service/identifier un site de communication moderne pour agir en tant que site d’accueil du parcours d’apprentissage Microsoft 365.
- Exécutez un script PowerShell qui configurera votre client avec les artefacts dont dépend le parcours d’apprentissage.
- Accédez à la page du site CustomLearningAdmin.aspx pour charger le site Web d’administration afin d’initialiser la configuration de contenu personnalisé.

## <a name="prerequisites"></a>Conditions préalables
Pour garantir une configuration manuelle réussie du volet Web du parcours d'apprentissage, les conditions préalables suivantes doivent être remplies. 

- Vous devez avoir configuré et configuré le catalogue d'applications à l'échelle du client. Voir [Configurer votre client Office 365](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) et suivre la section « Créer un catalogue d'applications ». 
- Si votre catalogue d'applications à l'échelle du client a déjà été mis en service, vous devez accéder à un compte dispose des droits nécessaires pour y télécharger un package. En règle générale, ce compte a un rôle d'administrateur SharePoint. 
- Si un compte avec ce rôle ne fonctionne pas, allez dans le Centre d'administration SharePoint et recherchez les administrateurs de collection de sites pour la collection de sites catalogue d'applications et connectez-vous en tant qu'administrateurs de collection de sites, ou ajoutez le compte d'administrateur SharePoint qui a échoué aux administrateurs de collection de sites. 
- Vous aurez également besoin d'accéder à un compte qui est un administrateur client SharePoint.

## <a name="step-1---check-your-language-settings"></a>Étape 1 : vérifier vos paramètres de langue
Comme première étape du processus d'installation manuelle, vérifiez les paramètres de langue de votre site. Voici les options possibles :

### <a name="option-1---you-dont-want-multilingual-support"></a>Option 1 : vous ne souhaitez pas une prise en charge multilingue
Si vous ne souhaitez pas une prise en charge multilingue de votre site, assurez-vous qu'il est désactivé.
1.  À partir du site de communication SharePoint, sélectionnez **Paramètres**  >  **Informations du site** Afficher tous les  >  **paramètres du site**  >  **Paramètres de langue.** 
2.  Définissez **le commutateur Activer les pages et les actualités à** traduire en plusieurs langues pour **qu'ils soient éteints.**
3.  Cliquez sur **Enregistrer**. 
4.  Continuez jusqu'à l'étape 2.

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>Option 2 : vous souhaitez une prise en charge multilingue et la langue par défaut vous va bien
Un site de communication SharePoint a une langue par défaut. La langue par défaut détermine la langue dans laquelle vous affichez les parcours d'apprentissage, y compris la page Administration des parcours d'apprentissage. Le paramètre de langue par défaut est définie lors de la création du site et ne peut pas être modifiée par la suite. Avant de poursuivre l'installation manuelle, assurez-vous que la langue par défaut du site cible vous est correcte.

1.  À partir du site de communication SharePoint, sélectionnez **Paramètres**  >  **Informations du site** Afficher tous les  >  **paramètres du site**  >  **Paramètres de langue.** 
2.  Définissez **le commutateur Activer les pages et les actualités** à traduire en plusieurs **langues.**
    - Si vous êtes d'accord avec la langue qui apparaît en haut de la liste sous **Langue,** vous pouvez ajouter des langues supplémentaires, puis cliquer sur **Enregistrer**. Continuez jusqu'à l'étape 2.
    - Si vous souhaitez une langue par défaut différente de celle sélectionnée pour le site, vous devez créer un nouveau site de communication SharePoint avec la langue de votre choix. Continuez jusqu'à l'option 3. 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>Option #3 : vous souhaitez une prise en charge multilingue, mais vous souhaitez une autre langue par défaut pour le site
Avec cette option, vous créez un nouveau site de communication SharePoint Online avec la langue par défaut de votre choix, puis définissez les paramètres de langue pour le site. 
1.  Pour créer un nouveau site de communication SharePoint, voir [Créer un site de communication dans SharePoint Online.](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) Lors de la création du site, assurez-vous de définir la langue par défaut pour le parcours d'apprentissage. 
2. À partir du site que vous avez créé, sélectionnez **Paramètres**  >  **Informations sur le site** Afficher tous les  >  **paramètres de langue** des  >  **paramètres du site.** 
2.  Définissez **le commutateur Activer les pages et actualités** à traduire en plusieurs **langues.**
3. Ajoutez des langues supplémentaires, si nécessaire, puis cliquez sur **Enregistrer.** 
4. Continuez jusqu'à l'étape 2. 

>! [Remarque] Si vous devez migrer du contenu personnalisé d'un site vers un site nouvellement créé, consultez la section « Migrer le contenu personnalisé » plus loin dans ce document. 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>Étape 2 : obtenir le package de partie Web Et le script d'installation à partir de GitHub
Dans le cadre du processus de configuration, vous aurez besoin du package de volets d'apprentissage De Microsoft 365 et du script d'installation de PowerShell.

- Allez dans le référentiel GitHub du [parcours d'apprentissage.](https://github.com/pnp/custom-learning-office-365)
- Cliquez **sur Télécharger** pour enregistrer le package de partie Web Et le script sur un lecteur local. Vous utiliserez le script et le package de partie Web Dans les étapes ultérieures de ce processus.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Étape 2 : Télécharger le partie Web Dans le catalogue d'applications client
Pour configurer le parcours d'apprentissage de Microsoft 365, téléchargez le fichier customlearning.sppkg dans le catalogue d'applications à l'échelle du client et déployez-le. Voir Utiliser le catalogue d'applications pour rendre des applications métier personnalisées disponibles pour votre environnement [SharePoint Online](/sharepoint/use-app-catalog) pour obtenir des instructions détaillées sur l'ajout d'une application au catalogue d'applications.

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>Étape 3 : mise en service/identification d'un site de communication moderne
Identifiez un site de communication SharePoint existant ou provisionnez-en un nouveau dans votre client SharePoint Online. Pour plus d'informations sur la mise en service d'un site de communication, voir Créer un site de communication dans [SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) et suivre les étapes de création d'un site de communication.

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>Étape 4 : ajouter l'application de parcours d'apprentissage Microsoft 365 au site

1. À partir du site SharePoint, cliquez sur le menu Système, puis cliquez **sur Ajouter une application.** 
2. Sous **Vos applications,** cliquez **sur À partir de votre** organisation, puis cliquez sur Parcours d'apprentissage pour Office **365.** 

## <a name="step-5---set-permissions-for-the-site"></a>Étape 5 : définir des autorisations pour le site
Assurez-vous que les autorisations suivantes sont définies pour le site :
- **Administrateur de collection de** sites ou partie du groupe Propriétaires : autorisations requises pour initialiser l'élément de liste CustomConfig qui définit le parcours d'apprentissage pour sa première utilisation. 
- **Groupe Membres** : autorisations requises pour administrer les parcours d'apprentissage, notamment le masquage et l'affichage de contenu et l'administration des sélections personnalisées
- **Groupe Visiteurs** : autorisations requises pour afficher le contenu du site. 

## <a name="step-6--execute-powershell-configuration-script"></a>Étape 6 : exécuter un script de configuration PowerShell
Un script PowerShell est inclus, que vous devrez exécuter pour créer trois propriétés `CustomLearningConfiguration.ps1` [de client](/sharepoint/dev/spfx/tenant-properties) que la solution utilise. En outre, le script crée deux pages d'application à composant unique dans la bibliothèque de [pages](/sharepoint/dev/spfx/web-parts/single-part-app-pages) de site pour héberger les composants Web Parts d'administrateur et d'utilisateur à un emplacement connu.

1. Si vous n'avez pas encore téléchargé SharePoint Online Management Shell, téléchargez-le maintenant. Voir [téléchargement de SharePoint Online Management Shell.](https://go.microsoft.com/fwlink/p/?LinkId=255251)
2. Vous devrez peut-être définir une stratégie d'exécution PowerShell pour exécuter le script. Pour plus d'informations, voir [À propos des stratégies d'exécution.](/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)
3. Exécutez `CustomLearningConfiguration.ps1` le script. En plus de vos informations d'identification d'administrateur client, le script vous invite à vous faire part de votre nom de client et de votre nom de site. L'exemple suivant, pour l'URL de votre site, est le nom du client `https://contoso.sharepoint.com/sites/O365CL` et le nom du `contoso` `O365CL` site. 

### <a name="disabling-telemetry-collection"></a>Désactivation de la collection de télémétrie
Une partie de cette solution inclut l'option d'option de suivi de télémétrie rendue anonyme, qui est définie sur la valeur par défaut. Si vous exécutez une installation manuelle et que vous souhaitez désactiver le suivi de télémétrie, modifiez le script pour définir la variable $optInTelemetry sur $false et exécutez `CustomlearningConfiguration.ps1` le script.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Valider la réussite de l'approvisionnement et initialiser la liste CustomConfig

Une fois le script PowerShell exécuté, vous accédez au site, initialisez l'élément de liste **CustomConfig** qui définit le parcours d'apprentissage pour sa première utilisation et validez que le site fonctionne.

- Accédez à `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. L’ouverture de **CustomLearningAdmin.aspx** initialise l'élément de liste **CustomConfig** qui configure le parcours d’apprentissage pour la première utilisation. Vous devriez voir une page qui ressemble à ceci :

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Ajouter des propriétaires au site
En tant qu'administrateur client, il est peu probable que vous soyez la personne qui personnalisant le site, vous devrez donc affecter quelques propriétaires au site. Les propriétaires ont des privilèges d'administration sur le site pour pouvoir modifier les pages du site et renommer le site. Ils ont également la possibilité de masquer et d'afficher le contenu remis via le volet Web Du parcours d'apprentissage. En outre, ils ont la possibilité de créer une playlist personnalisée et de les affecter à des sous-catégories personnalisées.  

1. Dans le menu **Paramètres** SharePoint, cliquez sur **Autorisations du site.**
2. Cliquez **sur Paramètres d'autorisation avancés.**
3. Cliquez **sur parcours d'apprentissage pour les propriétaires d'Office 365.**
4. Cliquez **sur**  >  **Ajouter des utilisateurs à ce groupe,** puis ajoutez les personnes que vous souhaitez être propriétaires. 
5. Ajoutez un lien [vers Explorer le site](https://docs.microsoft.com/Office365/CustomLearning/custom_explore) dans le message de partage, puis cliquez sur **Partager.**

## <a name="migrate-custom-content"></a>Migrer du contenu personnalisé
Après avoir rétabli votre site de parcours d'apprentissage en suivant les étapes ci-dessus, vous devez déplacer le contenu de votre liste **CustomPlaylists** et de votre liste **CustomAssets.** Vous pouvez également, si vous le souhaitez, déplacer les pages personnalisées réelles qui constitueront vos ressources personnalisées si elles existent dans le site de parcours d'apprentissage existant, et votre intention est de les supprimer. La tâche peut être difficile, car pour tous les éléments de la liste **CustomPlaylists,** l'ID de l'élément de liste dans la liste **CustomAssets** est insérez dans le champ JSONData de chaque élément de liste de playlist. Ainsi, le simple déplacement du contenu de la liste **CustomPlaylists** d'un site à l'autre ne sera pas suffisant. En outre, la **liste CustomAssets** contient l'URL absolue de la page de la bien personnalisée dans le champ JSONData de l'élément de liste. Si les ressources ne sont pas déplacées et que le site n'est pas renommé (en modifiant l'URL absolue sur la page de la bien), **CustomAssets** peut rester. Mais vous devrez corriger manuellement les entrées. Étant donné la complexité de ce type de migration, nous vous suggérons de faire appel à l'un de nos partenaires de parcours d'apprentissage pour vous aider à effectuer cette transition. 

### <a name="next-steps"></a>Étapes suivantes
- Voir [Personnaliser le parcours d'apprentissage.](custom_overview.md) 
- Voir [Traduire les pages du site.](custom_translate_page_ml.md)