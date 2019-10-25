---
author: pkrebs
ms.author: pkrebs
title: Gérer les mises à jour de contenu des chemins d’apprentissage
ms.date: 10/20/2019
description: Gérer les mises à jour de contenu des chemins d’apprentissage
ms.openlocfilehash: 7a8b348f1a19af669e4e87396de966cf916c93da
ms.sourcegitcommit: 1ec8bc253850e9dd52eebf609033856e76d3e908
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726768"
---
# <a name="how-learning-content-updates-are-applied"></a>Application des mises à jour du contenu d’apprentissage
Le catalogue des chemins d’apprentissage Microsoft 365 est automatiquement mis à jour trimestriellement. Le contenu du catalogue, qui est un ensemble de métadonnées JSON, est stocké dans un cache global au sein du client d’une organisation. Le cache global est automatiquement mis à jour lorsqu’un administrateur de la collection de sites d’apprentissage ou le propriétaire ouvre la page d’administration des chemins d’apprentissage. Pour plus d’informations, consultez la rubrique Managing content updates. 

## <a name="access-the-learning-pathways-administration-page"></a>Accéder à la page d’administration des voies d’apprentissage

La page d’administration des voies d’apprentissage est le point de contrôle central pour l’administration du composant WebPart des chemins d’apprentissage Microsoft 365. Seuls les administrateurs ont la possibilité d’ouvrir la page d’administration à partir de l’élément de menu **Accueil** de SharePoint.  

### <a name="to-access-the-learning-pathways-administration-page"></a>Pour accéder à la page d’administration des voies d’apprentissage
- À partir de la page d’accueil des chemins d’apprentissage Microsoft 365, cliquez sur le menu **Accueil** , puis sur **administration des chemins d’apprentissage**. Lorsqu’un administrateur charge la page d’administration, le cache global est mis à jour et le contenu mis à jour est désormais disponible pour les chemins d’apprentissage des utilisateurs au sein de l’organisation. 

## <a name="what-if-theres-content-in-the-updates-you-want-to-hide"></a>Qu’en est-il si le contenu des mises à jour que vous souhaitez masquer ?
Vérifiez la liste des mises à jour de contenu [Manage content updates](custom_contentupdatesmanage.md). Si le contenu que vous souhaitez masquer aux utilisateurs, vous pouvez le masquer par sous-catégorie ou par liste de lecture. Vous pouvez également masquer le contenu par technologie. Pour obtenir des instructions sur le masquage du contenu, consultez l’une des rubriques suivantes : 

- [Gérer les mises à jour de contenu](custom_hideshowsub.md)
- [Gérer les mises à jour de contenu](custom_hideshowplaylists.md)
- [Gérer les mises à jour de contenu](custom_hideshowtech.md)