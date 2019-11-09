---
author: pkrebs
ms.author: pkrebs
title: Modèles d’intégration des partenaires
ms.date: 3/9/2019
description: Modèles d’intégration des partenaires
ms.openlocfilehash: 0d52210c600e14fc9f224fbe6f91645fe4045c45
ms.sourcegitcommit: 6a17a7ab6d28349654520f2c28d08c480e3c7b47
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/08/2019
ms.locfileid: "38076018"
---
# <a name="partner-integration-models"></a>Modèles d’intégration des partenaires
S’il n’est pas possible de compléter le contenu des chemins d’apprentissage Microsoft 365 directement à partir du service de mise en service SharePoint Online, il existe plusieurs modèles d’intégration que les partenaires peuvent utiliser pour créer des services à valeur ajoutée alignés. offres. Les modèles d’intégration des partenaires ci-dessus sont présentés par ordre croissant de complexité et de niveaux d’investissement. Nos conseils sont donc de développer votre expertise et votre diplôme sur des niveaux plus avancés en fonction de vos modèles d’entreprise.

![CG-part-intmodel. png](media/cg-part-intmodel.png) 

## <a name="how-should-i-get-started"></a>Comment dois-je commencer ? 
Pour commencer, voici quelques bonnes pratiques à suivre.     

### <a name="1-begin-with-building-expertise-as-an-enabler"></a>1. Commencez par la création d’une expertise en tant qu’activateur. 
Vous pouvez contribuer à un pourcentage de votre base de clients immédiatement en activant son portail de formation sur les voies d’apprentissage et en effectuant une organisée de contenu Microsoft ciblée. Pour obtenir des instructions sur la mise en service des voies https://docs.microsoft.com/en-us/office365/customlearning/custom_provisiond’apprentissage, voir.  

### <a name="2-then-extend-your-services-as-an-integrator"></a>2. étendez vos services en tant qu’intégrateur.
Effectuer un retour d’automatisation sur l’analyse des investissements, en fonction de la quantité de votre contenu et/ou de vos besoins d’intégration de services. Par exemple, il n’est pas judicieux de prendre les coûts de développement et d’exploitation en ce qui concerne nos directives d’intégration de contenu si vous pouvez rapidement créer manuellement une sélection personnalisée ciblée pointant vers votre contenu payant ou référencer vos services.

### <a name="3-when-the-return-on-investment-makes-sense--consider-redistribution"></a>3. lorsque le retour sur investissement est pertinent, envisagez de redistribuer 
Lorsque le retour sur investissement est pertinent, envisagez de redistribuer (ou d’utiliser les partenaires de voies d’apprentissage associés) pour créer des solutions reconditionnées. Celles-ci sont basées sur les modèles SharePoint et l’infrastructure pratique qui fournit des solutions pour extraire les sites personnalisés, puis les déployer dans les environnements client 

## <a name="partner-provided-content-integration-guidelines"></a>Instructions d’intégration de contenu fournies par un partenaire
Le contenu des chemins d’apprentissage Microsoft 365 est piloté par un ensemble de fichiers JSON qui agissent comme des manifestes de contenu pour votre package de formation. Il existe trois fichiers : Metadata. JSON, playlists. JSON et biens. JSON. Ces fichiers doivent être structurés pour correspondre aux modèles que le composant WebPart reconnaît puis héberger à partir d’un réseau de distribution de contenu (CDN) pour autoriser le composant WebPart à le charger. Microsoft fournira des modèles de démarrage de ces fichiers pour vous aider à démarrer.  

**Clause d’exclusion de responsabilité :** la structure de fichiers JSON est susceptible d’être modifiée en fonction du travail de la solution à venir. Le programme d’adoption du partenaire des chemins d’apprentissage Microsoft 365 (EAP) est informé des modifications imminentes de cette nature. Ainsi que les instructions de compatibilité et/ou de transition des clients. 

### <a name="download-the-microsoft-365-learning-pathways-solution"></a>Téléchargement de la solution des chemins d’apprentissage Microsoft 365
Vous pouvez télécharger la solution des chemins d’apprentissage Microsoft 365, ainsi que les fichiers JSON, à partir du référentiel GitHub : https://github.com/pnp/custom-learning-office-365. Notez que, pour l’instant, Microsoft ne prend pas en charge la requête de tirage GitHub sur la solution. Toutefois, vous pouvez utiliser les fichiers GitHub comme point de départ pour créer votre propre Pack de contenu personnalisé. 

