---
author: pkrebs
ms.author: pkrebs
title: Option de configuration pour les voies de formation
ms.date: 07/16/2020
description: Option de configuration pour les voies de formation
ms.service: sharepoint online
ms.openlocfilehash: 3246434cf450a17d324ce5b5afed5b9d7a4339ec
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233966"
---
# <a name="setup-options-for-multilingual-learning-pathways"></a>Options de configuration pour les voies de formation multilingues
Avec la publication de fonctionnalités multilingues pour les sites de communications SharePoint Online, les voies de formation prennent désormais en charge plusieurs langues. Vous pouvez configurer les voies de formation de différentes manières afin de répondre aux besoins de votre organisation. Pour vous aider à choisir le meilleur chemin pour votre organisation, nous avons décrit les options de configuration. 

## <a name="new-install-scenarios"></a>Nouveaux scénarios d’installation
Les « nouveaux scénarios d’installation » expliquent les options permettant d’installer une nouvelle instance des voies de formation à l’aide du service de carnet d’adresses Microsoft 365. 

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>Scénario 1 : nous n’avons pas installé les voies de formation et besoin de chemins d’apprentissage en prise en charge multilingue 
Si vous n’avez pas installé les voies de formation et que vous en avez besoin dans plusieurs langues, vous pouvez utiliser le service de carnet d’adresses Microsoft 365 pour installer une nouvelle solution de voies de formation avec prise en charge de neuf langues. L’anglais sera la langue par défaut et ne peut pas être modifié. 
- Pour mettre en service une nouvelle solution de voies d’apprentissage avec l’anglais comme langue par défaut pour le site, reportez-vous à la rubrique mise en [service d’une nouvelle solution de voies d’apprentissage](custom_provision.md).

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>Scénario 2 : nous avons installé les voies de formation, mais ne les utilisez pas et/ou n’avons effectué aucune personnalisation au site ou aux playlists. 
Si vous avez installé les voies de formation mais que vous ne les utilisez pas activement, ou si vous n’avez apporté aucune personnalisation au site ou aux sélections, vous pouvez utiliser le service de carnet d’adresses Microsoft 365 pour installer une nouvelle solution avec prise en charge de neuf langues. L’anglais sera la langue par défaut et ne peut pas être modifié. 
- Pour mettre en service une nouvelle solution de voies d’apprentissage avec l’anglais comme langue par défaut pour le site, reportez-vous à la rubrique mise en [service d’une nouvelle solution de voies d’apprentissage](custom_provision.md).

### <a name="scenario-3-we-havent-installed-learning-pathways-and-dont-need-multilingual-support"></a>Scénario 3 : nous n’avons pas installé les voies de formation et n’avez pas besoin de prise en charge multilingue 
Si vous n’avez pas installé les voies de formation et que vous n’avez pas besoin de la prise en charge multilingue, vous pouvez l’installer à partir du service de carnet d’adresses Microsoft 365. L’anglais sera la langue par défaut. Après l’installation, vous devez désactiver la prise en charge multilingue. 
- Pour mettre en service une nouvelle solution de voies d’apprentissage sans prise en charge multilingue, consultez la rubrique mise en [service d’une nouvelle solution de voies d’apprentissage](custom_provision.md).

## <a name="update-learning-pathways-with-a-web-part-upload-scenarios"></a>Mettre à jour les chemins d’apprentissage (avec un téléchargement de composants WebPart)
Si vous disposez d’une version existante des chemins d’apprentissage installés, vous pouvez télécharger le composant WebPart voies d’apprentissage dans le catalogue d’applications SharePoint pour activer la prise en charge multilingue. 

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-dont-need-multilingual-support"></a>Scénario 1 : nous devons mettre à niveau une version existante des chemins d’apprentissage, mais n’avez pas besoin de la prise en charge multilingue
Vous pouvez mettre à jour les chemins d’apprentissage version 4,0 sans prise en charge multilingue. Avec la mise à jour, vous disposez de deux nouvelles fonctionnalités, notamment un sélecteur d’image pour les listes de lecture et sous-catégories personnalisées. 

