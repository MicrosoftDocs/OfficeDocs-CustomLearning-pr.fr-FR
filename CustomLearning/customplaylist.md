---
author: karuanag
ms.author: karuanag
title: Personnaliser et partager des sélections
ms.date: 02/10/2019
description: Créer des playlists personnalisées à partir d'un contenu existant ou de nouvelles pages SharePoint
ms.openlocfilehash: d330b6e401c9020eb68877bc8a132350811a2f31
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989725"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="9aa4f-103">Personnaliser et partager des sélections</span><span class="sxs-lookup"><span data-stu-id="9aa4f-103">Customize and Share Playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="9aa4f-104">Créer une playlist</span><span class="sxs-lookup"><span data-stu-id="9aa4f-104">Create a Playlist</span></span>

<span data-ttu-id="9aa4f-p101">Une playlist est une sélection de «biens». Une «ressource» est une page SharePoint ou un élément de contenu de formation Microsoft existant. Lorsque vous créez une liste de sélection, vous sélectionnez des biens qui se regroupent pour créer un cursus pour votre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-p101">A playlist is a compliation of "assets". An "asset" is a SharePoint page or existing item of Microsoft training content. When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="9aa4f-p102">L'avantage de l'ajout de pages SharePoint est que vous pouvez créer des pages SharePoint avec une vidéo YouTube ou des vidéos hébergées dans votre organisation. Vous pouvez également créer des pages avec des formulaires ou d'autres contenus Office 365.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-p102">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization. You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="9aa4f-110">Étape 1: créer une page SharePoint pour votre playlist</span><span class="sxs-lookup"><span data-stu-id="9aa4f-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="9aa4f-p103">Dans cet exemple, nous allons d'abord créer une page SharePoint à ajouter à la liste de lecture. Nous allons créer une page avec un composant WebPart de vidéo YouTube et un composant WebPart texte.  Ces instructions supposent que vous utilisez le service SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-p103">In this example, we’ll first create a SharePoint page to add to the playlist. We’ll create a page with a YouTube video web part and Text web part.  These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="9aa4f-114">Créer une page</span><span class="sxs-lookup"><span data-stu-id="9aa4f-114">Create a new page</span></span>
1.  <span data-ttu-id="9aa4f-115">Sélectionnez le menu paramètres > contenu > site Web > nouvelle page de site >.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="9aa4f-116">Dans la zone de titre, tapez utiliser la boîte de commandes teams</span><span class="sxs-lookup"><span data-stu-id="9aa4f-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="9aa4f-117">Sélectionnez la section Ajouter une nouvelle section, puis sélectionnez deux colonnes.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-117">Select the Add a new section, and then select Two Columns.</span></span>