### <a name="metadatajson-structure"></a>Structure Metadata. JSON
Vous pouvez considérer ce fichier comme le cerveau des menus et de la structure. Elle contient toutes les structures de navigation, ainsi que les listes de sélection des données dans les deux autres fichiers. 


|              Nom        |                     Description                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|**Technologie**              |Le contenu est balisé et peut être masqué en fonction de la technologie qu’il a affectée.                 |  
|&nbsp;&nbsp;Réf                |GUID représentant la technologie                                                           |  
|&nbsp;&nbsp;Nom              |Nom d’affichage de la technologie                                                             |
|&nbsp;&nbsp;*Objets []*     |Tableau de sujets qui constituent un sous-ensemble de la technologie                                   | 
|&nbsp;&nbsp;&nbsp;&nbsp;Réf    |GUID représentant l’objet                                                              |
|&nbsp;&nbsp;&nbsp;&nbsp;Nom  |Nom d’affichage de l’objet                                                                |
|**Catégories []**             |Les catégories informent la navigation du composant WebPart. Chaque catégorie représente un niveau supérieur de la navigation.                                                                                                                 |
|&nbsp;&nbsp;Réf                |GUID représentant la catégorie/sous-catégorie                                                 |
|&nbsp;&nbsp;Nom              |Nom d’affichage de la catégorie/sous-catégorie                                                  |
|&nbsp;&nbsp;Photo             |URL de l’image qui doit être affichée dans l’expérience utilisateur (par rapport à la base du CDN)            |
|&nbsp;&nbsp;TechnologyId      |GUID de la technologie à laquelle ce contenu est lié (facultatif – chaîne vide)            |
|&nbsp;&nbsp;SubjectId         |GUID de l’objet auquel ce contenu est lié (facultatif – chaîne vide)               |
|&nbsp;&nbsp;Journal            |À partir d’une baie source, elle n’est pas spécifiquement utilisée dans une expérience utilisateur autre que les données personnalisées ajoutées par l’utilisateur est marquée comme « client » et la zone d’administration d’expérience utilisateur n’autorise pas la modification des éléments qui ne sont pas marqués « client ».                           |
|&nbsp;&nbsp;*Sous-catégories []*|Les sous-catégories sont fondamentalement le niveau de navigation du niveau 2 vers le bas. La structure est identique à celle d’une catégorie qui vient d’être imbriquée.          |
|**Audiences []**             |Lorsque plusieurs audiences associées à une catégorie/sous-catégorie sont indiquées, un sélecteur est disponible pour afficher les audiences disponibles. |         
|&nbsp;&nbsp;Réf                |GUID de l’audience                                                                       |  
|&nbsp;&nbsp;Nom              |Nom d’affichage de l’audience                                                               |       
|**Sources []**               |Tableau de chaînes qui balise le contenu avec sa source, non spécifiquement utilisées dans l’expérience utilisateur, à l’exception des données personnalisées ajoutées par l’utilisateur, sont marquées comme « locataire » et la zone admin UX n’autorise pas la modification des éléments qui ne sont pas marqués « client ».                                                   |  
|**Levels []**               |Lorsque plusieurs niveaux de sélection associés à une catégorie/sous-catégorie sont marqués, un sélecteur est disponible pour afficher les niveaux disponibles.             |  
|&nbsp;&nbsp;Réf                |GUID du niveau                                                                          |  
|&nbsp;&nbsp;Nom              |Nom d’affichage du niveau                                                                  | 
|**StatusTag [ ]**           |La balise d’état permet d’identifier le contenu présentant différents statuts qui seront exposés dans l’expérience utilisateur. Certains de ces indicateurs seront affichés pour le consommateur et d’autres seulement pour l’administrateur.                                                   |  
|&nbsp;&nbsp;Réf                |GUID du StatugTag                                                                      |  
|&nbsp;&nbsp;Nom              |Nom d’affichage du StatusTag                                                              | 
|**Télémétrie []**            |                                                                                           |  
|&nbsp;&nbsp;AppInsightsKey    |GUID de la clé Insights de l’application que vous avez configuré pour effectuer le suivi du chargement du composant WebPart Visionneuse. Le suivi peut être désactivé par un administrateur pour l’ensemble du client, mais les informations envoyées sont des utilisateurs anonymes avec l’ID de client. Pour plus d’informations, reportez-vous à cette section.https://github.com/pnp/custom-learning-office-365#disabling-telemetry-collection               |  
|**Version**                   |Les informations de version sont utilisées par la solution pour indiquer aux administrateurs que le composant WebPart a été mis à jour et permettre au composant WebPart de mettre à jour automatiquement le contenu personnalisé vers la dernière version du manifeste si des modifications importantes ont été apportées.         | 
|&nbsp;&nbsp;Manifeste          |Version du manifeste                                               |
|&nbsp;&nbsp;ManifestMinWebPart|Version minimale du composant WebPart qui fonctionne avec la version du manifeste             |
|&nbsp;&nbsp;CurrentWebPart    |URL de l’image qui doit être affichée dans l’expérience utilisateur (par rapport à la base du CDN)            |
|&nbsp;&nbsp;Reversion           |URL du référentiel où se trouvent les instructions de mise à jour du composant WebPart.                    |
|**Packs de contenu**             |À ce stade, les packs de contenu pour les CDN supplémentaires ne sont pas pris en charge. Les packs de contenu permettent à Microsoft de suggérer d’autres solutions Microsoft créées qui peuvent être configurées via le service de mise en service qui exploite M365LP pour fournir du contenu et qui se trouvent dans et de lui-même CDN personnalisé.       | 
|&nbsp;&nbsp;Réf                |GUID du Pack de contenu/CDN                                                              |
|&nbsp;&nbsp;Nom              |Nom d’affichage du CDN                                                                   |
|&nbsp;&nbsp;Description       |Description à afficher dans l’interface utilisateur pour l’ajout d’un pack de contenu                               |
|&nbsp;&nbsp;Photo             |Image à afficher dans l’interface utilisateur pour l’ajout d’un pack de contenu                                     |
|&nbsp;&nbsp;ProvisionURL      |L’URL du package de service de mise en service pour créer la collection de sites du Pack de contenu  |
|&nbsp;&nbsp;CDNbase           |L’URL de base pour les manifestes du Pack de contenu                                       |
|AssetOrigins                  |Tableau d’origine de l’URL utilisé dans le fichier immobilisations. JSON décrit plus loin. Si l’URL d’origine la prend en charge, un message post est envoyé à help_getClientHeight. Une réponse dans la propriété Data de : « help_getClientHeight = {height of content} » (par exemple, « help_getClientHeight = 5769 ») permettra de redimensionner l’iFrame à la hauteur appropriée du contenu de cadres.         |

