---
author: karuanag
ms.author: karuanag
title: Installation du composant WebPart de la solution d'apprentissage personnalisée
ms.date: 02/10/2019
description: Instructions d'installation du composant WebPart de la solution d'apprentissage personnalisée
ms.openlocfilehash: 53229e5b1b8175b06d888091963d1a9f2f0bd361
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989685"
---
# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="80430-103">Installation du composant WebPart de la solution d'apprentissage personnalisée</span><span class="sxs-lookup"><span data-stu-id="80430-103">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="80430-104">Conditions préalables pour une installation à l'échelle du client</span><span class="sxs-lookup"><span data-stu-id="80430-104">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="80430-p101">Pour installer le composant WebPart de formation personnalisée pour l'ensemble de votre client, vous devez disposer des autorisations d'administration d'Office 365.  Si vous ne disposez pas de ces autorisations, vous pouvez travailler avec votre administrateur Office 365 ou installer le composant WebPart pour une collection de sites individuelle.</span><span class="sxs-lookup"><span data-stu-id="80430-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="80430-107">Vous ou votre administrateur Office 365 devez avoir configuré et configuré un [catalogue d'applications](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) à l'échelle du client ou un catalogue d'applications de [collection de sites](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)pour recevoir le composant WebPart.</span><span class="sxs-lookup"><span data-stu-id="80430-107">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="80430-p102">Nous prenons en charge SharePoint Online uniquement. Le composant WebPart n'est pas pris en charge pour l'installation sur une version de SharePoint sur site.</span><span class="sxs-lookup"><span data-stu-id="80430-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="80430-110">Ajouter le composant WebPart formation personnalisée à votre client</span><span class="sxs-lookup"><span data-stu-id="80430-110">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="80430-p103">Téléchargez le composant WebPart formation personnalisée et enregistrez-le sur votre lecteur local.  Ce fichier est nommé «MS-Custom-Learning. sppkg».  Ne modifiez pas le nom ou le suffixe du fichier.</span><span class="sxs-lookup"><span data-stu-id="80430-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="80430-114">Accédez au [portail d'administration Office 365](https://admin.microsoft.com/AdminPortal/Home#/homepage) pour votre client.</span><span class="sxs-lookup"><span data-stu-id="80430-114">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="80430-p104">Dans le volet de navigation de gauche, sélectionnez centres d'administration, SharePoint. Cette opération s'ouvre dans un nouvel onglet., dans le centre d'administration SharePoint, sélectionnez applications, catalogue d'applications, applications pour SharePoint</span><span class="sxs-lookup"><span data-stu-id="80430-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="80430-117">Sélectionnez Télécharger le composant WebPart et sélectionnez le fichier «MS-Custom-Learning. sppkg» que vous avez téléchargé</span><span class="sxs-lookup"><span data-stu-id="80430-117">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="80430-118">Pour cette installation à l'échelle du client, cochez la case en regard de «mettre cette solution à disposition de tous les» dans l'organisation.</span><span class="sxs-lookup"><span data-stu-id="80430-118">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  
 
> [!NOTE]
> <span data-ttu-id="80430-p105">Une fois le composant WebPart installé, vous le trouverez dans votre galerie de WebPart dans SharePoint Online.  **Dans la Galerie, le composant WebPart est nommé «Microsoft Learning»**</span><span class="sxs-lookup"><span data-stu-id="80430-p105">Once the webpart is installed you will find it in your webpart gallery in SharePoint Online.  **In the gallery the webpart is named "Microsoft Learning"**</span></span>

![Déployer la solution](media/trustapp_sm.png)


## <a name="add-the-microsoft-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="80430-122">Ajouter le composant WebPart formation Microsoft à une page SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="80430-122">Add the Microsoft Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="80430-p106">Une fois que l'apprentissage personnalisé est installé dans votre client, vous pouvez ajouter le composant WebPart à une page SharePoint. La formation Office 365 et Windows 10 est disponible pour votre site.</span><span class="sxs-lookup"><span data-stu-id="80430-p106">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do Office 365 and Windows 10 training is available to your site.</span></span>

1. <span data-ttu-id="80430-125">Ajoutez le composant WebPart formation personnalisée dans une mise en forme de colonne à pleine chasse:</span><span class="sxs-lookup"><span data-stu-id="80430-125">Add the Custom Learning webpart in a full width column layout:</span></span>

![Mise en page SharePoint](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="80430-p107">Dans la page SharePoint, sélectionnez Ajouter une section, puis sélectionnez colonne pleine chasse.  L'invite suivante apparaît:</span><span class="sxs-lookup"><span data-stu-id="80430-p107">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="80430-p108">Sélectionnez Microsoft Learning.  Vous devez maintenant voir les éléments suivants:</span><span class="sxs-lookup"><span data-stu-id="80430-p108">Select Microsoft Learning.  You should now see the following:</span></span> 

![Composant WebPart formation personnalisée](media/clo365addwebpart.png)

 <span data-ttu-id="80430-133">Vous pouvez maintenant cliquer sur les vignettes pour explorer le contenu par défaut inclus dans la solution.</span><span class="sxs-lookup"><span data-stu-id="80430-133">You can now click on the tiles to explore the default content included in the solution.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="80430-134">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="80430-134">Next Steps</span></span>
- <span data-ttu-id="80430-135">Explorez le [contenu par défaut](webpartcontent.md) inclus dans le composant WebPart.</span><span class="sxs-lookup"><span data-stu-id="80430-135">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="80430-136">[Personnaliser](customization.md) l'expérience de formation pour votre organisation.</span><span class="sxs-lookup"><span data-stu-id="80430-136">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="80430-137">Encouragez l' [adoption](driveadoption.md) de votre solution de formation.</span><span class="sxs-lookup"><span data-stu-id="80430-137">[Drive adoption](driveadoption.md) of your training solution.</span></span>

