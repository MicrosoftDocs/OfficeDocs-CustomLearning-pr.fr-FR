---
author: pkrebs
ms.author: pkrebs
title: Créer des pages SharePoint pour les playlists
ms.date: 02/10/2019
description: Créer des pages SharePoint pour les playlists
ms.service: sharepoint-online
ms.openlocfilehash: 40c249fbd5b0fdaefd555f23bf20ac23240ea954
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999085"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="1f2ef-103">Créer des pages SharePoint pour des playlists personnalisées</span><span class="sxs-lookup"><span data-stu-id="1f2ef-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="1f2ef-104">L'une des fonctionnalités uniques du parcours d'apprentissage est la possibilité de créer des playlists assemblées à partir des ressources de Microsoft et des ressources SharePoint que vous créez.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="1f2ef-105">Dans cet exemple, nous allons créer une page SharePoint avant de créer une playlist.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="1f2ef-106">La possibilité de créer des playlists à partir de pages SharePoint offre de nombreuses opportunités de créer des pages à l'aide des composants Web Parts disponibles auprès de Microsoft ou de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="1f2ef-107">Par exemple, une playlist peut inclure une page SharePoint avec des vidéos incorporées à partir de YouTube, un formulaire créé à partir de formulaires Office 365 ou un rapport Power BI incorporé.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="1f2ef-108">Dans cet exemple, nous allons vous montrer comment créer une page avec le partie Web Part Embed et le volet Texte.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="1f2ef-109">Créer une page SharePoint pour une playlist personnalisée</span><span class="sxs-lookup"><span data-stu-id="1f2ef-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="1f2ef-110">Cliquez sur l'icône **d'engrenage** SharePoint, puis cliquez **sur Ajouter une page.**</span><span class="sxs-lookup"><span data-stu-id="1f2ef-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="1f2ef-111">Cliquez **sur Ajouter une nouvelle section (+)** sur le côté gauche de la page, puis cliquez sur **Deux** colonnes pour la mise en page de section.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="1f2ef-112">Dans la colonne de gauche, cliquez sur +, puis cliquez sur le **volet Incorporer.**</span><span class="sxs-lookup"><span data-stu-id="1f2ef-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="1f2ef-113">Dans la colonne de droite, cliquez sur +, puis sur **le** volet Texte.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="1f2ef-114">Votre page doit ressembler à ceci.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-114">Your page should look like this.</span></span>

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="1f2ef-116">Ajouter une vidéo et du texte à partir de YouTube</span><span class="sxs-lookup"><span data-stu-id="1f2ef-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="1f2ef-117">Dans votre navigateur, allez sur YouTube.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="1f2ef-118">Pour cet exemple, recherchez « Qu'est-ce qu'Office 365 – Meilleures applications de productivité de Microsoft ».</span><span class="sxs-lookup"><span data-stu-id="1f2ef-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="1f2ef-119">Cliquez sur la vidéo pour la lire, puis suspendez-la, puis cliquez dessus avec le bouton droit.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="1f2ef-120">Cliquez **sur Copier le code incorporer,** puis revenir à la page SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="1f2ef-121">Cliquez **sur Ajouter du code d'incorporation** dans le volet Web Incorporer, puis ajoutez le code de la vidéo YouTube. </span><span class="sxs-lookup"><span data-stu-id="1f2ef-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="1f2ef-122">Revenir à la page YouTube et copier le **texte Description** de la vidéo.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="1f2ef-123">Revenir à la page SharePoint, sélectionnez **le** volet Texte, puis copiez le texte de la vidéo YouTube.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="1f2ef-124">Sélectionnez **l'icône Modifier le** site Web Part dans la zone Titre de la page SharePoint, puis nommez la page « Introduction à la sélection personnalisée ».</span><span class="sxs-lookup"><span data-stu-id="1f2ef-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="1f2ef-125">Pour **la disposition,** **sélectionnez Plain,** puis fermez le volet des propriétés **de la région** de titre.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="1f2ef-126">La page doit maintenant ressembler à ce qui suit.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="1f2ef-128">Publier la page</span><span class="sxs-lookup"><span data-stu-id="1f2ef-128">Publish the page</span></span>

- <span data-ttu-id="1f2ef-129">Sélectionnez **le bouton** Publier.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-129">Select the **Publish** button.</span></span> <span data-ttu-id="1f2ef-130">Vous êtes maintenant prêt à ajouter cette page SharePoint à votre playlist personnalisée.</span><span class="sxs-lookup"><span data-stu-id="1f2ef-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 