### <a name="playlistsjson-structure"></a>Structure playlists. JSON
playlists. JSON : le manifeste de sélections est un tableau d’objets qui décrivent les métadonnées d’une sélection et les biens inclus dans la sélection.

|              Nom        |                     Description                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|ID                            |GUID représentant la playlist                                                             |  
|Titre                         |Nom d’affichage de la playlist                                                               |
|Image                         |URL relative (du CDN) vers une image pour visualiser la playlist                              |                      
|LevelId                       |Niveau associé                                                                           |
|AudienceId                   |Audience associée                                                                        |
|TechnologyId                 |Technologie associée                                                                      |
|SubjectId                    |Nom d’affichage de la catégorie/sous-catégorie                                                  |
|Source                        |À partir du tableau source, il n’est pas utilisé spécifiquement dans une expérience utilisateur autre que les données personnalisées ajoutées par l’utilisateur est marqué comme « client » et la zone admin UX n’autorise pas la modification des éléments qui ne sont pas marqués « client ».                                              |
|CatId                         |ID de catégorie ou de sous-catégorie qui représente le conteneur dans lequel la playlist doit s’afficher. Actuellement, le manifeste ne prend pas en charge la sélection d’une catégorie ou sous-catégorie comme conteneur si elle comporte également des enfants de sous-catégorie.        |
|Description                   |Une description A été montrée pour chaque liste de lecture dans l’expérience utilisateur                                           |
|StatusTagId                   |Balise d’État associée                                                                      |
|StatusNote                    |Remarques sur le contenu affiché aux administrateurs                                            |
|*Ressources []*                        |Un tableau de GUID pour les éléments qui font partie de cette playlist, dans l’ordre d’affichage.        |         

