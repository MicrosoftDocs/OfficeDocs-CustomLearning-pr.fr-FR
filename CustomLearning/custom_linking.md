---
author: pkrebs
ms.author: pkrebs
title: Liaison aux ressources des chemins d’apprentissage Microsoft 365
ms.date: 02/15/2019
description: Comment établir un lien vers les éléments des chemins d’apprentissage Microsoft 365
ms.openlocfilehash: cc8ba80e1c658fabb44e3df405c9293ec763ab3d
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/21/2019
ms.locfileid: "34327275"
---
# <a name="link-to-learning-pathways-content"></a><span data-ttu-id="372be-103">Lien vers le contenu des voies d’apprentissage</span><span class="sxs-lookup"><span data-stu-id="372be-103">Link to learning pathways content</span></span>

<span data-ttu-id="372be-104">Avec les voies de formation, il existe deux façons de créer un lien vers du contenu :</span><span class="sxs-lookup"><span data-stu-id="372be-104">With learning pathways, there are two ways to link to content:</span></span>

- <span data-ttu-id="372be-105">Lien vers la page qui héberge le composant WebPart filtré pour le contenu que vous souhaitez afficher</span><span class="sxs-lookup"><span data-stu-id="372be-105">Link to the page that host the Web part filtered for the content you want to display</span></span> 
- <span data-ttu-id="372be-106">Lien direct vers une instance du composant WebPart</span><span class="sxs-lookup"><span data-stu-id="372be-106">Link directly to an instance of the Web part</span></span>

## <a name="link-to-a-page"></a><span data-ttu-id="372be-107">Lien vers une page</span><span class="sxs-lookup"><span data-stu-id="372be-107">Link to a page</span></span>

<span data-ttu-id="372be-108">Si vous avez créé de nouvelles pages et des expériences d’apprentissage avec le composant WebPart des chemins d’apprentissage Microsoft 365, vous pouvez créer un lien vers la page avec le composant WebPart configuré pour afficher le contenu que vous souhaitez afficher.</span><span class="sxs-lookup"><span data-stu-id="372be-108">If you've created new pages and learning experiences with the Microsoft 365 learning pathways web part, you can link to the page with the Web part configured to show the content you want to display.</span></span> <span data-ttu-id="372be-109">Dans la section précédente, nous avons abordé le mode d’affichage des sélections Excel sur une page.</span><span class="sxs-lookup"><span data-stu-id="372be-109">In the previous section, we covered how to display Excel playlists on a page.</span></span> <span data-ttu-id="372be-110">Vous pouvez maintenant modifier la page d’accueil pour créer un lien vers la page.</span><span class="sxs-lookup"><span data-stu-id="372be-110">You could now edit the Home page to link to the page.</span></span> 

1. <span data-ttu-id="372be-111">À partir de la page d’accueil, cliquez sur **modifier**.</span><span class="sxs-lookup"><span data-stu-id="372be-111">From the Home page, click **Edit**.</span></span>
2. <span data-ttu-id="372be-112">Cliquez sur **modifier les détails** dans l’une des vignettes de page d’accueil.</span><span class="sxs-lookup"><span data-stu-id="372be-112">Click **Edit details** in one of the Home page tiles.</span></span> <span data-ttu-id="372be-113">Dans cet exemple, nous modifions les vignettes de **playlists recommandées** .</span><span class="sxs-lookup"><span data-stu-id="372be-113">In this example, we edit the **Recommended playlists** tiles.</span></span>
3. <span data-ttu-id="372be-114">Sous **lien**, cliquez sur **modifier**.</span><span class="sxs-lookup"><span data-stu-id="372be-114">Under **Link**, click **Change**.</span></span>

![CG-linktopage. png](media/cg-linktopage.png)

