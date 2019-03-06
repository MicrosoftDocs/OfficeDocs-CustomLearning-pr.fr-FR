---
author: pkrebs
ms.author: pkrebs
title: Mise à niveau de formation personnalisée
ms.date: 02/10/2019
description: Formation personnalisée pour la configuration du composant WebPart manuel Office 365
ms.openlocfilehash: f9729c922b374cc6b775737fa7c7c76a4719534c
ms.sourcegitcommit: b6617bbbaee0784d6216e96052c2469f97cf51e9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2019
ms.locfileid: "30411894"
---
# <a name="manual-upgrade-for-custom-learning"></a>Mise à niveau manuelle de l'apprentissage personnalisé

Custom Learning for Office 365 fournit un processus de mise à niveau manuel pour les organisations qui ont participé à des projets pilotes. Avec le processus de mise à niveau, les organisations peuvent continuer à utiliser leur site d'apprentissage personnalisé actuel et effectuer une mise à niveau en ajoutant le nouveau composant WebPart d'apprentissage personnalisé amélioré à son catalogue d'applications SharePoint, puis en exécutant un script PowerShell. Vous trouverez ci-dessous une vue d'ensemble du processus de mise à niveau: 

- Vérifier que la personne chargée de télécharger le nouveau composant WebPart et d'exécuter le script PowerShell dispose des autorisations requises.
- Téléchargez le composant WebPart, customlearning. sppkg, dans votre catalogue d'applications client Office 365
- Exécuter un script PowerShell qui configurera votre client avec les artefacts appropriés requis pour l'apprentissage personnalisé
- Accédez à la page CustomLearningAdmin. aspx dans le site d'apprentissage personnalisé pour initialiser la configuration ccontent personnalisée.

## <a name="prerequisites"></a>Conditions préalables
Pour garantir la réussite de la mise à niveau de l'apprentissage personnalisé, les conditions préalables suivantes doivent être remplies. 

- Vous devez avoir configuré un catalogue d'applications à l'échelle du client. Si vous n'avez pas de catalogue d'applications client, reportez-vous à la rubrique [configurer votre client Office 365](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) et suivre la section créer un site de catalogue d'applications. 
- Si votre catalogue d'applications à l'échelle du client a déjà été configuré, vous devez accéder à un compte disposant des droits pour télécharger un package vers celui-ci. Il s'agit généralement d'un compte doté du rôle d'administrateur SharePoint. 
- Si un compte avec le rôle de l'administrateur SharePoint ne fonctionne pas: accédez au centre d'administration SharePoint, sélectionnez le catalogue d'applications, cliquez sur propriétaires, connectez-vous en tant qu'administrateur de collection de sites ou ajoutez le compte d'administrateur SharePoint qui a échoué sur le site. Liste administrateurs de collection. 

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>Étape 1: obtenir le package de composants WebPart et le script de configuration à partir de GitHub
Dans le cadre du processus de configuration, vous avez besoin du package de composants WebPart de formation personnalisé et du script de configuration PowerShell.

