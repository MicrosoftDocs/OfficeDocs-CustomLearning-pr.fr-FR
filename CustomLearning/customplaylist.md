---
author: karuanag
ms.author: karuanag
manager: alexb
title: Personnaliser et partager des playlists
ms.date: 02/10/2019
description: Créer des playlists personnalisées à partir de contenu existant ou de nouvelles pages SharePoint
ms.service: sharepoint-online
audience: itpro
ms.topic: article
ms.openlocfilehash: 31a0e5524181d26f4d62ae7206636c9e553b6f8f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000210"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="66c57-103">Personnaliser et partager des playlists</span><span class="sxs-lookup"><span data-stu-id="66c57-103">Customize and share playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="66c57-104">Créer une playlist</span><span class="sxs-lookup"><span data-stu-id="66c57-104">Create a Playlist</span></span>

<span data-ttu-id="66c57-105">Une playlist est une compliation des « ressources ».</span><span class="sxs-lookup"><span data-stu-id="66c57-105">A playlist is a compliation of "assets".</span></span> <span data-ttu-id="66c57-106">Une « ressources » est une page SharePoint ou un élément existant de contenu de formation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="66c57-106">An "asset" is a SharePoint page or existing item of Microsoft training content.</span></span> <span data-ttu-id="66c57-107">Lorsque vous créez une playlist, vous sélectionnez les ressources qui vont ensemble pour créer un parcours d'apprentissage pour votre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="66c57-107">When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="66c57-108">L'avantage de l'ajout de pages SharePoint est que vous pouvez créer des pages SharePoint avec des vidéos YouTube ou des vidéos hébergées dans votre organisation.</span><span class="sxs-lookup"><span data-stu-id="66c57-108">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization.</span></span> <span data-ttu-id="66c57-109">Vous pouvez également créer des pages avec des formulaires ou d'autres contenus Office 365.</span><span class="sxs-lookup"><span data-stu-id="66c57-109">You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="66c57-110">Étape 1 : Créer une page SharePoint pour votre playlist</span><span class="sxs-lookup"><span data-stu-id="66c57-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="66c57-111">Dans cet exemple, nous allons d'abord créer une page SharePoint à ajouter à la playlist.</span><span class="sxs-lookup"><span data-stu-id="66c57-111">In this example, we’ll first create a SharePoint page to add to the playlist.</span></span> <span data-ttu-id="66c57-112">Nous allons créer une page avec un partie web de vidéo YouTube et un élément Web Part Texte.</span><span class="sxs-lookup"><span data-stu-id="66c57-112">We’ll create a page with a YouTube video web part and Text web part.</span></span>  <span data-ttu-id="66c57-113">Ces instructions supposent que vous utilisez le service SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="66c57-113">These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="66c57-114">Créez une page.</span><span class="sxs-lookup"><span data-stu-id="66c57-114">Create a new page</span></span>
1.  <span data-ttu-id="66c57-115">Sélectionnez le menu Paramètres > contenu du site > Pages du site > Page > Site.</span><span class="sxs-lookup"><span data-stu-id="66c57-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="66c57-116">Dans la zone de titre, tapez Utiliser la zone de commande Teams</span><span class="sxs-lookup"><span data-stu-id="66c57-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="66c57-117">Sélectionnez la section Ajouter une nouvelle section, puis deux colonnes.</span><span class="sxs-lookup"><span data-stu-id="66c57-117">Select the Add a new section, and then select Two Columns.</span></span>

