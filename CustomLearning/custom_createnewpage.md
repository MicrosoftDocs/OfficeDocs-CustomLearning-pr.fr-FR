---
author: pkrebs
ms.author: pkrebs
title: Créer des pages SharePoint pour les playlists
ms.date: 02/10/2019
description: Créer des pages SharePoint pour les playlists
ms.openlocfilehash: c2de66a0746260e8f6539656ad70052b209c54ba
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055492"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a>Créer des pages SharePoint pour les playlists personnalisées

L'une des fonctionnalités uniques de la formation personnalisée est la possibilité de créer des sélections assemblées à partir de biens provenant de Microsoft et de ressources SharePoint que vous créez. Dans cet exemple, nous allons créer une page SharePoint avant de créer une playlist. La possibilité de créer des sélections à partir de pages SharePoint permet de créer des pages à l'aide des composants WebPart disponibles auprès de Microsoft ou de votre organisation. Par exemple, une playlist peut inclure une page SharePoint avec des vidéos incorporées provenant de YouTube ou un formulaire créé à partir de formulaires Office 365, ou un rapport intégré Power BI. Dans cet exemple, nous allons vous montrer comment créer une page avec le composant WebPart embed et le composant WebPart texte.  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a>Créer une page SharePoint pour une liste de lecture personnalisée

1. Cliquez sur l'icône de l' **engrenage** SharePoint, puis cliquez sur **Ajouter une page**.
2. Cliquez sur **Ajouter une nouvelle section (+)** sur le côté gauche de la page, puis cliquez sur **deux colonnes** pour la disposition de la section.
3. Dans la colonne de gauche, cliquez sur +, puis sur **** le composant WebPart incorporer. 
4. Dans la colonne de droite, cliquez sur +, puis sur le composant WebPart **texte** . Votre page doit ressembler à ce qui suit.

![CG-pagenewstart. png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a>Ajouter une vidéo et du texte à partir de YouTube

1. Dans votre navigateur, accédez à YouTube. Pour cet exemple, recherchez «qu'est-ce que Office 365 – meilleures applications de productivité de Microsoft».
2. Cliquez sur la vidéo pour la lire, puis suspendez-la, puis cliquez dessus avec le bouton droit. 
3. Cliquez sur **copier le code incorporé**, puis revenez à la page SharePoint. 
4. Cliquez sur **Ajouter un code incorporé** dans le composant WebPart **embed** , puis ajoutez le code à partir de la vidéo YouTube.
5. ReVenez à la page YouTube et copiez le texte de **Description** de la vidéo. 
6. ReVenez à la page SharePoint, sélectionnez le composant WebPart **texte** , puis copiez le texte à partir de la vidéo YouTube.
7. Sélectionnez l'icône **modifier le composant WebPart** dans la zone de titre de la page SharePoint, puis nommez la page «introduction de la playlist personnalisée». 
8. Pour **disposition**, sélectionnez **standard**, puis fermer la zone de propriétés **région de titre** . La page doit maintenant ressembler à ce qui suit. 

![CG-pagenewfinish. png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a>Publier la page

- Sélectionnez le bouton **publier** . Vous êtes maintenant prêt à ajouter cette page SharePoint à votre playlist personnalisée. 