### <a name="assetjson-structure"></a>Structure Asset. JSON
playlists. JSON : le manifeste de sélections est un tableau d’objets qui décrivent les métadonnées d’une sélection et les biens inclus dans la sélection.

|              Nom        |                     Description                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|ID                            |GUID représentant la playlist                                                             |  
|Titre                         |Nom d’affichage de la playlist                                                               |
|Description                   |---                                                                                           |                      
|URL                           |URL source de l’élément à appliquer à l’iFrame                                  |
|TechnologyId                  |Technologie associée                                                                      |
|SubjectId                     |Objet associé                                                                         |
|Source                        |Nom d’affichage de la catégorie/sous-catégorie                                                  |
|StatusTagId                   |Balise d’État associée                                                                      |
|StatusNote                    |Remarques sur le contenu affiché aux administrateurs.                                           |

### <a name="caching"></a>Mise en cache
La version actuelle du composant WebPart Visionneuse utilise une version mise en cache des fichiers manifeste pendant 24 heures. Au bout de 24 heures, le premier utilisateur qui a atteint le composant WebPart a atteint le gain de performances pour actualiser le cache en téléchargeant les manifestes à partir du CDN source et fusionne ces informations avec les technologies et les playlists masquées, ainsi que la fusion dans des sous-catégories personnalisées, playlists et biens. Le composant WebPart admin télécharge toujours le contenu des manifestes et les fusionne et met à jour le cache.  En d’autres termes, l’administrateur peut forcer une mise à jour du cache à tout moment en chargeant le composant WebPart d’administration, puis en accédant à la page d’administration.

## <a name="content-pack-guidelines"></a>Instructions pour le Pack de contenu
La fonctionnalité du Pack de contenu déverrouille les scénarios suivants :
- Possibilité pour les partenaires de redistribuer un contenu d’apprentissage personnalisé à valeur ajoutée personnalisé adapté à l’environnement des clients
- Possibilité pour les organisations disposant d’une équipe de formation solide et d’un support informatique de créer un contenu d’apprentissage personnalisé dirigé vers ses systèmes internes et sa gouvernance
- Possibilité pour Microsoft de fournir des voies de formation supplémentaires à l’avenir auxquelles les clients peuvent s’abonner

Ce jeu de documentation actuel est intentionnellement ciblé pour les partenaires en raison de la complexité de la fonctionnalité. L’équipe de service travaille activement à mieux prendre en charge et à activer le scénario #2, à l’avenir. 

### <a name="how-content-packs-work"></a>Fonctionnement des modules de contenu
Microsoft utilise des pages GitHub en tant que source de réseau de distribution de contenu (CDN) pour ses fichiers manifeste et ses images. Nous disposons d’un dossier docs à la racine de notre référentiel GitHub qui inclut des sous-dossiers pour chaque version des fichiers manifeste. Dans chaque dossier, il existe trois fichiers Manifest, ainsi qu’un dossier images pour stocker toutes les images de catégorie, de sous-catégorie et de playlist. 

Il est important que vous mainteniez la même structure de contrôle de version que celle que Microsoft doit utiliser pour étendre la solution de voies d’apprentissage avec votre propre Pack de contenu. Votre point de terminaison CDN ne doit pas inclure le dossier version, car la version de manifeste prise en charge par le composant WebPart est intégrée automatiquement à l’URL du CDN. Nous allons évidemment vous laisser le temps de créer de nouvelles instances de vos fichiers manifeste à tout moment.

![CG-part-JSON-Folder. png](media/cg-part-json-folder.png) 

Pour plus d’informations sur l’utilisation des pages GitHub comme source de CDN, consultez la documentation d' [https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages](https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages)aide suivante :.

La solution de Microsoft rend les informations relatives aux ressources ouvertes au public, car il n’existe aucune sécurité pour les personnes qui ont accès à ces fichiers. Nous pensons qu’il doit y avoir une couche de contenu gratuite pour un consommateur, ceci dit, si vous avez besoin de payer le mur pour tout ou partie de votre contenu, vous devrez l’implémenter différemment dans les limites techniques de la solution et l’utilisation de pages GitHub n’est pas une moyenne s une exigence. Tout fournisseur de CDN que vous souhaitez utiliser est parfait si vous conservez la structure de numérotation des versions que nous avons décrite. Comme indiqué précédemment, la version de la structure de manifeste prise en charge par le composant WebPart est intégrée dans le code et est automatiquement ajoutée à l’URL du CDN. 

