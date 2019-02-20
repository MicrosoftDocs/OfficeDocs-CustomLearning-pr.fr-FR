---
author: pkrebs
ms.author: pkrebs
title: Liaison aux ressources de formation personnalisées
ms.date: 02/15/2019
description: Comment établir un lien vers des ressources de formation personnalisées
ms.openlocfilehash: cdde37f370663ca50241833a15e8411921b45a1b
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/19/2019
ms.locfileid: "30103729"
---
# <a name="link-to-custom-learning-content"></a>Lien vers du contenu de formation personnalisé

Avec l'apprentissage personnalisé, il existe deux façons de créer un lien vers du contenu:

- Lien vers la page qui héberge le composant WebPart filtré pour le contenu que vous souhaitez afficher. 
- Lien direct vers une instance du composant WebPart

## <a name="link-to-a-page"></a>Lien vers une page

Si vous avez créé de nouvelles pages et des expériences d'apprentissage avec le composant WebPart formation personnalisée, vous pouvez créer un lien vers la page avec le composant WebPart configuré pour afficher le contenu que vous souhaitez afficher. Dans la section précédente, nous avons abordé le mode d'affichage des sélections Excel sur une page. Vous pouvez maintenant modifier la page d'accueil pour créer un lien vers la page. 

1. À partir de la page d'accueil, cliquez sur **modifier**.
2. Cliquez sur **modifier les détails** dans l'une des vignettes de page d'accueil. Dans cet exemple, nous modifions **** les vignettes de playlists recommandées.
3. Sous **lien**, cliquez sur **modifier**.

![CG-linktopage. png](media/cg-linktopage.png)

4. Cliquez sur **site**, puis sur **pages du site**, cliquez sur la page vers laquelle vous souhaitez créer le lien, puis cliquez sur **ouvrir**. Dans cet exemple, nous créons un lien vers la page **Create-Your-Own-experience. aspx** abordée dans la section précédente.
5. Fermez le volet des propriétés du héros, cliquez sur **publier**, puis testez le lien. 

## <a name="link-to-the-custom-learning-web-part"></a>Lien vers le composant WebPart formation personnalisée
L'apprentissage personnalisé vous offre la possibilité de créer un lien vers une instance du composant WebPart indépendamment de la page qui contient le composant WebPart. Vous pouvez partager le lien copié ou le lier à d'autres pages. Le lien copié, lorsque l'utilisateur clique dessus, affiche l'instance du composant WebPart de formation personnalisée dans la page CustomLLearningViewer. aspx. Examinons un exemple. 

1. À partir de la page d'accueil, cliquez sur **formation Office 365**.
2. Cliquez sur **Microsoft teams**, puis sur **Introduction à Microsoft teams**.
3. Cliquez sur l'icône **copier** .

![CG-linktowebpart. png](media/cg-linktowebpart.png)

4. Dans le menu formation personnalisée, cliquez sur Accueil.
5. Collez l'URL copiée dans la barre d'adresses du navigateur, puis appuyez sur entrée. 

Comme le montre l'illustration suivante, le lien mène à la page CustomLearningViewer. aspx et affiche le contenu en fonction des paramètres du lien copié. 

![CG-linktowebpartviewer. png](media/cg-linktowebpartviewer.png)

