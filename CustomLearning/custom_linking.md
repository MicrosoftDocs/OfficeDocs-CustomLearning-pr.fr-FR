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
# <a name="link-to-custom-learning-content"></a><span data-ttu-id="9f0cc-103">Lien vers du contenu de formation personnalisé</span><span class="sxs-lookup"><span data-stu-id="9f0cc-103">Link to Custom Learning content</span></span>

<span data-ttu-id="9f0cc-104">Avec l'apprentissage personnalisé, il existe deux façons de créer un lien vers du contenu:</span><span class="sxs-lookup"><span data-stu-id="9f0cc-104">With Custom Learning, there are two ways to link to content:</span></span>

- <span data-ttu-id="9f0cc-105">Lien vers la page qui héberge le composant WebPart filtré pour le contenu que vous souhaitez afficher.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-105">Link to the page that host the Web part filtered for the content you want to display.</span></span> 
- <span data-ttu-id="9f0cc-106">Lien direct vers une instance du composant WebPart</span><span class="sxs-lookup"><span data-stu-id="9f0cc-106">Link directly to an instance of the Web part</span></span>

## <a name="link-to-a-page"></a><span data-ttu-id="9f0cc-107">Lien vers une page</span><span class="sxs-lookup"><span data-stu-id="9f0cc-107">Link to a page</span></span>

<span data-ttu-id="9f0cc-p101">Si vous avez créé de nouvelles pages et des expériences d'apprentissage avec le composant WebPart formation personnalisée, vous pouvez créer un lien vers la page avec le composant WebPart configuré pour afficher le contenu que vous souhaitez afficher. Dans la section précédente, nous avons abordé le mode d'affichage des sélections Excel sur une page. Vous pouvez maintenant modifier la page d'accueil pour créer un lien vers la page.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-p101">If you've created new pages and learning experiences with the Custom Learning Web part, you can link to the page with the Web part configured to show the content you want to display. In the previous section, we covered how to display Excel playlists on a page. You could now edit the Home page to link to the page.</span></span> 

1. <span data-ttu-id="9f0cc-111">À partir de la page d'accueil, cliquez sur **modifier**.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-111">From the Home page, click **Edit**.</span></span>
2. <span data-ttu-id="9f0cc-p102">Cliquez sur **modifier les détails** dans l'une des vignettes de page d'accueil. Dans cet exemple, nous modifions \*\*\*\* les vignettes de playlists recommandées.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-p102">Click **Edit details** in one of the Home page tiles. In this example, we edit the **Recommended playlists** tiles.</span></span>
3. <span data-ttu-id="9f0cc-114">Sous **lien**, cliquez sur **modifier**.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-114">Under **Link**, click **Change**.</span></span>

![CG-linktopage. png](media/cg-linktopage.png)

4. <span data-ttu-id="9f0cc-p103">Cliquez sur **site**, puis sur **pages du site**, cliquez sur la page vers laquelle vous souhaitez créer le lien, puis cliquez sur **ouvrir**. Dans cet exemple, nous créons un lien vers la page **Create-Your-Own-experience. aspx** abordée dans la section précédente.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-p103">Click **Site**, then **Site Pages**, click the page you want to link to, and then click **Open**. In this example, we link to the **Create-your-own-experience.aspx** page covered in the previous section.</span></span>
5. <span data-ttu-id="9f0cc-118">Fermez le volet des propriétés du héros, cliquez sur **publier**, puis testez le lien.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-118">Close the Hero properties pane, click **Publish**, and then test the link.</span></span> 

## <a name="link-to-the-custom-learning-web-part"></a><span data-ttu-id="9f0cc-119">Lien vers le composant WebPart formation personnalisée</span><span class="sxs-lookup"><span data-stu-id="9f0cc-119">Link to the Custom Learning web part</span></span>
<span data-ttu-id="9f0cc-p104">L'apprentissage personnalisé vous offre la possibilité de créer un lien vers une instance du composant WebPart indépendamment de la page qui contient le composant WebPart. Vous pouvez partager le lien copié ou le lier à d'autres pages. Le lien copié, lorsque l'utilisateur clique dessus, affiche l'instance du composant WebPart de formation personnalisée dans la page CustomLLearningViewer. aspx. Examinons un exemple.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-p104">Custom Learning gives you, the administrator, or an end-user, the ability to link to an instance of the Web part independent of the page that contains the Web part. You can share the copied link or link to it from other pages. The copied link, when clicked, shows the Custom Learning web part instance in the CustomLLearningViewer.aspx page. Let's look at an example.</span></span> 

1. <span data-ttu-id="9f0cc-124">À partir de la page d'accueil, cliquez sur **formation Office 365**.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-124">From the Home page, click **Office 365 training**.</span></span>
2. <span data-ttu-id="9f0cc-125">Cliquez sur **Microsoft teams**, puis sur **Introduction à Microsoft teams**.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-125">Click **Microsoft Teams**, and then click **Intro to Microsoft Teams**.</span></span>
3. <span data-ttu-id="9f0cc-126">Cliquez sur l'icône **copier** .</span><span class="sxs-lookup"><span data-stu-id="9f0cc-126">Click the **Copy** icon.</span></span>

![CG-linktowebpart. png](media/cg-linktowebpart.png)

4. <span data-ttu-id="9f0cc-128">Dans le menu formation personnalisée, cliquez sur Accueil.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-128">Click Home from the Custom Learning menu.</span></span>
5. <span data-ttu-id="9f0cc-129">Collez l'URL copiée dans la barre d'adresses du navigateur, puis appuyez sur entrée.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-129">Paste the copied URL in the address bar of the browser and press ENTER.</span></span> 

<span data-ttu-id="9f0cc-130">Comme le montre l'illustration suivante, le lien mène à la page CustomLearningViewer. aspx et affiche le contenu en fonction des paramètres du lien copié.</span><span class="sxs-lookup"><span data-stu-id="9f0cc-130">As shown in the following illustration, the link goes to the CustomLearningViewer.aspx page and displays the content based on the parameters in the copied link.</span></span> 

![CG-linktowebpartviewer. png](media/cg-linktowebpartviewer.png)

