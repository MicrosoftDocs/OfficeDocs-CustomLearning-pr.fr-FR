---
author: pkrebs
ms.author: pkrebs
title: Modèles d’intégration de partenaires
ms.date: 3/9/2019
description: Modèles d’intégration de partenaires
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: a91cdf4ee6aa3bbc22033dd484605ea5405b3c4c
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575989"
---
# <a name="partner-integration-models"></a>Modèles d’intégration de partenaires
Bien qu’il soit impossible de compléter directement le contenu du parcours d’apprentissage Microsoft 365 à partir du service d’approvisionnement SharePoint Online, les partenaires peuvent tirer parti de plusieurs modèles d’intégration pour créer des offres de services d’ajout de valeurs alignées. Les modèles d’intégration des partenaires ci-dessus sont présentés par ordre croissant de complexité et de niveaux d’investissement. Par conséquent, nous vous aiderons à développer votre expertise et à aller à des niveaux plus avancés en fonction de vos modèles d’entreprise.

![Flow affiche le rôle des enableurs, des intégrateurs et des redistibuteurs.](media/cg-part-intmodel.png)

## <a name="how-should-i-get-started"></a>Comment dois-je commencer ? 
Pour commencer, voici quelques meilleures pratiques à suivre.     

### <a name="1-begin-with-building-expertise-as-an-enabler"></a>1. Commencez par créer une expertise en tant qu’enableur. 
Vous pouvez aider un pourcentage de votre base de clients immédiatement en activant son portail de formation de parcours d’apprentissage et en activant une curation de contenu Microsoft ciblée. Pour obtenir des instructions sur la mise en service des parcours d’apprentissage, voir La mise en service d’une [nouvelle solution de parcours d’apprentissage.](/office365/customlearning/custom_provision)  

### <a name="2-then-extend-your-services-as-an-integrator"></a>2. Étendez ensuite vos services en tant qu’intégrateur
Effectuer une analyse de retour sur investissement d’automatisation, en fonction de la quantité de votre contenu et/ou des besoins d’intégration de services. Par exemple, il peut ne pas être logique de prendre en compte les coûts de développement et d’exploitation par rapport à nos recommandations en matière d’intégration de contenu si vous pouvez créer manuellement une ou plusieurs playlists personnalisées ciblées pointant vers votre contenu payant ou référencer vos services.

### <a name="3-when-the-return-on-investment-makes-sense--consider-redistribution"></a>3. Lorsque le retour sur investissement est logique , envisagez la redistribution 
Lorsque le retour sur investissement est logique , envisagez de redistribuer (ou de travailler avec des partenaires du parcours d’apprentissage associés) pour créer des solutions repackaged. Ceux-ci sont basés sur l’infrastructure SharePoint modèles et pratiques qui fournit des solutions pour extraire des sites personnalisés, puis les déployer dans les environnements clients 

## <a name="partner-provided-content-integration-guidelines"></a>Recommandations en matière d’intégration de contenu fournies par les partenaires
Le contenu pour Microsoft 365 parcours d’apprentissage est piloté par un ensemble de fichiers JSON qui agissent comme des manifestes de contenu pour votre package d’apprentissage. Il existe trois fichiers : metadata.js, playlists.jset assets.js. Ces fichiers doivent être structurés pour correspondre aux modèles reconnus par le partie Web Part, puis hébergés à partir d’un réseau de distribution de contenu (CDN) pour permettre au partie Web De les charger. Microsoft fournit des modèles de démarrage de ces fichiers pour vous aider à démarrer.  

**Clause d’exclusion de responsabilité** : la structure de fichier JSON est sujette à modification en fonction du travail à venir de la solution. Le Microsoft 365 programme d’adoption précoce (EAP) du partenaire du parcours d’apprentissage sera informé des changements majeurs de cette nature. Ainsi que les conseils de transition et/ou de compatibilité ascendante des clients. 

### <a name="download-the-microsoft-365-learning-pathways-solution"></a>Télécharger la solution Microsoft 365 parcours d’apprentissage
Vous pouvez télécharger la solution Microsoft 365 parcours d’apprentissage, ainsi que les fichiers JSON, à partir GitHub référentiel : https://github.com/pnp/custom-learning-office-365 . Notez qu’à ce jour, Microsoft ne prend pas GitHub de pull sur la solution. Toutefois, vous pouvez utiliser les fichiers GitHub comme point de départ pour créer votre propre pack de contenu personnalisé. 

