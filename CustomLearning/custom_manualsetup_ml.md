---
author: pkrebs
ms.author: pkrebs
title: Configuration manuelle des voies d’apprentissage pour ml
ms.date: 02/10/2019
description: Configuration manuelle des voies d’apprentissage
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: 44bd47f0a49634a2f6ac6aca2d221fb8e6f15980
ms.sourcegitcommit: ba0cddd12dd8687ec4b97c26174fdda09de83b05
ms.contentlocale: fr-FR
ms.lasthandoff: 07/06/2020
ms.locfileid: "45043276"
---
# <a name="learning-pathways-manual-setup-for-multilingual"></a>Configuration manuelle des voies d’apprentissage pour le multilingue

Les chemins d’apprentissage Microsoft 365 offrent une configuration manuelle pour les organisations qui ont besoin d’une prise en charge pour l’un des scénarios suivants :

- Votre organisation dispose d’un site de communication moderne SharePoint Online dédié à la formation et vous souhaitez ajouter des voies de formation à ce site. Dans ce scénario, le composant WebPart voies d’apprentissage n’a pas été configuré sur le site.

- Vous souhaitez installer les voies de formation pour la prise en charge multilingue dans l’un des sites de communication SharePoint de votre organisation. Le site possède une langue par défaut qui n’est pas l’anglais et est l’une des langues prises en charge par les voies d’apprentissage. Voici les langues prises en charge par les voies de formation :

- English
- Chinois (simplifié)
- Français
- Allemand
- Italien (Italie)
- Japonais (Japon)
- Portugais (Brésil)
- Russe (russe)
- Spanish

La configuration manuelle des voies de formation nécessite l’utilisation de Windows PowerShell et de SharePoint Online Management Shell. Voici une présentation des étapes de la configuration manuelle des voies de formation : 

- Vérifiez que vous remplissez toutes les conditions préalables.
- Vérifiez les paramètres de langue par défaut pour votre site. Si ce n’est pas le cas, poursuivez l’installation manuelle. Si vous avez besoin d’un autre paramètre de langue par défaut, vous devez créer un nouveau site. 
- Installez le fichier customlearning. sppkg dans votre catalogue d’applications client SharePoint.
- Approvisionner/identifier un site de communication moderne qui se comporte comme votre site d’accueil des chemins d’apprentissage Microsoft 365.
- Exécutez un script PowerShell qui configurera votre client avec les artefacts dont dépend le chemin d’apprentissage.
- Accédez à la page de site CustomLearningAdmin. aspx pour charger le composant WebPart d’administration afin d’initialiser la configuration de contenu personnalisé.

## <a name="prerequisites"></a>Conditions préalables
Pour garantir la réussite de la configuration manuelle du composant WebPart voies d’apprentissage, les conditions préalables suivantes doivent être remplies. 

