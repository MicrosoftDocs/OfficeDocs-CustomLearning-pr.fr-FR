---
author: pkrebs
ms.author: pkrebs
title: Options de configuration pour le parcours d'apprentissage multilingue
ms.date: 07/6/2020
description: Options de configuration pour le parcours d'apprentissage multilingue
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 1384885adc1d7119658bf968e18e8859c784ef37
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999310"
---
# <a name="setup-options-for-multilingual-learning-pathways"></a>Options de configuration pour le parcours d'apprentissage multilingue
Avec la publication de fonctionnalités multilingues pour les sites de communication SharePoint Online, le parcours d'apprentissage offre désormais une prise en charge de plusieurs langues. Vous pouvez configurer les parcours d'apprentissage de différentes manières pour répondre aux besoins de votre organisation. Pour vous aider à choisir le meilleur chemin d'accès pour votre organisation, nous avons présenté les options de configuration. 

## <a name="new-install-scenarios"></a>Nouveaux scénarios d'installation
Les « nouveaux scénarios d'installation » expliquent les options d'installation d'une nouvelle instance du parcours d'apprentissage à l'aide du service d'approvisionnement SharePoint, désormais disponible dans le look book SharePoint.

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>Scénario 1 : nous n'avons pas installé de parcours d'apprentissage et avons besoin d'une prise en charge multilingue des parcours d'apprentissage 
Si vous n'avez pas installé de parcours d'apprentissage et en avez besoin de plusieurs langues, vous pouvez utiliser le service d'approvisionnement SharePoint pour installer une nouvelle solution de parcours d'apprentissage avec prise en charge de neuf langues. L'anglais est la langue par défaut et ne peut pas être modifié. 
- Pour mettre en service une nouvelle solution de parcours d'apprentissage avec l'anglais comme langue par défaut pour le site, voir Mettre en service une nouvelle solution de parcours [d'apprentissage.](custom_provision_ml.md)

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>Scénario 2 : nous avons installé le parcours d'apprentissage, mais nous ne l'utilisons pas actuellement et/ou n'avons pas effectué de personnalisation sur le site ou les playlists 
Si vous avez installé le parcours d'apprentissage, mais que vous ne l'utilisez pas activement, ou si vous n'avez pas effectué de personnalisations sur le site ou les playlists, vous pouvez utiliser le service d'approvisionnement SharePoint pour installer une nouvelle solution avec la prise en charge de neuf langues. L'anglais est la langue par défaut et ne peut pas être modifié. 
- Pour mettre en service une nouvelle solution de parcours d'apprentissage avec l'anglais comme langue par défaut pour le site, voir Mettre en service une nouvelle solution de parcours [d'apprentissage.](custom_provision_ml.md)

### <a name="scenario-3-we-havent-installed-learning-pathways-and-dont-need-multilingual-support"></a>Scénario 3 : nous n'avons pas installé le parcours d'apprentissage et n'avons pas besoin d'une prise en charge multilingue 
Si vous n'avez pas installé le parcours d'apprentissage et que vous n'avez pas besoin d'une prise en charge multilingue, vous pouvez l'installer à partir du service d'approvisionnement SharePoint. L'anglais sera la langue par défaut. Après l'installation, vous devez désactiver la prise en charge multilingue. 
- Pour mettre en service une nouvelle solution de parcours d'apprentissage sans prise en charge multilingue, voir Mettre en service une nouvelle solution de [parcours d'apprentissage.](custom_provision_ml.md)

## <a name="update-learning-pathways-with-a-web-part-upload-scenarios"></a>Mettre à jour les scénarios de parcours d'apprentissage (avec un téléchargement de partie Web)
Si une version existante du parcours d'apprentissage est installée, vous pouvez télécharger le volet Web du parcours d'apprentissage dans le catalogue d'applications SharePoint pour activer la prise en charge multilingue. 

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-dont-need-multilingual-support"></a>Scénario 1 : nous devons mettre à niveau une version existante du parcours d'apprentissage, mais nous n'avons pas besoin d'une prise en charge multilingue
Vous pouvez mettre à jour le parcours d'apprentissage version 4.0 sans prise en charge multilingue. Avec la mise à jour, vous obtenez quelques nouvelles fonctionnalités, y compris un sélecteur d'image pour les sélections personnalisées et les sous-catégories. 

- Pour mettre à jour une solution de parcours d'apprentissage existante sans prise en charge multilingue, voir Mettre à jour les parcours d'apprentissage pour la prise en charge [multilingue.](custom_update_ml.md) Le processus de mise à niveau pour aucune prise en charge multilingue est identique à celui d'une prise en charge multilingue, mais avec moins d'étapes. 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>Scénario 2 : nous devons mettre à niveau la prise en charge multilingue et la langue par défaut de la collection de sites est notre langue par défaut
Le parcours d'apprentissage version 4.O prendra en charge les pages multilingues dans votre collection de sites. En plus de la prise en charge multilingue, vous obtenez quelques nouvelles fonctionnalités, notamment un sélecteur d'image pour les sélections personnalisées et les sous-catégories. 
- Pour mettre à jour une prise en charge multilingue d'un site de parcours d'apprentissage existant, voir Mettre à jour les parcours d'apprentissage pour la prise en charge [multilingue.](custom_update_ml.md) 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>Mettre à jour les parcours d'apprentissage pour la prise en charge multilingue avec l'installation manuelle 
L'exemple suivant décrit les scénarios de mise à jour d'une instance existante de la solution de parcours d'apprentissage vers la version multilingue version 4.0 en installant manuellement le volet Web Du parcours d'apprentissage. 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>Scénario 1 : nous avons besoin d'une prise en charge multilingue et la langue par défaut de la collection de sites n'est pas notre langue par défaut , pas de contenu personnalisé 
Le parcours d'apprentissage version 4.0 prendra en charge ce scénario. Toutefois, ce scénario suppose que vous n'avez pas de contenu ou de playlists personnalisés sur le site existant. Pour ce scénario, vous pouvez créer un nouveau site de communication SharePoint Online avec votre langue par défaut, télécharger le site Web Part, puis configurer manuellement les parcours d'apprentissage avec un script PowerShell. 
- Pour configurer le parcours d'apprentissage pour la prise en charge multilingue avec votre langue par défaut, voir Installation manuelle du parcours d'apprentissage pour la prise en charge [multilingue.](custom_manualsetup_ml.md)

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>Scénario 2 : nous avons besoin d'une prise en charge multilingue et la langue par défaut de la collection de sites n'est pas notre langue par défaut , et nous avons du contenu personnalisé. 
Pour ce scénario, vous pouvez créer un nouveau site de communication SharePoint Online avec votre langue par défaut, télécharger le site Web Part, puis configurer manuellement les parcours d'apprentissage avec un script PowerShell. 

Après avoir rétabli votre site de parcours d'apprentissage en suivant les étapes ci-dessus, vous devez déplacer le contenu de votre liste **CustomPlaylists** et de votre liste **CustomAssets.** Vous pouvez également, si vous le souhaitez, déplacer les pages personnalisées réelles qui constitueront vos ressources personnalisées si elles existent dans le site de parcours d'apprentissage existant, et votre intention est de les supprimer. La tâche peut être difficile, car pour tous les éléments de la liste **CustomPlaylists,** l'ID de l'élément de liste dans la liste **CustomAssets** est insérez dans le champ JSONData de chaque élément de liste de playlist. Par conséquent, le simple déplacement du contenu de la liste **CustomPlaylists** d'un site à l'autre ne sera pas suffisant. En outre, la **liste CustomAssets** contient l'URL absolue de la page de la bien personnalisée dans le champ JSONData de l'élément de liste. Si les ressources ne sont pas déplacées et que le site n'est pas renommé (en modifiant l'URL absolue sur la page de la bien), **CustomAssets** peut rester. Mais vous devrez corriger manuellement les entrées. Étant donné la complexité de ce type de migration, nous vous suggérons de faire appel à l'un de nos partenaires de parcours d'apprentissage pour vous aider à effectuer cette transition.
- Pour configurer le parcours d'apprentissage pour la prise en charge multilingue avec votre langue par défaut, voir Installation manuelle du parcours d'apprentissage pour la prise en charge [multilingue.](custom_manualsetup_ml.md)