1. Accédez au [référentiel GitHub de formation personnalisée](https://github.com/pnp/custom-learning-office-365).
2. Cliquez sur **cloner ou télécharger**, puis **Téléchargez zip**.   
3. Enregistrez le fichier **zip** à un emplacement sur votre lecteur local.
4. ExTrayez le fichier **zip** sur votre lecteur local.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Étape 2: Télécharger le composant WebPart dans le catalogue d'applications client
Pour configurer la formation personnalisée pour Office 365, téléchargez le fichier customlearning. sppkg dans le catalogue d'applications à l'échelle du client et déployez-le. Pour obtenir des instructions détaillées sur l'ajout d'une application au catalogue d'applications, voir [utiliser le catalogue d'applications pour mettre à disposition des applications d'entreprise personnalisées pour votre environnement SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) .

1. Dans Office 365, cliquez sur **administrateur**.
2. Sous **centres d'administration**, cliquez sur **SharePoint**.
3. Cliquez sur **applications** > **catalogue** > **d'applications distribuer des applications pour SharePoint.**
4. Cliquez sur **Télécharger** > ****.
5. Dans le dossier où vous avez enregistré le fichier ZIP, sélectionnez le dossier du **composant WebPart** , puis sélectionnez **customlearning. sppkg.**
6. Cliquez sur **Déployer**.

## <a name="step-5--execute-powershell-configuration-script"></a>Étape 5-exécuter le script de configuration PowerShell
Un script `CustomLearningConfiguration.ps1` PowerShell est inclus dans le téléchargement zip à partir de github. Vous devez exécuter le script pour créer trois [Propriétés de client](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) utilisées par la solution. En outre, le script crée deux [pages d'application à composant unique](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) dans la bibliothèque pages de site pour héberger les composants WebPart administrateur et utilisateur à un emplacement connu. Ces pages d'application sont les suivantes:

- CustomAdministration. aspx
- CustomViewer. aspx

### <a name="to-run-the-powershell-script"></a>Pour exécuter le script PowerShell
- À l'aide de PowerShell `CustomLearningConfiguration.ps1` , exécutez le script situé dans le dossier WebPart à partir du zip github. Si elle réussit, vous verrez trois paires clé/valeur et l' **administrateur de formation personnalisé pour désactiver...** dans la fenêtre de commande.

### <a name="disabling-telemetry-collection"></a>DésActivation de la collection de télémétrie
L'apprentissage personnalisé inclut le suivi de télémétrie anonyme, qui est défini par défaut sur activé. Si vous souhaitez désactiver le suivi de la télémétrie, modifiez le `CustomlearningConfiguration.ps1` script pour définir la `$optInTelemetry` variable sur. `$false`

## <a name="step-6---initialize-web-part-custom-configuration"></a>Étape 6: initialiser la configuration personnalisée du composant WebPart
Une fois le script PowerShell exécuté, accédez à `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. L'ouverture de **CustomLearningAdmin. aspx** Initialise l'élément de liste **CustomConfig** qui configure la formation personnalisée pour la première utilisation. Vous devriez voir une page semblable à celle-ci:

![CG-adminapppage. png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Ajouter des propriétaires au site
En tant qu'administrateur client, il est peu probable que vous soyez la personne qui personnalise le site; vous devrez donc affecter quelques propriétaires au site. Les propriétaires disposent de privilèges d'administrateur sur le site afin qu'ils puissent modifier les pages du site et repersonnaliser le site. Ils ont également la possibilité de masquer et d'afficher le contenu fourni par le biais du composant WebPart formation personnalisée. Ils ont également la possibilité de créer une playlist personnalisée et de les affecter à des sous-catégories personnalisées.  

1. Dans le menu **paramètres** SharePoint, cliquez sur **autorisations de site**.
2. Cliquez sur **paramètres d'autorisation avancés**.
3. Cliquez sur **formation personnalisée pour les propriétaires Office 365**.
4. Cliquez sur **nouveau** > **Ajouter des utilisateurs à ce groupe**, ajoutez les personnes voulues, puis cliquez sur **partager**.

La mise à niveau est maintenant terminée. Pour en savoir plus sur la personnalisation du site de formation personnalisé et du composant WebPart pour votre environnement, voir [personnaliser l'expérience de formation](custom_overview.md).

## <a name="upgrade-instructions-for-site-owners"></a>Instructions de mise à niveau pour les propriétaires de site
Custom Learning for Office 365 a introduit diverses améliorations pour le composant WebPart. L'utilisation du composant WebPart est décrite en détail dans la section [personnaliser l'expérience d'apprentissage](custom_overview.md) . Pour le moment, le propriétaire du site doit:  

- Vérifiez que le composant WebPart formation personnalisée pour Office 365 est disponible. 
- Remplacer le composant WebPart existant sur les pages par le nouveau composant WebPart
- Remplacer tous les liens pointant vers l'ancien composant WebPart

### <a name="verify-the-custom-learning-for-office-365-web-part-is-available"></a>Vérifier que le composant WebPart formation personnalisée pour Office 365 est disponible
1.  À partir du site d'apprentissage personnalisé, cliquez sur **paramètres**, puis cliquez sur ***Ajouter une page**.
2.  Cliquez sur **+** l'icône sur la page pour ajouter un composant WebPart, puis sélectionnez le composant WebPart **formation personnalisée pour Office 365** . La page doit maintenant ressembler à ce qui suit:

[CG-adminapppage. png](media/cg-adminapppage.png)
 
### <a name="replace-the-old-web-part-with-the-new-web-part"></a>Remplacer l'ancien composant WebPart par le nouveau composant WebPart
Avant de remplacer le composant WebPart formation personnalisée ou d'apporter des modifications au site, nous vous recommandons de lire la documentation [personnaliser l'expérience d'apprentissage](custom_overview.md) car elle explique comment utiliser le nouveau composant WebPart. 

Pour mettre à niveau le site d'apprentissage personnalisé, remplacez les instances existantes du composant WebPart par le nouveau composant WebPart. Bien que nous ne pouvons pas savoir où le composant WebPart a été ajouté, les conseils pour les pilotes précédents consistaient à ajouter le composant WebPart aux pages suivantes, donc examinez-le pour remplacer le composant WebPart sur ces pages:

- Get-started-with-Office-365. aspx
- Get-started-with-Microsoft-Teams. aspx
- Get-started-with-OneDrive. aspx
- Get-started-with-SharePoint. aspx

### <a name="replace-existing-links-to-the-web-part"></a>Remplacer les liens existants par le composant WebPart
Avec les améliorations apportées au nouveau composant WebPart, les liens vers une playlist ont changé. Dans le cadre de la mise à niveau, vous devez remplacer les liens vers le composant WebPart, y compris les éléments de menu, et les liens sur la page d'accueil. Avant de remplacer le composant WebPart formation personnalisée ou d'apporter des modifications au site, nous vous recommandons de lire la documentation [personnaliser l'expérience d'apprentissage](custom_overview.md) car elle explique comment utiliser le nouveau composant WebPart. 

## <a name="recreate-existing-playlists"></a>Recréer des playlists existantes 
Pour vous assurer que les playlists fonctionnent correctement, toutes les sélections qui ont été créées avec la version antérieure du composant WebPart devront être recréées. Avant de supprimer les sélections, créez une liste des sélections personnalisées et des ressources associées afin de pouvoir les recréer facilement avec le nouveau composant WebPart d'apprentissage personnalisé. Créer une copie d'une sélection, puis la supprimer. Vous pouvez utiliser le champ JSONData pour effectuer une copie du contenu d'une sélection avant de le supprimer. Cela facilitera la création ultérieure.


• À partir du site d'apprentissage personnalisé, cliquez sur paramètres > contenu du site. • Sélectionnez une sélection, sélectionnez les ellipses, sélectionnez Modifier, puis copiez le contenu du champ JSONData et enregistrez-le dans le bloc-notes ou dans un autre document pour référence ultérieure. Sélectionnez Annuler.
• Sélectionnez la sélection, sélectionnez les ellipses, puis sélectionnez Supprimer.
• Vous êtes maintenant prêt à recréer la sélection avec le nouveau composant WebPart.
Pour obtenir des instructions sur l'utilisation du nouveau composant WebPart formation personnalisée pour https://docs.microsoft.com/en-us/office365/customlearning/custom_overviewOffice 365, reportez-vous à la rubrique.

## <a name="step-8---chan"></a>Étape 8-Chan

### <a name="next-steps"></a>Étapes suivantes
- [Personnaliser](custom_overview.md) l'expérience de formation pour votre organisation.