- Pour mettre à jour une solution de voies d’apprentissage existantes sans prise en charge multilingue, consultez la rubrique [mise à jour des chemins d’apprentissage pour la prise en charge multilingue](custom_update.md). Le processus de mise à niveau sans prise en charge multilingue est le même que pour la prise en charge multilingue, mais avec moins d’étapes. 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>Scénario 2 : nous devons effectuer une mise à niveau vers la prise en charge multilingue et la langue par défaut de la collection de sites est notre langue par défaut
Voies d’apprentissage version 4. O prend en charge les pages multilingues dans votre collection de sites. En plus de la prise en charge multilingue, vous disposez de deux nouvelles fonctionnalités, notamment un sélecteur d’image pour les listes et les sous-catégories personnalisées. 
- Pour mettre à jour une prise en charge multilingue des voies d’apprentissage existantes, consultez la rubrique [mise à jour des chemins d’apprentissage pour la prise en charge multilingue](custom_update.md). 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>Mettre à jour les voies de formation pour la prise en charge multilingue avec installation manuelle 
Le code suivant décrit les scénarios de mise à jour d’une instance existante de la solution de voies d’apprentissage vers la version 4,0 multilingue en installant manuellement le composant WebPart voies d’apprentissage. 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>Scénario 1 : nous avons besoin d’une prise en charge multilingue et la langue par défaut de la collection de sites n’est pas notre langue par défaut, aucun contenu personnalisé 
Les voies d’apprentissage version 4,0 prendront en charge ce scénario. Toutefois, ce scénario suppose que vous n’avez pas de contenu ou de sélections personnalisés sur le site existant. Pour ce scénario, vous pouvez créer un site de communication SharePoint Online avec votre langue par défaut, Télécharger le composant WebPart, puis configurer manuellement les voies de formation avec un script PowerShell. 
- Pour configurer les voies de formation pour la prise en charge multilingue avec votre langue par défaut, consultez la rubrique [installation manuelle des voies de formation pour la prise en charge multilingue](custom_manualsetup.md).

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>Scénario 2 : nous avons besoin d’une prise en charge multilingue et la langue par défaut de la collection de sites n’est pas notre langue par défaut – plus nous avons un contenu personnalisé 
Pour ce scénario, vous pouvez créer un site de communication SharePoint Online avec votre langue par défaut, Télécharger le composant WebPart, puis configurer manuellement les voies de formation avec un script PowerShell. 

Une fois que vous avez rétablissez votre site de voies d’apprentissage en suivant les étapes ci-dessus, vous devrez déplacer le contenu de votre liste **CustomPlaylists** et de votre liste **CustomAssets** . Vous pouvez également déplacer les pages personnalisées réelles qui composent vos biens personnalisés si elles résident sur le site des voies d’apprentissage existantes, et que votre intention est de la supprimer. La tâche peut être difficile, car pour tous les éléments de la liste **CustomPlaylists** , l’ID de l’élément de liste dans la liste **CustomAssets** est enfoui dans le champ JSONData de chaque élément de liste de playlist. Par conséquent, le simple fait de délimiter le contenu de la liste **CustomPlaylists** d’un site à l’autre ne suffira pas. De plus, la liste **CustomAssets** contient l’URL absolue de la page de l’élément personnalisé dans le champ JSONData de l’élément de liste. Si les ressources ne sont pas déplacées et que le site n’est pas renommé (ce qui modifie l’URL absolue vers la page de l’élément), **CustomAssets** peut être conservé. Toutefois, vous devrez corriger manuellement les entrées. Étant donné la complexité de ce type de migration, nous vous conseillons d’avoir inscrit l’un de nos partenaires de parcours de formation pour vous aider à effectuer cette transition.
- Pour configurer les voies de formation pour la prise en charge multilingue avec votre langue par défaut, consultez la rubrique [installation manuelle des voies de formation pour la prise en charge multilingue](custom_manualsetup.md).