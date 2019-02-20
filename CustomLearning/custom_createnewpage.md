---
author: pkrebs
ms.author: pkrebs
title: Créer des pages SharePoint pour les playlists
ms.date: 02/10/2019
description: Créer des pages SharePoint pour les playlists
ms.openlocfilehash: c2de66a0746260e8f6539656ad70052b209c54ba
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/19/2019
ms.locfileid: "30103689"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="05275-103">Créer des pages SharePoint pour les playlists personnalisées</span><span class="sxs-lookup"><span data-stu-id="05275-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="05275-p101">L'une des fonctionnalités uniques de la formation personnalisée est la possibilité de créer des sélections assemblées à partir de biens provenant de Microsoft et de ressources SharePoint que vous créez. Dans cet exemple, nous allons créer une page SharePoint avant de créer une playlist. La possibilité de créer des sélections à partir de pages SharePoint permet de créer des pages à l'aide des composants WebPart disponibles auprès de Microsoft ou de votre organisation. Par exemple, une playlist peut inclure une page SharePoint avec des vidéos incorporées provenant de YouTube ou un formulaire créé à partir de formulaires Office 365, ou un rapport intégré Power BI. Dans cet exemple, nous allons vous montrer comment créer une page avec le composant WebPart embed et le composant WebPart texte.</span><span class="sxs-lookup"><span data-stu-id="05275-p101">One of the unique features of Custom Learning is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create. In this example, we’ll create a SharePoint page in advance of creating a playlist. The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization. For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report. In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="05275-109">Créer une page SharePoint pour une liste de lecture personnalisée</span><span class="sxs-lookup"><span data-stu-id="05275-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="05275-110">Cliquez sur l'icône de l' **engrenage** SharePoint, puis cliquez sur **Ajouter une page**.</span><span class="sxs-lookup"><span data-stu-id="05275-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="05275-111">Cliquez sur **Ajouter une nouvelle section (+)** sur le côté gauche de la page, puis cliquez sur **deux colonnes** pour la disposition de la section.</span><span class="sxs-lookup"><span data-stu-id="05275-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="05275-112">Dans la colonne de gauche, cliquez sur +, puis sur \*\*\*\* le composant WebPart incorporer.</span><span class="sxs-lookup"><span data-stu-id="05275-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="05275-p102">Dans la colonne de droite, cliquez sur +, puis sur le composant WebPart **texte** . Votre page doit ressembler à ce qui suit.</span><span class="sxs-lookup"><span data-stu-id="05275-p102">In the right column, click +, and then click the **Text** web part. Your page should look like this.</span></span>

![CG-pagenewstart. png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="05275-116">Ajouter une vidéo et du texte à partir de YouTube</span><span class="sxs-lookup"><span data-stu-id="05275-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="05275-p103">Dans votre navigateur, accédez à YouTube. Pour cet exemple, recherchez «qu'est-ce que Office 365 – meilleures applications de productivité de Microsoft».</span><span class="sxs-lookup"><span data-stu-id="05275-p103">In your browser, go to YouTube. For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="05275-119">Cliquez sur la vidéo pour la lire, puis suspendez-la, puis cliquez dessus avec le bouton droit.</span><span class="sxs-lookup"><span data-stu-id="05275-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="05275-120">Cliquez sur **copier le code incorporé**, puis revenez à la page SharePoint.</span><span class="sxs-lookup"><span data-stu-id="05275-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="05275-121">Cliquez sur **Ajouter un code incorporé** dans le composant WebPart **embed** , puis ajoutez le code à partir de la vidéo YouTube.</span><span class="sxs-lookup"><span data-stu-id="05275-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="05275-122">ReVenez à la page YouTube et copiez le texte de **Description** de la vidéo.</span><span class="sxs-lookup"><span data-stu-id="05275-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="05275-123">ReVenez à la page SharePoint, sélectionnez le composant WebPart **texte** , puis copiez le texte à partir de la vidéo YouTube.</span><span class="sxs-lookup"><span data-stu-id="05275-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="05275-124">Sélectionnez l'icône **modifier le composant WebPart** dans la zone de titre de la page SharePoint, puis nommez la page «introduction de la playlist personnalisée».</span><span class="sxs-lookup"><span data-stu-id="05275-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="05275-p104">Pour **disposition**, sélectionnez **standard**, puis fermer la zone de propriétés **région de titre** . La page doit maintenant ressembler à ce qui suit.</span><span class="sxs-lookup"><span data-stu-id="05275-p104">For **Layout**, select **Plain**, then close **Title Region** properties pane. The page should now look something like the following.</span></span> 

![CG-pagenewfinish. png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="05275-128">Publier la page</span><span class="sxs-lookup"><span data-stu-id="05275-128">Publish the page</span></span>

- <span data-ttu-id="05275-p105">Sélectionnez le bouton **publier** . Vous êtes maintenant prêt à ajouter cette page SharePoint à votre playlist personnalisée.</span><span class="sxs-lookup"><span data-stu-id="05275-p105">Select the **Publish** button. Now you're ready to add this SharePoint page to your custom playlist.</span></span> 