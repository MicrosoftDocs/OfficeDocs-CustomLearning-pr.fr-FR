---
author: pkrebs
ms.author: pkrebs
title: Créer des SharePoint pour les playlists
ms.date: 02/10/2019
description: Créer des SharePoint pour les playlists
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: ce4a204b3072469840b6f3fa8f93d9e78833b181
ms.sourcegitcommit: 956ab22dd8ce23ee1779f1a01d34b434243c3cb1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/11/2021
ms.locfileid: "52310658"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a>Créer SharePoint pages personnalisées pour les playlists personnalisées

L’une des fonctionnalités uniques du parcours d’apprentissage est la possibilité de créer des playlists assemblées à partir des ressources de Microsoft et des ressources SharePoint que vous créez. Dans cet exemple, nous allons créer une page SharePoint avant de créer une playlist. La possibilité de créer des playlists à partir SharePoint pages offre de nombreuses opportunités de créer des pages à l’aide des composants Web Parts disponibles auprès de Microsoft ou de votre organisation. Par exemple, une playlist peut inclure une page SharePoint avec des vidéos incorporées à partir de YouTube, un formulaire créé à partir de Office 365 Forms ou un rapport Power BI incorporé. Dans cet exemple, nous allons vous montrer comment créer une page avec le partie Web Part Embed et le volet Texte.  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a>Créer une page SharePoint de lecture personnalisée

1. Cliquez sur l SharePoint **icône Engrenage,** puis cliquez **sur Ajouter une page.**
2. Cliquez **sur Ajouter une nouvelle section (+)** sur le côté gauche de la page, puis cliquez sur **Deux** colonnes pour la mise en page de section.
3. Dans la colonne de gauche, cliquez sur +, puis cliquez sur le **volet Incorporer.** 
4. Dans la colonne de droite, cliquez sur +, puis sur **le** volet Texte. Votre page doit ressembler à ceci.

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a>Ajouter une vidéo et du texte à partir de YouTube

1. Dans votre navigateur, allez sur YouTube. Pour cet exemple, recherchez « What is Office 365 - Microsoft’s best productivity apps ».
2. Cliquez sur la vidéo pour la lire, puis suspendez-la, puis cliquez dessus avec le bouton droit. 
3. Cliquez **sur Copier le code** incorporer, puis revenir à la page SharePoint page. 
4. Cliquez **sur Ajouter du code d’incorporation** dans le volet Web Incorporer, puis ajoutez le code de la vidéo YouTube. 
5. Revenir à la page YouTube et copier le **texte Description** de la vidéo. 
6. Revenir à la page SharePoint, sélectionnez le volet **Texte,** puis copiez le texte de la vidéo YouTube.
7. Sélectionnez **l’icône Modifier le** site Web Part dans la zone Titre de la page SharePoint, puis nommez la page « Introduction à la sélection personnalisée ». 
8. Pour **la disposition,** **sélectionnez Plain,** puis fermez le volet des propriétés **de la région** de titre. La page doit maintenant ressembler à ce qui suit. 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a>Publier la page

- Sélectionnez **le bouton** Publier. Vous êtes maintenant prêt à ajouter cette page SharePoint à votre playlist personnalisée. 