![ajout de deux colonnes](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="9aa4f-119">Dans la zone de gauche, sélectionnez Ajouter un nouveau composant WebPart, puis sélectionnez incorporer.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="9aa4f-120">Dans un navigateur Web, accédez à cette URL https://youtu.be/wYrRCRphrp0 et obtenez le code d'intégration pour la vidéo.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="9aa4f-121">Dans le composant WebPart SharePoint, sélectionnez Ajouter un code incorporé, puis collez-le dans la zone incorporer.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="9aa4f-122">Dans la zone de droite, sélectionnez Ajouter un nouveau composant WebPart, puis texte.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="9aa4f-p104">Dans un navigateur Web, accédez à l'URL suivante https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b : et copiez le bloc try! Instructions de la page et collez-les dans le composant WebPart texte. Votre page doit ressembler à ce qui suit.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-p104">In a Web browser, go to this URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it! Instructions from the page and paste them into the Text Web part. Your page should look like the following.</span></span> 

![Page incorporer](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="9aa4f-127">Cliquez sur **publier**, puis copiez l'URL de la page et collez-la dans le bloc-notes.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="9aa4f-128">Étape 2: créer la playlist</span><span class="sxs-lookup"><span data-stu-id="9aa4f-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="9aa4f-p105">Accédez à la page **administration de formation personnalisée** dans votre expérience de site. ![custom_admin. png](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="9aa4f-p105">Navigate to the **Custom Learning Administration** page in your site experience. ![custom_admin.png](media/custom_admin.png)</span></span>
1. <span data-ttu-id="9aa4f-131">Vérifier que la **catégorie** est sélectionnée</span><span class="sxs-lookup"><span data-stu-id="9aa4f-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="9aa4f-132">Cliquez sur la catégorie dans laquelle vous souhaitez que votre nouvelle playlist apparaisse.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="9aa4f-133">En regard du nom de la catégorie, cliquez sur le ![symbole plus custom_addplay. png.](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="9aa4f-133">Next to the category name, click on the plus symbol ![custom_addplay.png](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="9aa4f-p106">Renseignez les valeurs comme indiqué dans l'exemple ci-dessous, puis sélectionnez **créer**. ![custom_details. png](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="9aa4f-p106">Fill in the values as shown in the example below and select **Create**. ![custom_details.png](media/custom_details.png)</span></span>
- <span data-ttu-id="9aa4f-136">**Title** -nom d'affichage de la playlist</span><span class="sxs-lookup"><span data-stu-id="9aa4f-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="9aa4f-137">**Description** : informations sur les éléments qui seront appris</span><span class="sxs-lookup"><span data-stu-id="9aa4f-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="9aa4f-138">**Catégorie** -présélectionnée en fonction de votre sélection initiale</span><span class="sxs-lookup"><span data-stu-id="9aa4f-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="9aa4f-139">**Sous-catégorie** -présélectionnée en fonction de votre sélection initiale</span><span class="sxs-lookup"><span data-stu-id="9aa4f-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="9aa4f-140">**Technologie** : sélectionnez si nécessaire</span><span class="sxs-lookup"><span data-stu-id="9aa4f-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="9aa4f-141">**Niveau** -débutant, Intermidate ou avancé</span><span class="sxs-lookup"><span data-stu-id="9aa4f-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="9aa4f-142">**Audience** : permet de cibler du contenu sur la base d'une liste prédéfinie de rôles fournis par Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="9aa4f-143">Cliquez sur **enregistrer les détails**</span><span class="sxs-lookup"><span data-stu-id="9aa4f-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="9aa4f-p107">Vous pouvez personnaliser l'image de l'icône pour votre sélection.  Cliquez sur l'icône de l'image et insérez une URL d'une image précédemment chargée.  Assurez-vous que l'image se trouve dans la collection de sites d'apprentissage personnalisée ou dans un autre emplacement où tous les utilisateurs auront accès au fichier.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-p107">You can customize the icon image for your playlist.  Click the image icon and insert an URL of a previously uploaded image.  Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="9aa4f-147">![custom_image. png](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="9aa4f-147">![custom_image.png](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="9aa4f-148">Étape 3: ajouter des ressources à la liste de lecture</span><span class="sxs-lookup"><span data-stu-id="9aa4f-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="9aa4f-149">Dans cette étape, vous allez ajouter des biens existants de Microsoft et la page SharePoint que vous avez créée dans la liste de lecture.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="9aa4f-150">Une fois que vous avez enregistré les détails de votre playlist, vous pouvez utiliser la recherche pour les ressources existantes.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="9aa4f-p108">**Entrez un terme de recherche** pour afficher la liste des biens prédéfinis disponibles dans d'autres playlists. **Cliquez sur le nom** d'un élément pour l'inclure dans votre nouvelle playlist. ![custom_slist. png](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="9aa4f-p108">**Enter in any search term** to see a list of predefined assets that are available from other playlists. **Click on the name** of an asset to include it in your new playlist. ![custom_slist.png](media/custom_slist.png)</span></span>

<span data-ttu-id="9aa4f-154">Vous pouvez également ajouter la page SharePoint que vous avez créée précédemment ou en créer une de toutes pièces dans l'expérience.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="9aa4f-155">Cliquez sur l'option **nouvel élément** dans la boîte de dialogue Liste des éléments de sélection.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-155">Click on the **New Asset** option in the Playlist Assets dialog</span></span>
1. <span data-ttu-id="9aa4f-p109">Donnez un **titre**à votre ressource. Une fois entrés, les options ![supplémentaires affichent custom_newpage. png.](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="9aa4f-p109">Give your asset a **Title**. Once entered, additional options will display ![custom_newpage.png](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="9aa4f-158">Vous pouvez désormais créer une page de ressource dans SharePoint Online ou entrer l'URL d'une page existante pour l'ajouter à votre sélection personnalisée.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-158">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="9aa4f-159">Les champs **catégorie**, **sous-catégorie** et **technologie** seront pré-remplis en fonction de vos sélections précédentes pour cette playlist.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-159">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="9aa4f-160">Effectuez les sélections appropriées pour le niveau et l'audience de cet élément individuel.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-160">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="9aa4f-161">Cliquez sur **enregistrer l'élément** pour l'ajouter à la playlist personnalisée.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-161">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="9aa4f-162">Répétez ces étapes, que vous recherchiez ou ajoutiez des pages, jusqu'à ce que votre playlist soit terminée.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-162">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="9aa4f-163">Cliquez sur **Fermer la playlist** pour enregistrer</span><span class="sxs-lookup"><span data-stu-id="9aa4f-163">Click **Close Playlist** to save</span></span>

<span data-ttu-id="9aa4f-164">Votre playlist avec ce contenu sera désormais disponible partout où vous avez installé/intégré le composant WebPart formation personnalisée.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-164">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="9aa4f-165">Si vous avez commis une erreur après avoir fermé la sélection, vous pouvez la supprimer de la catégorie en cliquant sur X en regard du nom de la playlist.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-165">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="9aa4f-166">Points à considérer</span><span class="sxs-lookup"><span data-stu-id="9aa4f-166">Things to Think About</span></span>

<span data-ttu-id="9aa4f-p110">Les playlists personnalisées peuvent être utilisées pour aider vos utilisateurs finaux à effectuer diverses tâches.  Disposez-vous d'un formulaire de demande de délai d'expiration?  Un formulaire pour demander de l'équipement matériel?  Tous les composants de formation existants peuvent être programmés dans l'expérience.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-p110">Custom playlists can be used to assist your end users in a variety of tasks.  Do you have a time off request form?  A form to request hardware equipment?  Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="9aa4f-171">Partager des sélections</span><span class="sxs-lookup"><span data-stu-id="9aa4f-171">Share Playlists</span></span>

1. <span data-ttu-id="9aa4f-172">Accéder à une playlist dans l'expérience de composant WebPart ou de site</span><span class="sxs-lookup"><span data-stu-id="9aa4f-172">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="9aa4f-173">Dans le coin supérieur gauche, vous verrez trois icônes.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-173">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="9aa4f-174">Cliquer sur l'icône représentant un lien</span><span class="sxs-lookup"><span data-stu-id="9aa4f-174">Click on the icon representing a link</span></span>
1. <span data-ttu-id="9aa4f-175">Copier l'URL vers la playlist</span><span class="sxs-lookup"><span data-stu-id="9aa4f-175">Copy the URL to the playlist</span></span>

<span data-ttu-id="9aa4f-176">![share. png](media/share.png) cette URL peut maintenant être insérée dans la navigation de votre site ou dans d'autres communications pour mettre vos employés directement dans cette playlist.</span><span class="sxs-lookup"><span data-stu-id="9aa4f-176">![share.png](media/share.png) This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoptiondriveadoptionmd"></a><span data-ttu-id="9aa4f-177">Étapes suivantes- [adoption du lecteur](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="9aa4f-177">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