### <a name="content-pack-integration-guidance"></a>Guide d’intégration du Pack de contenu 
Les composants WebPart de l’administrateur et de la visionneuse ont été étendus pour permettre à l’utilisateur de configurer des points de terminaison CDN supplémentaires dans leur client, ce qui permettra au composant WebPart Visionneuse de sélectionner le CDN qui doit sourceiser les données qu’ils affichent. 

Trames clés à garder à l’esprit pour cette fonctionnalité : 
- Il s’agit du principal applicable aux scénarios de redistribution des partenaires : la configuration de la playlist manuelle est trop lourde 
- Les packs de contenu personnalisés sont une fonctionnalité avancée qui doit être utilisé uniquement par les partenaires ayant une expérience d’administration de contenu Web. Les sources de contenu non fiables peuvent introduire du contenu non sécurisé dans votre site. Vous devez uniquement ajouter des sources approuvées.

> **Important** Avant d’ajouter un pack de contenu personnalisé, vous devez disposer des chemins d’apprentissage Microsoft 365 3,0 ou version ultérieure. Pour informataion sur la mise en service des chemins d’apprentissage Microsoft 365, voir [provisionner les chemins d’apprentissage microsoft 365](https://docs.microsoft.com/en-us/office365/customlearning/custom_provision).

### <a name="content-whitelisting"></a>Liste d’interliste de contenu
En tant que partenaire, il est de votre responsabilité pour aider vos clients à s’assurer que votre contenu est la liste d’autorisation dans leur environnement. Nous vous suggérons de créer un scénario de test dans son environnement afin de vérifier que votre contenu peut être iFrame dans une page SharePoint à l’intérieur de son pare-feu. Suivez les instructions [créer des pages SharePoint pour les playlists personnalisées](https://docs.microsoft.com/en-us/office365/customlearning/custom_createnewpage) pour confirmer que c’est le cas.

### <a name="add-a-content-pack-to-learning-pathways"></a>Ajouter un pack de contenu aux voies d’apprentissage
Une fois que vous avez modifié le JSON et défini votre CDN, vous pouvez ajouter le Pack de contacts aux voies d’apprentissage. 

1. Sur la page d' **Accueil** du site des voies d’apprentissage, pointez sur **Accueil** , puis cliquez sur **administration des chemins d’apprentissage**. 
2. Dans la page **administration** , cliquez sur **... Ajoutez le Pack de contenu** dans le coin supérieur droit de la page.
3. Cliquez sur Pack de contenu personnalisé, puis entrez un nom pour le Pack de contenu, puis spécifiez le CDN dans lequel se trouvent les fichiers JSON.

![CG-part-addconpack. png](media/cg-part-addconpack.png)

4. Cliquez sur **Enregistrer**. Le contenu de votre pack de contenu personnalisé doit maintenant apparaître dans la page Administration. Voici un exemple. 

![CG-part-addconpackex. png](media/cg-part-addconpackex.png)

### <a name="filter-to-the-content-pack-in-the-web-part"></a>Filtrer sur le Pack de contenu dans le composant WebPart
Les voies de formation vous permettent d’ajouter le composant WebPart voies d’apprentissage à une page, de filtrer le composant WebPart de sorte qu’il pointe vers la source du Pack de contenu personnalisé, puis de filtrer le composant WebPart sur la catégorie, la sous-catégorie, la liste de choix et l’élément de votre choix. 

1. Sur le site des voies d’apprentissage, cliquez sur **nouveau**, puis sur **page**.
2. Cliquez sur **vide**, puis sur **créer une page**.
3. Donnez un nom à la page. 
4. Cliquez sur **+ Ajouter une nouvelle section** sur le côté gauche de la page.
5. Cliquez **+** en haut au milieu de la nouvelle section, puis ajoutez le composant WebPart des **chemins d’apprentissage Microsoft 365** .
6. Cliquez sur le composant WebPart, puis cliquez sur l’icône **modifier** .
7. Dans la zone **Sélectionnez la source d’apprentissage** , sélectionnez votre pack de contenu personnalisé, puis filtrez le composant WebPart pour le contenu de votre choix. Vous trouverez ci-dessous un exemple de composant WebPart filtré sur une sélection à partir d’un pack de contenu personnalisé.

![CG-part-conpackfilter. png](media/cg-part-conpackfilter.png)  