### <a name="metadatajson-structure"></a>Metadata.jsstructure
Vous pouvez voir ce fichier comme le brains des menus et de la structure. Il contient toute la structure de navigation ainsi que les listes de sélection des données dans les deux autres fichiers. 


|              Nom        |                     Description                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|**Technologies**              |Le contenu est balisé et peut être masqué en fonction de la technologie qui lui est affectée.                 |  
|&nbsp;&nbsp;ID                |GUID représentant la technologie                                                           |  
|&nbsp;&nbsp;Nom              |Nom complet de la technologie                                                             |
|&nbsp;&nbsp;*Subjects[ ]*     |Tableau de sujets qui sont un sous-ensemble de la technologie                                   | 
|&nbsp;&nbsp;&nbsp;&nbsp;ID    |GUID représentant l’objet                                                              |
|&nbsp;&nbsp;&nbsp;&nbsp;Nom  |Nom complet de l’objet                                                                |
|**Catégories [ ]**             |Les catégories informent la navigation du webpart. Chaque catégorie représente un niveau supérieur de la navigation                                                                                                                 |
|&nbsp;&nbsp;ID                |GUID représentant la catégorie/sous-catégorie                                                 |
|&nbsp;&nbsp;Nom              |Nom complet de la catégorie/sous-catégorie                                                  |
|&nbsp;&nbsp;Image             |URL de l’image qui doit être affichée dans l’UX (par rapport à la base de CDN)            |
|&nbsp;&nbsp;TechnologyId      |GUID de la technologie à qui ce contenu est lié (facultatif – chaîne vide)            |
|&nbsp;&nbsp;SubjectId         |GUID de l’objet lié à ce contenu (facultatif – chaîne vide)               |
|&nbsp;&nbsp;Source            |À partir du tableau source, non spécifiquement utilisé dans l’expérience utilisateur autre que les données personnalisées ajoutées par l’utilisateur est marqué comme « client » et la zone d’administration de l’expérience utilisateur n’autorise pas la modification de tout ce qui n’est pas marqué « Client ».                           |
|&nbsp;&nbsp;*Sous-catégories[ ]*|Sub-Categories sont essentiellement le niveau de navigation du niveau 2 vers le bas. La structure est identique à une catégorie imbrique.          |
|**Audiences [ ]**             |Lorsque les playlists associées à une catégorie/sous-catégorie sont marquées par différentes audiences, un sélecteur est disponible pour afficher les audiences disponibles. |         
|&nbsp;&nbsp;ID                |GUID de l’audience                                                                       |  
|&nbsp;&nbsp;Nom              |Nom d’affichage de l’audience                                                               |       
|**Sources [ ]**               |Le tableau de chaînes qui balisent le contenu avec sa source, non spécifiquement utilisé dans l’expérience utilisateur autre que les données personnalisées ajoutées par l’utilisateur est marqué comme « client » et la zone d’administration de l’expérience utilisateur n’autorise pas la modification de tout ce qui n’est pas marqué « Client ».                                                   |  
|**Niveaux [ ]**               |Lorsque les playlists associées à une catégorie/sous-catégorie sont marquées à différents niveaux, un sélecteur est disponible pour afficher les niveaux disponibles.             |  
|&nbsp;&nbsp;ID                |GUID du niveau                                                                          |  
|&nbsp;&nbsp;Nom              |Nom complet du niveau                                                                  | 
|**StatusTag [ ]**           |La balise d’état consiste à identifier le contenu avec différents états qui seront exposés dans l’UX. Certains de ces indicateurs s’afficheront pour le consommateur et d’autres uniquement pour l’administrateur.                                                   |  
|&nbsp;&nbsp;ID                |GUID de l’élément DontgTag                                                                      |  
|&nbsp;&nbsp;Nom              |Nom d’affichage du statustag                                                              | 
|**Télémétrie [ ]**            |                                                                                           |  
|&nbsp;&nbsp;AppInsightsKey    |GUID de la clé d’informations de l’application que vous avez définie pour suivre le chargement du partie Web De la visionneuse. Le suivi peut être désactivé par un administrateur pour l’ensemble du client, mais les informations envoyées sont des utilisateurs anonymisés avec l’ID de client. Pour plus d’informations, consultez cette section. https://github.com/pnp/custom-learning-office-365#disabling-telemetry-collection               |  
|**Version**                   |Les informations de version sont utilisées par la solution pour indiquer aux administrateurs que le webpart a été mis à jour et permettre également au webpart de mettre à jour le contenu personnalisé vers la dernière version du manifeste si des modifications importantes ont été apportées.         | 
|&nbsp;&nbsp;Manifeste          |Version du manifeste                                               |
|&nbsp;&nbsp;ManifestMinWebPart|Version minimale du webpart qui fonctionne avec la version du manifeste             |
|&nbsp;&nbsp;CurrentWebPart    |URL de l’image qui doit être affichée dans l’UX (par rapport à la base de CDN)            |
|&nbsp;&nbsp;RepoURL           |URL du référentiel dans lequel se trouve les instructions de mise à jour du site Web Part.                    |
|**Packs de contenu**             |Pour l’instant, les packs de contenu pour CDN’autres ne sont pas pris en charge. Les packs de contenu permettent à Microsoft de suggérer d’autres solutions créées par Microsoft qui peuvent être mis en service via le service d’approvisionnement qui exploitent M365LP pour fournir du contenu et qui se trouvent dans et par eux-mêmes des CDN personnalisés.       | 
|&nbsp;&nbsp;ID                |GUID du pack de contenu/CDN                                                              |
|&nbsp;&nbsp;Nom              |Nom d’affichage du CDN                                                                   |
|&nbsp;&nbsp;Description       |Description à afficher dans l’interface utilisateur pour l’ajout d’un pack de contenu                               |
|&nbsp;&nbsp;Image             |Image à afficher dans l’interface utilisateur pour l’ajout d’un pack de contenu                                     |
|&nbsp;&nbsp;ProvisionURL      |URL du package de service d’approvisionnement pour créer la collection de sites du pack de contenu  |
|&nbsp;&nbsp;CDNbase           |URL de base pour les manifestes du pack de contenu                                       |
|AssetOrigins                  |Tableau d’origine d’URL utilisé dans le assets.jsfichier décrit plus loin. Si l’URL d’origine la prend en charge, un message de publication est envoyé help_getClientHeight. Une réponse dans la propriété de données de : « help_getClientHeight={height of content} » (par exemple « help_getClientHeight=5769 ») permet de re reserrer l’iFrame à la hauteur appropriée du contenu d’origine.         |