4. <span data-ttu-id="372be-116">Cliquez sur **site**, puis sur **pages du site**, cliquez sur la page vers laquelle vous souhaitez créer le lien, puis cliquez sur **ouvrir**.</span><span class="sxs-lookup"><span data-stu-id="372be-116">Click **Site**, then **Site Pages**, click the page you want to link to, and then click **Open**.</span></span> <span data-ttu-id="372be-117">Dans cet exemple, nous créons un lien vers la page **Create-Your-Own-experience. aspx** abordée dans la section précédente.</span><span class="sxs-lookup"><span data-stu-id="372be-117">In this example, we link to the **Create-your-own-experience.aspx** page covered in the previous section.</span></span>
5. <span data-ttu-id="372be-118">Fermez le volet des propriétés du héros, cliquez sur **publier**, puis testez le lien.</span><span class="sxs-lookup"><span data-stu-id="372be-118">Close the Hero properties pane, click **Publish**, and then test the link.</span></span> 

## <a name="link-to-the-microsoft-365-learning-pathways-web-part"></a><span data-ttu-id="372be-119">Lien vers le composant WebPart des chemins d’apprentissage Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="372be-119">Link to the Microsoft 365 learning pathways web part</span></span>
<span data-ttu-id="372be-120">Les voies pédagogiques vous permettent d’accéder à une instance du composant WebPart, indépendamment de la page qui contient le composant WebPart, à l’administrateur ou à un utilisateur final.</span><span class="sxs-lookup"><span data-stu-id="372be-120">Learning pathways gives you, the administrator, or an end-user, the ability to link to an instance of the Web part independent of the page that contains the Web part.</span></span> <span data-ttu-id="372be-121">Vous pouvez partager le lien copié ou le lier à d’autres pages.</span><span class="sxs-lookup"><span data-stu-id="372be-121">You can share the copied link or link to it from other pages.</span></span> <span data-ttu-id="372be-122">Le lien copié, lorsque vous cliquez dessus, présente l’instance du composant WebPart des chemins d’apprentissage Microsoft 365 dans la page CustomLLearningViewer. aspx.</span><span class="sxs-lookup"><span data-stu-id="372be-122">The copied link, when clicked, shows the Microsoft 365 learning pathways web part instance in the CustomLLearningViewer.aspx page.</span></span> <span data-ttu-id="372be-123">Prenons un exemple.</span><span class="sxs-lookup"><span data-stu-id="372be-123">Let's look at an example.</span></span> 

1. <span data-ttu-id="372be-124">À partir de la page d’accueil, cliquez sur **formation Microsoft365**.</span><span class="sxs-lookup"><span data-stu-id="372be-124">From the Home page, click **Microsoft365 training**.</span></span>
2. <span data-ttu-id="372be-125">Cliquez sur **Microsoft teams**, puis sur **Introduction à Microsoft teams**.</span><span class="sxs-lookup"><span data-stu-id="372be-125">Click **Microsoft Teams**, and then click **Intro to Microsoft Teams**.</span></span>
3. <span data-ttu-id="372be-126">Cliquez sur l’icône **copier** .</span><span class="sxs-lookup"><span data-stu-id="372be-126">Click the **Copy** icon.</span></span>

![CG-linktowebpart. png](media/cg-linktowebpart.png)

4. <span data-ttu-id="372be-128">Cliquez sur Accueil dans le menu site des chemins d’apprentissage Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="372be-128">Click Home from the Microsoft 365 learning pathways site menu.</span></span>
5. <span data-ttu-id="372be-129">Collez l’URL copiée dans la barre d’adresses du navigateur, puis appuyez sur entrée.</span><span class="sxs-lookup"><span data-stu-id="372be-129">Paste the copied URL in the address bar of the browser and press ENTER.</span></span> 

<span data-ttu-id="372be-130">Comme le montre l’illustration suivante, le lien mène à la page CustomLearningViewer. aspx et affiche le contenu en fonction des paramètres du lien copié.</span><span class="sxs-lookup"><span data-stu-id="372be-130">As shown in the following illustration, the link goes to the CustomLearningViewer.aspx page and displays the content based on the parameters in the copied link.</span></span> 

![CG-linktowebpartviewer. png](media/cg-linktowebpartviewer.png)