- Vous devez avoir configuré et configuré le catalogue d’applications à l’échelle du client. Consultez la rubrique [configurer votre client Office 365](https://docs.microsoft.com/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) et suivez la section « créer un catalogue d’applications ». 
- Si votre catalogue d’applications à l’échelle du client a déjà été mis en service, vous devez accéder à un compte disposant des droits pour télécharger un package vers celui-ci. En règle générale, ce compte dispose d’un rôle d’administrateur SharePoint. 
- Si un compte associé à ce rôle ne fonctionne pas, accédez au centre d’administration SharePoint et recherchez les administrateurs de collections de sites pour la collection de sites de catalogue d’applications, ou ouvrez une session en tant qu’administrateur de collection de sites ou ajoutez le compte d’administrateur SharePoint qui a échoué aux administrateurs de collection de sites. 
- Vous aurez également besoin d’accéder à un compte qui est un administrateur de client SharePoint.

## <a name="step-1---check-your-language-settings"></a>Étape 1 : vérifier vos paramètres de langue
Lors de la première étape du processus d’installation manuelle, vérifiez les paramètres de langue de votre site. Les options possibles sont les suivantes :

### <a name="option-1---you-dont-want-multilingual-support"></a>Option 1 : vous ne voulez pas de prise en charge multilingue
Si vous ne voulez pas de prise en charge multilingue pour votre site, vérifiez qu’elle est désactivée.
1.  À partir du site de communication SharePoint, sélectionnez **paramètres**du  >  **site informations**  >  **Afficher tous les**paramètres de langue des paramètres du site  >  **Language settings**. 
2.  Définissez le commutateur **activer la traduction des pages et des informations en plusieurs langues** sur **désactivé**.
3.  Cliquez sur **Enregistrer**. 
4.  Passez à l’étape 2.

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>Option 2 : vous souhaitez une prise en charge multilingue et vous êtes OK avec la langue par défaut
Un site de communication SharePoint possède une langue par défaut. La langue par défaut détermine la langue dans laquelle vous visualisez les voies de formation, y compris la page d’administration des voies d’apprentissage. Le paramètre de langue par défaut est défini lors de la création initiale du site et ne peut pas être modifié par la suite. Avant de poursuivre la configuration manuelle, vérifiez que vous êtes OK avec la langue par défaut du site cible.

1.  À partir du site de communication SharePoint, sélectionnez **paramètres**du  >  **site informations**  >  **Afficher tous les**paramètres de langue des paramètres du site  >  **Language settings**. 
2.  Définissez le commutateur **activer la traduction des pages et des informations en plusieurs langues** sur **activé**.
    - Si vous êtes OK avec la langue qui apparaît en haut de la liste sous **langue**, vous pouvez ajouter des langues supplémentaires, puis cliquez sur **Enregistrer**. Passez à l’étape 2.
    - Si vous souhaitez utiliser une langue par défaut différente de celle sélectionnée pour le site, vous devez créer un nouveau site de communication SharePoint avec la langue de votre choix. Passez à l’option 3. 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>Option #3-vous souhaitez une prise en charge multilingue mais souhaitez une autre langue par défaut pour le site
Avec cette option, vous créez un site de communication SharePoint Online avec la langue par défaut souhaitée, puis définissez les paramètres de langue pour le site. 
1.  Pour créer un nouveau site de communication SharePoint, voir [créer un site de communication dans SharePoint Online](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb). Lors de la création du site, veillez à définir la langue sur la langue par défaut souhaitée pour les voies d’apprentissage. 
2. À partir du site que vous avez créé, sélectionnez **paramètres**des  >  **informations de site**  >  **Afficher tous les**paramètres de langue des paramètres du site  >  **Language settings**. 
2.  Définissez le commutateur **activer la traduction des pages et des informations en plusieurs langues** sur **activé**.
3. Ajoutez des langues supplémentaires, si nécessaire, puis cliquez sur **Enregistrer**. 
4. Passez à l’étape 2. 

>! Note Si vous devez migrer le contenu personnalisé d’un site vers un site nouvellement créé, reportez-vous à la section « migrer du contenu personnalisé » plus loin dans ce document. 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>Étape 2 : obtenir le package de composants WebPart et le script de configuration à partir de GitHub
Dans le cadre du processus de configuration, vous avez besoin du package de composants WebPart des chemins d’apprentissage Microsoft 365 et du script de configuration de PowerShell.

- Accédez au [référentiel GitHub des voies d’apprentissage](https://github.com/pnp/custom-learning-office-365).
- Cliquez sur **Télécharger** pour enregistrer le package de composants WebPart et le script sur un lecteur local. Vous utiliserez le script et le package de composants WebPart dans les étapes ultérieures de ce processus.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Étape 2 : Télécharger le composant WebPart dans le catalogue d’applications client
Pour configurer les voies d’apprentissage de Microsoft 365, téléchargez le fichier customlearning. sppkg dans le catalogue d’applications à l’échelle du client et déployez-le. Pour obtenir des instructions détaillées sur la façon d’ajouter une application au catalogue d’applications, voir [utiliser le catalogue d’applications pour mettre à disposition des applications d’entreprise personnalisées pour votre environnement SharePoint Online](https://docs.microsoft.com/sharepoint/use-app-catalog) .

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>Étape 3 : configurer/identifier un site de communication moderne
Identifiez un site de communication SharePoint existant ou approvisionnez-en un nouveau dans votre client SharePoint Online. Pour plus d’informations sur la mise en service d’un site de communication, voir [créer un site de communication dans SharePoint Online](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) et suivre les étapes de création d’un site de communication.

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>Étape 4 : ajouter l’application des chemins d’apprentissage Microsoft 365 au site

1. À partir du site SharePoint, cliquez sur le menu système, puis cliquez sur **Ajouter une application**. 
2. Sous **vos applications**, cliquez sur **à partir de votre organisation**, puis cliquez sur **parcours de formation pour Office 365**. 

## <a name="step-5---set-permissions-for-the-site"></a>Étape 5 : définir des autorisations pour le site
Assurez-vous que les autorisations suivantes sont définies pour le site :
- **Administrateur de la collection de sites ou partie du groupe propriétaires** : autorisations requises pour initialiser l’élément de liste CustomConfig qui configure les voies de formation pour sa première utilisation. 
- **Groupe de membres** -autorisations requises pour administrer les voies de formation, y compris le masquage et l’affichage du contenu, ainsi que l’administration des playlists personnalisées
- **Groupe visiteurs** -autorisations requises pour afficher le contenu du site. 

## <a name="step-6--execute-powershell-configuration-script"></a>Étape 6-exécuter le script de configuration PowerShell
Un script PowerShell `CustomLearningConfiguration.ps1` est inclus que vous devrez exécuter pour créer trois propriétés de [client](https://docs.microsoft.com/sharepoint/dev/spfx/tenant-properties) utilisées par la solution. En outre, le script crée deux [pages d’application à composant unique](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/single-part-app-pages) dans la bibliothèque pages de site pour héberger les composants WebPart administrateur et utilisateur à un emplacement connu.

1. Si vous n’avez pas encore téléchargé SharePoint Online Management Shell, téléchargez-le maintenant. Voir [téléchargement de SharePoint Online Management Shell](https://go.microsoft.com/fwlink/p/?LinkId=255251).
2. Vous devrez peut-être définir une stratégie d’exécution PowerShell pour exécuter le script. Pour plus d’informations, consultez la rubrique [à propos des stratégies d’exécution](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).
3. Exécutez le `CustomLearningConfiguration.ps1` script. En plus de vos informations d’identification d’administrateur client, le script vous invite à indiquer le nom de votre client et le nom de votre site. Dans l’exemple suivant, pour l’URL de votre site, `https://contoso.sharepoint.com/sites/O365CL` , `contoso` est le nom du client et `O365CL` est le nom du site. 

### <a name="disabling-telemetry-collection"></a>Désactivation de la collection de télémétrie
Une partie de cette solution inclut le suivi des télémétries anonyme, qui est défini par défaut sur activé. Si vous effectuez une installation manuelle et que vous souhaitez désactiver le suivi de la télémétrie, modifiez le `CustomlearningConfiguration.ps1` script de manière à définir la variable $optInTelemetry sur $false et exécutez le script.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Valider la réussite de la mise en service et initialiser la liste CustomConfig

Une fois le script PowerShell exécuté, accédez au site, initialisez l’élément de liste **CustomConfig** qui configure les voies de formation pour sa première utilisation et validez le bon fonctionnement du site.

- Accédez à `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. L’ouverture de **CustomLearningAdmin. aspx** Initialise l’élément de liste **CustomConfig** qui configure les voies de formation pour la première utilisation. Vous devriez voir une page semblable à celle-ci :

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Ajouter des propriétaires au site
En tant qu’administrateur client, il est peu probable que vous soyez la personne qui personnalise le site ; vous devrez donc affecter quelques propriétaires au site. Les propriétaires disposent de privilèges d’administrateur sur le site afin qu’ils puissent modifier les pages du site et repersonnaliser le site. Ils ont également la possibilité de masquer et d’afficher le contenu fourni via le composant WebPart voies d’apprentissage. En outre, ils auront la possibilité de créer une playlist personnalisée et de les affecter à des sous-catégories personnalisées.  

1. Dans le menu **paramètres** SharePoint, cliquez sur **autorisations de site**.
2. Cliquez sur **paramètres d’autorisation avancés**.
3. Cliquez sur **voies d’apprentissage pour les propriétaires Office 365**.
4. Cliquez sur **nouveau**  >  **Ajouter des utilisateurs à ce groupe**, puis ajoutez les personnes que vous souhaitez être propriétaires. 
5. Ajoutez un lien pour [Explorer le site](https://docs.microsoft.com/Office365/CustomLearning/custom_explore) dans le message de partage, puis cliquez sur **partager**.

## <a name="migrate-custom-content"></a>Migrer du contenu personnalisé
Une fois que vous avez rétablissez votre site de voies d’apprentissage en suivant les étapes ci-dessus, vous devrez déplacer le contenu de votre liste **CustomPlaylists** et de votre liste **CustomAssets** . Vous pouvez également déplacer les pages personnalisées réelles qui composent vos biens personnalisés si elles résident sur le site des voies d’apprentissage existantes, et que votre intention est de la supprimer. La tâche peut être difficile, car pour tous les éléments de la liste **CustomPlaylists** , l’ID de l’élément de liste dans la liste **CustomAssets** est enfoui dans le champ JSONData de chaque élément de liste de playlist. Par conséquent, le simple fait de simplement délimiter le contenu de la liste **CustomPlaylists** d’un site à l’autre sera insuffisant. De plus, la liste **CustomAssets** contient l’URL absolue de la page de l’élément personnalisé dans le champ JSONData de l’élément de liste. Si les ressources ne sont pas déplacées et que le site n’est pas renommé (ce qui modifie l’URL absolue vers la page de l’élément), **CustomAssets** peut être conservé. Toutefois, vous devrez corriger manuellement les entrées. Étant donné la complexité de ce type de migration, nous vous conseillons d’avoir inscrit l’un de nos partenaires de parcours de formation pour vous aider à effectuer cette transition. 

### <a name="next-steps"></a>Étapes suivantes
- Voir [Customize Learning voies](custom_overview.md). 
- Voir [traduire des pages de site](custom_translate_page_ml.md).