### <a name="playlistsjson-structure"></a>Playlists.jsstructure
playlists.js- Le manifeste des playlists est un tableau d’objets qui décrivent les métadonnées sur une playlist et les ressources incluses dans la playlist.

|              Nom        |                     Description                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|ID                            |GUID représentant la playlist                                                             |  
|Titre                         |Nom complet de la playlist                                                               |
|Image                         |URL relative (à partir de CDN) vers une image pour visualiser la playlist                              |                      
|LevelId                       |Niveau associé                                                                           |
|AudienceId                   |Public associé                                                                        |
|TechnologyId                 |Technologie associée                                                                      |
|SubjectId                    |Nom complet de la catégorie/sous-catégorie                                                  |
|Source                        |À partir du tableau source, non spécifiquement utilisé dans l’expérience utilisateur autre que les données personnalisées ajoutées par l’utilisateur est marqué comme « client » et la zone d’administration de l’expérience utilisateur n’autorise pas la modification de tout ce qui n’est pas marqué « Client ».                                              |
|CatId                         |ID de catégorie ou de sous-catégorie qui représente le conteneur dans qui la playlist doit être affichée. Actuellement, le manifeste ne prend pas en charge la sélection d’une catégorie ou d’une sous-catégorie comme conteneur s’il a également des enfants de sous-catégorie.        |
|Description                   |Description de chaque sélection dans l’UX                                           |
|StatusTagId                   |Balise d’état associée                                                                      |
|StatusNote                    |Remarques sur le contenu affiché aux administrateurs                                            |
|*Assets[]*                        |Tableau de GUID pour les ressources qui font partie de cette playlist, dans l’ordre d’affichage.        |         

### <a name="assetjson-structure"></a>Asset.jsstructure
playlists.js- Le manifeste des playlists est un tableau d’objets qui décrivent les métadonnées sur une playlist et les ressources incluses dans la playlist.