![ajouter deux colonnes](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="66c57-119">Dans la zone de gauche, sélectionnez Ajouter un nouveau site Web, puis Incorporer.</span><span class="sxs-lookup"><span data-stu-id="66c57-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="66c57-120">Dans un navigateur Web, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span><span class="sxs-lookup"><span data-stu-id="66c57-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="66c57-121">Dans le partie Web Part SharePoint, sélectionnez Ajouter du code d'incorporation, puis collez-le dans la zone Incorporer.</span><span class="sxs-lookup"><span data-stu-id="66c57-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="66c57-122">Dans la zone de droite, sélectionnez Ajouter un nouveau site Web, puis sélectionnez Texte.</span><span class="sxs-lookup"><span data-stu-id="66c57-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="66c57-123">Dans un navigateur Web, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span><span class="sxs-lookup"><span data-stu-id="66c57-123">In a Web browser, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span></span> <span data-ttu-id="66c57-124">Instructions de la page et collez-les dans le volet Texte.</span><span class="sxs-lookup"><span data-stu-id="66c57-124">Instructions from the page and paste them into the Text Web part.</span></span> <span data-ttu-id="66c57-125">Votre page doit ressembler à ce qui suit.</span><span class="sxs-lookup"><span data-stu-id="66c57-125">Your page should look like the following.</span></span> 
<span data-ttu-id="66c57-126">![Page Incorporer](media/clo365teamscommandbox.png)</span><span class="sxs-lookup"><span data-stu-id="66c57-126">![Embed page](media/clo365teamscommandbox.png)</span></span>
9.  <span data-ttu-id="66c57-127">Cliquez **sur** Publier, puis copiez l'URL de la page et collez-la dans le Bloc-notes</span><span class="sxs-lookup"><span data-stu-id="66c57-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="66c57-128">Étape 2 : Créer la playlist</span><span class="sxs-lookup"><span data-stu-id="66c57-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="66c57-129">Accédez à la page **Administration de l'apprentissage personnalisé** dans votre expérience de site.</span><span class="sxs-lookup"><span data-stu-id="66c57-129">Navigate to the **Custom Learning Administration** page in your site experience.</span></span>
<span data-ttu-id="66c57-130">![Écran dans lequel vous sélectionnez Administration de l'apprentissage personnalisé.](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="66c57-130">![Screen where you select Custom Learning Administration.](media/custom_admin.png)</span></span>
1. <span data-ttu-id="66c57-131">Assurez-vous **que la** catégorie est sélectionnée</span><span class="sxs-lookup"><span data-stu-id="66c57-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="66c57-132">Cliquez sur la catégorie dans laquelle vous souhaitez que votre nouvelle playlist apparaisse</span><span class="sxs-lookup"><span data-stu-id="66c57-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="66c57-133">En dehors du nom de la catégorie, cliquez sur la fenêtre symbole plus avec l'option Catégorie et le ![ signe Plus mis en surbrill valeur.](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="66c57-133">Next to the category name, click on the plus symbol ![Window with the Category option and the Plus sign highlighted.](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="66c57-134">Remplissez les valeurs comme indiqué dans l'exemple ci-dessous, puis sélectionnez **Créer.**</span><span class="sxs-lookup"><span data-stu-id="66c57-134">Fill in the values as shown in the example below and select **Create**.</span></span> 
<span data-ttu-id="66c57-135">![Page dans laquelle vous entrez les détails de la sélection.](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="66c57-135">![Page where you enter playlist details.](media/custom_details.png)</span></span>
- <span data-ttu-id="66c57-136">**Titre** - Nom complet de la playlist</span><span class="sxs-lookup"><span data-stu-id="66c57-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="66c57-137">**Description** : informations sur ce qui sera appris</span><span class="sxs-lookup"><span data-stu-id="66c57-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="66c57-138">**Catégorie** : pré-sélectionné en fonction de votre sélection initiale</span><span class="sxs-lookup"><span data-stu-id="66c57-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="66c57-139">**Sous-catégorie** : pré-sélectionné en fonction de votre sélection intial</span><span class="sxs-lookup"><span data-stu-id="66c57-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="66c57-140">**Technologie** : sélectionnez le cas échéant</span><span class="sxs-lookup"><span data-stu-id="66c57-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="66c57-141">**Niveau** - Débutant, Intermidate ou Avancé</span><span class="sxs-lookup"><span data-stu-id="66c57-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="66c57-142">**Audience** : cela vous permet de cibler du contenu en fonction d'une liste prédéfinë de rôles fournis par Microsoft.</span><span class="sxs-lookup"><span data-stu-id="66c57-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="66c57-143">Cliquez sur **Enregistrer les détails**</span><span class="sxs-lookup"><span data-stu-id="66c57-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="66c57-144">Vous pouvez personnaliser l'image d'icône de votre playlist.</span><span class="sxs-lookup"><span data-stu-id="66c57-144">You can customize the icon image for your playlist.</span></span>  <span data-ttu-id="66c57-145">Cliquez sur l'icône d'image et insérez l'URL d'une image précédemment téléchargée.</span><span class="sxs-lookup"><span data-stu-id="66c57-145">Click the image icon and insert an URL of a previously uploaded image.</span></span>  <span data-ttu-id="66c57-146">Assurez-vous que l'image se trouve dans la collection de sites d'apprentissage personnalisé ou dans un autre emplacement où tous les utilisateurs auront accès au fichier.</span><span class="sxs-lookup"><span data-stu-id="66c57-146">Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="66c57-147">![Choisissez une fenêtre d'image.](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="66c57-147">![Choose an image window.](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="66c57-148">Étape 3 : Ajouter des ressources à la playlist</span><span class="sxs-lookup"><span data-stu-id="66c57-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="66c57-149">Dans cette étape, vous allez ajouter des ressources existantes de Microsoft et de la page SharePoint que vous avez créée à la playlist.</span><span class="sxs-lookup"><span data-stu-id="66c57-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="66c57-150">Une fois que vous avez enregistré les détails de votre playlist, vous pouvez utiliser la recherche de ressources existantes.</span><span class="sxs-lookup"><span data-stu-id="66c57-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="66c57-151">**Entrez n'importe quel terme de** recherche pour voir une liste des ressources prédéfines disponibles à partir d'autres playlists.</span><span class="sxs-lookup"><span data-stu-id="66c57-151">**Enter in any search term** to see a list of predefined assets that are available from other playlists.</span></span> <span data-ttu-id="66c57-152">**Cliquez sur le nom d'un** bien pour l'inclure dans votre nouvelle playlist.</span><span class="sxs-lookup"><span data-stu-id="66c57-152">**Click on the name** of an asset to include it in your new playlist.</span></span><br/>
<span data-ttu-id="66c57-153">![Page Des ressources de sélection](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="66c57-153">![Playlist assets page](media/custom_slist.png)</span></span>

<span data-ttu-id="66c57-154">Vous pouvez également ajouter la page SharePoint que vous avez créée précédemment ou en créer une à partir de zéro dans l'expérience.</span><span class="sxs-lookup"><span data-stu-id="66c57-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="66c57-155">Cliquez sur **l'option Nouvel** actif dans la boîte de dialogue Playlist Assets.</span><span class="sxs-lookup"><span data-stu-id="66c57-155">Click on the **New Asset** option in the Playlist Assets dialog.</span></span>
1. <span data-ttu-id="66c57-156">Donnez un titre à votre **bien.**</span><span class="sxs-lookup"><span data-stu-id="66c57-156">Give your asset a **Title**.</span></span> <span data-ttu-id="66c57-157">Une fois entrées, des options supplémentaires s'affichent.</span><span class="sxs-lookup"><span data-stu-id="66c57-157">Once entered, additional options will display.</span></span>
<span data-ttu-id="66c57-158">![Formulaire dans lequel vous entrez votre titre et des détails supplémentaires.](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="66c57-158">![Form where you enter your title and additional details.](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="66c57-159">Vous pouvez désormais créer une page de biens dans SharePoint Online ou entrer l'URL d'une page existante pour l'ajouter à votre playlist personnalisée.</span><span class="sxs-lookup"><span data-stu-id="66c57-159">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="66c57-160">**Les** champs Catégorie, **Sous-catégorie** et Technologie seront pré-remplis en fonction de vos sélections précédentes pour cette playlist. </span><span class="sxs-lookup"><span data-stu-id="66c57-160">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="66c57-161">Effectuer les sélections appropriées pour le niveau et l'audience pour cette bien individuelle.</span><span class="sxs-lookup"><span data-stu-id="66c57-161">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="66c57-162">Cliquez **sur Enregistrer le bien** pour l'ajouter à la sélection personnalisée</span><span class="sxs-lookup"><span data-stu-id="66c57-162">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="66c57-163">Répétez ces étapes, en recherchant ou en ajoutant des pages individuelles, jusqu'à ce que votre playlist soit terminée.</span><span class="sxs-lookup"><span data-stu-id="66c57-163">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="66c57-164">Cliquez **sur Fermer la playlist** pour enregistrer</span><span class="sxs-lookup"><span data-stu-id="66c57-164">Click **Close Playlist** to save</span></span>

<span data-ttu-id="66c57-165">Votre playlist avec ce contenu sera désormais disponible partout où vous avez installé/incorporé le site web d'apprentissage personnalisé.</span><span class="sxs-lookup"><span data-stu-id="66c57-165">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="66c57-166">Si vous faites une erreur une fois que vous avez fermé la playlist, vous pouvez la supprimer de la catégorie en cliquant sur le X à côté du nom de la playlist.</span><span class="sxs-lookup"><span data-stu-id="66c57-166">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="66c57-167">Éléments à prendre en pense</span><span class="sxs-lookup"><span data-stu-id="66c57-167">Things to Think About</span></span>

<span data-ttu-id="66c57-168">Les playlists personnalisées peuvent être utilisées pour aider vos utilisateurs finaux dans diverses tâches.</span><span class="sxs-lookup"><span data-stu-id="66c57-168">Custom playlists can be used to assist your end users in a variety of tasks.</span></span>  <span data-ttu-id="66c57-169">Avez-vous un formulaire de demande de congé ?</span><span class="sxs-lookup"><span data-stu-id="66c57-169">Do you have a time off request form?</span></span>  <span data-ttu-id="66c57-170">Un formulaire pour demander de l'équipement matériel ?</span><span class="sxs-lookup"><span data-stu-id="66c57-170">A form to request hardware equipment?</span></span>  <span data-ttu-id="66c57-171">Les ressources de formation existantes peuvent être programmées dans l'expérience.</span><span class="sxs-lookup"><span data-stu-id="66c57-171">Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="66c57-172">Partager des playlists</span><span class="sxs-lookup"><span data-stu-id="66c57-172">Share Playlists</span></span>

1. <span data-ttu-id="66c57-173">Accéder à n'importe quelle playlist dans l'expérience de site ou de webpart</span><span class="sxs-lookup"><span data-stu-id="66c57-173">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="66c57-174">Dans le coin supérieur gauche, vous verrez trois icônes</span><span class="sxs-lookup"><span data-stu-id="66c57-174">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="66c57-175">Cliquez sur l'icône représentant un lien</span><span class="sxs-lookup"><span data-stu-id="66c57-175">Click on the icon representing a link</span></span>
1. <span data-ttu-id="66c57-176">Copiez l'URL sur l'écran de sélection ![ où vous cliquez sur Copier en côté de l'URL.](media/share.png)</span><span class="sxs-lookup"><span data-stu-id="66c57-176">Copy the URL to the playlist ![Screen where you click Copy next to the URL.](media/share.png)</span></span>
<span data-ttu-id="66c57-177">Cette URL peut désormais être insérée dans la navigation de votre site ou utilisée dans d'autres communications pour diriger vos employés directement vers cette playlist.</span><span class="sxs-lookup"><span data-stu-id="66c57-177">This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoption"></a><span data-ttu-id="66c57-178">Étapes suivantes : [stimuler l'adoption](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="66c57-178">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