|              Nom        |                     Description                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|ID                            |GUID représentant la playlist                                                             |  
|Titre                         |Nom complet de la playlist                                                               |
|Description                   |---                                                                                           |                      
|URL                           |URL source de la bien, à appliquer à l’iFrame                                  |
|TechnologyId                  |Technologie associée                                                                      |
|SubjectId                     |Objet associé                                                                         |
|Source                        |Nom complet de la catégorie/sous-catégorie                                                  |
|StatusTagId                   |Balise d’état associée                                                                      |
|StatusNote                    |Remarques sur le contenu affiché aux administrateurs.                                           |

### <a name="caching"></a>Mise en cache
La version actuelle du volet Visionneuse utilise une version mise en cache des fichiers manifeste pendant 24 heures. Au bout de 24 heures, le premier utilisateur qui a atteint le site webpart prend les performances pour actualiser le cache en téléchargeant les manifestes à partir de l’CDN source et en fusionnant ces informations avec les technologies et playlists masquées, ainsi que la fusion de sous-catégories, de playlists et de ressources personnalisées. Sinon, le partie Web De l’administrateur télécharge toujours le contenu à partir des manifestes et les fusionne et met à jour le cache.  En d’autres termes, l’administrateur peut forcer une mise à jour du cache à tout moment en chargeant le partie Web De l’administrateur, c’est-à-dire en allant sur la page Administration.

## <a name="content-pack-guidelines"></a>Instructions relatives au pack de contenu
La fonctionnalité pack de contenu déverrouille les scénarios suivants :
- Possibilité pour les partenaires de redistribuer du contenu d’apprentissage personnalisé à valeur ajoutée personnalisé personnalisé adapté à l’environnement des clients
- Capacité pour les organisations avec une équipe de formation forte et un support informatique à créer du contenu d’apprentissage personnalisé dirigé vers leurs propres systèmes internes et gouvernance
- Possibilité pour Microsoft de fournir des parcours d’apprentissage supplémentaires à l’avenir que les clients peuvent choisir

Cet ensemble de documentation actuel est intentionnellement ciblé pour les partenaires en raison de la complexité de la fonctionnalité. L’équipe de service travaille activement pour mieux prendre en charge et activer les scénarios #2, à l’avenir. 

### <a name="how-content-packs-work"></a>Fonctionnement des packs de contenu
Microsoft utilise GitHub pages en tant que source réseau de distribution de contenu (CDN) pour ses fichiers manifestes et images. Nous avons un dossier de documents à la racine de notre référentiel GitHub qui inclut des sous-dossiers pour chaque version des fichiers manifeste. À l’intérieur de chaque dossier se trouve trois fichiers manifeste, ainsi qu’un dossier d’images pour stocker toutes les images de catégorie, de sous-catégorie et de playlist. 

Il est important que vous maintenez la même structure de gestion des versions que Microsoft si vous choisissez d’étendre la solution de parcours d’apprentissage avec votre propre pack de contenu. Votre point de terminaison CDN ne doit pas inclure le dossier de version, car la version de manifeste que le partie Web Part prend en charge y est intégré et est automatiquement ajouté à l’URL CDN’url. Nous vous laisserons évidemment le temps de créer de nouvelles instances de vos fichiers manifeste chaque fois que nous les réviserons.

![Screenshot shows sample structure.](media/cg-part-json-folder.png) 

Pour plus d’informations sur l’utilisation GitHub pages comme source CDN’aide, consultez la documentation d’aide suivante [https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages](https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages) :

La solution de Microsoft rend les informations sur les biens ouvertes au public, car il n’existe aucune sécurité quant aux personnes ayant accès à ces fichiers. Nous pensons qu’il devrait y avoir une couche gratuite de contenu pour un consommateur, qui dit que si vous avez besoin d’un mur de salaire pour tout ou partie de votre contenu, vous devrez implémenter cela différemment dans les limites techniques de la solution et l’utilisation de pages GitHub n’est en aucun cas une exigence. Tout CDN fournisseur que vous souhaitez utiliser est correct si vous conservez la structure de numéro de version que nous avons décrite. Comme indiqué précédemment, la version de la structure de manifeste que le partie Web Part prend en charge est intégré au code et est automatiquement ajouté à l CDN URL. 

### <a name="content-pack-integration-guidance"></a>Conseils sur l’intégration des packs de contenu 
Les composants Web Parts d’administrateur et de visionneuse ont été étendus pour permettre au consommateur de configurer des points de terminaison CDN supplémentaires dans son client, ce qui permettra ensuite au composant Web Part de visionneuse de sélectionner les CDN dont il doit sourcer les données qu’il affiche. 

Cadrage des touches à garder à l’esprit pour cette fonctionnalité : 
- Ceci est applicable en premier lieu pour les scénarios de redistribution des partenaires , où la configuration de la sélection manuelle est trop fastidieuse 
- Les packs de contenu personnalisés sont une fonctionnalité avancée qui ne doit être utilisée que par les partenaires ayant de l’expérience en matière d’administration de contenu web. Les sources de contenu non fiables peuvent introduire du contenu non sécurisé dans votre site. Vous devez ajouter uniquement les sources de confiance.

> **IMPORTANT** Avant d’ajouter un pack de contenu personnalisé, vous devez avoir Microsoft 365 parcours d’apprentissage 3.0 ou ultérieur. Pour obtenir des informations sur la mise en service Microsoft 365 parcours d’apprentissage, voir [Provision Microsoft 365 learning pathways](./custom_provision.md).

### <a name="content-whitelisting"></a>Liste blanche de contenu
En tant que partenaire, il est de votre responsabilité d’aider vos clients à s’assurer que votre contenu est sur liste blanche dans leur environnement. Nous vous suggérons de créer un scénario de test dans leur environnement pour vérifier que votre contenu peut être iFrame’d dans une page SharePoint à l’intérieur de leur pare-feu. Suivez les pages Créer SharePoint pour obtenir des instructions sur les [playlists personnalisées](./custom_createnewpage.md) pour confirmer que c’est le cas.

### <a name="add-a-content-pack-to-learning-pathways"></a>Ajouter un pack de contenu aux parcours d’apprentissage
Une fois que vous avez créé le JSON et défini votre CDN, vous pouvez ajouter le Contact Pack au parcours d’apprentissage. 

1. Dans la **page** d’accueil du site du parcours d’apprentissage, pointez sur **Accueil,** puis cliquez sur **Administration du parcours d’apprentissage.** 
2. Dans la page **Administration,** cliquez sur **... Ajoutez le Pack de** contenu dans le coin supérieur droit de la page.
3. Cliquez sur Pack de contenu personnalisé, puis entrez le nom du pack de contenu, puis spécifiez le CDN où se trouvent les fichiers JSON.

   ![Écran dans lequel vous entrez le nom et les chemins d’accès.](media/cg-part-addconpack.png)

4. Cliquez sur **Enregistrer**. Le contenu de votre pack de contenu personnalisé doit maintenant apparaître dans la page Administration. Voici un exemple. 

   ![Exemple de page d’administration.](media/cg-part-addconpackex.png)

### <a name="filter-to-the-content-pack-in-the-web-part"></a>Filtrer vers le pack de contenu dans le partie Web Part
Avec les parcours d’apprentissage, vous pouvez ajouter le volet Web Des parcours d’apprentissage à une page, filtrer le partie Web Pour pointer vers la source du pack de contenu personnalisé, puis filtrer le partie Web Dans la catégorie, la sous-catégorie, la playlist et le bien que vous souhaitez. 

1. À partir du site du parcours d’apprentissage, cliquez **sur Nouveau,** puis **sur Page.**
2. Cliquez **sur Vide,** puis **créez une page.**
3. Nommez la page. 
4. Cliquez **sur + Ajouter une nouvelle section** sur le côté gauche de la page.
5. Cliquez en haut du milieu de la nouvelle section, puis ajoutez le Microsoft 365 web du parcours **+** **d’apprentissage.**
6. Cliquez sur le volet Web, puis sur **l’icône** Modifier.
7. Dans la **zone Sélectionner la source** d’apprentissage, sélectionnez votre pack de contenu personnalisé, puis filtrez le contenu en sélectionnant le contenu de votre choix. L’exemple suivant illustre le filtre de la sélection d’un élément Web Part à partir d’un pack de contenu personnalisé.

   ![Capture d’écran d’un exemple de partie Web Part filtrée sur une playlist à partir d’un pack de contenu personnalisé.](media/cg-part-conpackfilter.png)