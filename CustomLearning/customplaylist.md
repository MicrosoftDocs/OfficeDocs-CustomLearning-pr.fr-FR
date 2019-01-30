# <a name="customize-the-services-and-playlists"></a><span data-ttu-id="5029d-101">Personnaliser les Services et les listes de diffusion</span><span class="sxs-lookup"><span data-stu-id="5029d-101">Customize the Services and Playlists</span></span>

<span data-ttu-id="5029d-p101">Par défaut à la fois l’expérience de site et le composant webpart incluent le contenu de tous les services Office 365.  Si une seule tout ou partie de ces services sont disponibles dans votre société, vous pouvez ajuster le contenu est disponible pour vos utilisateurs.  Dans cet article, nous personnaliser le contenu du composant webpart.</span><span class="sxs-lookup"><span data-stu-id="5029d-p101">By default both the site experience and the webpart include content for all Office 365 services.  If only all or some of these services are available in your company you can adjust what content is available to your users.  In this article we will customize the webpart content.</span></span>  

## <a name="customizing-the-webpart-content"></a><span data-ttu-id="5029d-105">Personnaliser le contenu du composant webpart</span><span class="sxs-lookup"><span data-stu-id="5029d-105">Customizing the webpart content</span></span>

<span data-ttu-id="5029d-106">Le composant webpart personnalisé Learning fournit deux fonctionnalités principales :</span><span class="sxs-lookup"><span data-stu-id="5029d-106">The Custom Learning webpart provides two key features:</span></span>
- <span data-ttu-id="5029d-107">Masquer les Technologies</span><span class="sxs-lookup"><span data-stu-id="5029d-107">Hide/Show Technologies</span></span>
- <span data-ttu-id="5029d-108">Créer une sélection</span><span class="sxs-lookup"><span data-stu-id="5029d-108">Create a Playlist</span></span>

### <a name="hide-or-show-technology-categories"></a><span data-ttu-id="5029d-109">Masquer ou afficher les catégories de technologies</span><span class="sxs-lookup"><span data-stu-id="5029d-109">Hide or Show Technology Categories</span></span>

<span data-ttu-id="5029d-110">Pour masquer et afficher le contenu dans le composant WebPart :</span><span class="sxs-lookup"><span data-stu-id="5029d-110">To hide and show content in the Web part:</span></span> 
1.  <span data-ttu-id="5029d-111">Cliquez sur le menu déroulant du composant webpart, puis cliquez sur Afficher/masquer les Technologies</span><span class="sxs-lookup"><span data-stu-id="5029d-111">Click the dropdown menu on the webpart, then click Hide/Show Technologies</span></span>

![Option de menu](media/clohideshow.png)

2. <span data-ttu-id="5029d-113">Sélectionnez un checkox pour masquer ou afficher une technologie et sélectionnez **Appliquer**.</span><span class="sxs-lookup"><span data-stu-id="5029d-113">Select a checkox to hide or show a technology and select **Apply**.</span></span>

![Options de technologie](media/clohideshow1.png)

### <a name="create-a-playlist"></a><span data-ttu-id="5029d-115">Créer une sélection</span><span class="sxs-lookup"><span data-stu-id="5029d-115">Create a Playlist</span></span>

<span data-ttu-id="5029d-p102">Une sélection est une compliation de « ressources ». Un « actif » est une page SharePoint ou un élément existant du contenu de formation Microsoft. Lorsque vous créez une sélection vous sélectionnez actifs qui vont ensemble pour créer un chemin d’accès de formation pour vos utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="5029d-p102">A playlist is a compliation of "assets". An "asset" is a SharePoint page or existing item of Microsoft training content. When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="5029d-p103">L’avantage de l’ajout de pages SharePoint est que vous pouvez créer des pages SharePoint avec un YouTube vidéos ou vidéos hébergées dans votre organisation. Vous pouvez également créer des pages avec des formulaires ou tout autre contenu Office 365.</span><span class="sxs-lookup"><span data-stu-id="5029d-p103">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization. You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="5029d-121">Étape 1 : Créer une page SharePoint pour votre sélection.</span><span class="sxs-lookup"><span data-stu-id="5029d-121">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="5029d-p104">Dans cet exemple, nous allons d’abord créer une page SharePoint à ajouter à la sélection. Nous allons créer une page avec un composant WebPart vidéo YouTube et un composant WebPart de texte.  Ces instructions supposent que vous utilisez le service SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="5029d-p104">In this example, we’ll first create a SharePoint page to add to the playlist. We’ll create a page with a YouTube video web part and Text web part.  These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="5029d-125">Créer une nouvelle page</span><span class="sxs-lookup"><span data-stu-id="5029d-125">Create a new page</span></span>
1.  <span data-ttu-id="5029d-126">Sélectionnez les paramètres du menu > contenu du Site > Pages du Site > nouveau > Page du Site.</span><span class="sxs-lookup"><span data-stu-id="5029d-126">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="5029d-127">Dans la zone Titre, tapez utiliser la zone de commande d’équipes</span><span class="sxs-lookup"><span data-stu-id="5029d-127">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="5029d-128">Sélectionnez Ajouter une nouvelle section, puis sélectionnez deux colonnes.</span><span class="sxs-lookup"><span data-stu-id="5029d-128">Select the Add a new section, and then select Two Columns.</span></span>

![Ajoutez deux colonnes](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="5029d-130">Dans la zone de gauche, sélectionnez Ajouter un nouveau composant WebPart, puis sélectionnez incorporer.</span><span class="sxs-lookup"><span data-stu-id="5029d-130">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="5029d-131">Dans un navigateur Web, accédez à cette URL https://youtu.be/wYrRCRphrp0 et obtenir le code intégré pour la vidéo.</span><span class="sxs-lookup"><span data-stu-id="5029d-131">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="5029d-132">Dans le composant WebPart de SharePoint, sélectionnez Ajouter incorporer le code et collez-le dans la zone incorporer.</span><span class="sxs-lookup"><span data-stu-id="5029d-132">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="5029d-133">Dans la zone de droite, sélectionnez Ajouter un nouveau composant WebPart, puis sélectionnez texte.</span><span class="sxs-lookup"><span data-stu-id="5029d-133">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="5029d-p105">Dans un navigateur Web, accédez à cette URL : https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b et copier le bloc Try il ! Instructions de la page et collez-les dans le composant WebPart de texte. Votre page doit se présenter comme suit.</span><span class="sxs-lookup"><span data-stu-id="5029d-p105">In a Web browser, go to this URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it! Instructions from the page and paste them into the Text Web part. Your page should look like the following.</span></span> 

![Incorporation de page](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="5029d-138">Cliquez sur Publier, puis copiez l’URL de la page et collez-le dans le bloc-notes</span><span class="sxs-lookup"><span data-stu-id="5029d-138">Click Publish, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="5029d-139">Étape 2 : Créer la sélection</span><span class="sxs-lookup"><span data-stu-id="5029d-139">Step 2: Create the Playlist</span></span>
1.  <span data-ttu-id="5029d-p106">Accédez à où vous avez installé le composant webpart personnalisé apprentissage. Dans l’expérience de site complète, il est hébergé sur la page de formation Office 365.</span><span class="sxs-lookup"><span data-stu-id="5029d-p106">Navigate to where you have installed the Custom Learning webpart. In the full site experience it is hosted on the Office 365 training page.</span></span> 
2.  <span data-ttu-id="5029d-142">Dans le menu déroulant, sélectionnez Créer une nouvelle sélection.</span><span class="sxs-lookup"><span data-stu-id="5029d-142">From the dropdown menu select Create New Playlist.</span></span> 

![créer une sélection personnalisée](media/clo365createplaylist.png)

3.  <span data-ttu-id="5029d-144">Renseignez les valeurs comme indiqué dans l’exemple ci-dessous, sélectionnez **créer**.</span><span class="sxs-lookup"><span data-stu-id="5029d-144">Fill in the values as shown in the example below and select **Create**.</span></span> 

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="5029d-145">Étape 3 : Ajouter des ressources à la sélection</span><span class="sxs-lookup"><span data-stu-id="5029d-145">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="5029d-146">Dans cette étape, vous allez ajouter des ressources existantes de Microsoft et de la page SharePoint que vous avez créé à la sélection.</span><span class="sxs-lookup"><span data-stu-id="5029d-146">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1.  <span data-ttu-id="5029d-147">Cliquez sur le bouton menu, puis cliquez sur Ajouter un élément existant.</span><span class="sxs-lookup"><span data-stu-id="5029d-147">Click the menu button, then click Add Existing Asset.</span></span>

![ajouter des biens](media/clo365addasset.png)

2.  <span data-ttu-id="5029d-149">Filtre pour la formation des équipes de Microsoft Office 365 applications ></span><span class="sxs-lookup"><span data-stu-id="5029d-149">Filter on Office 365 Apps > Microsoft Teams Training</span></span>
3.  <span data-ttu-id="5029d-150">Ajouter Bienvenue à Microsoft Teams, que votre équipe en cours d’exécution et démarrer des conversations et émettre des appels.</span><span class="sxs-lookup"><span data-stu-id="5029d-150">Add Welcome to Microsoft Teams, Get your team up and running, and Start chats and make calls.</span></span>
4.  <span data-ttu-id="5029d-151">Sélectionnez le > du bouton menu Créer actif.</span><span class="sxs-lookup"><span data-stu-id="5029d-151">Select the menu button > Create Asset.</span></span>
5.  <span data-ttu-id="5029d-152">Type, utilisez la zone de commande d’équipes dans la zone de titre actif.</span><span class="sxs-lookup"><span data-stu-id="5029d-152">Type Use the Teams command box in the Asset title box.</span></span> 
6.  <span data-ttu-id="5029d-153">Coller l’utilisation de SharePoint à l’URL de page boîte équipes commande vous avez copié dans le champ de contenu actif.</span><span class="sxs-lookup"><span data-stu-id="5029d-153">Paste the SharePoint Use the Teams command box page URL you copied in the Asset content field.</span></span> 
7.  <span data-ttu-id="5029d-p107">Accédez maintenant à la > de sélections personnalisé > Page d’accueil de votre première jours avec des équipes > utilisent la zone de commande d’équipes. Votre page doit se présenter comme suit.</span><span class="sxs-lookup"><span data-stu-id="5029d-p107">Now navigate back to the Home Page > Custom Playlists > Your first days with Teams > Use the Teams command box. Your page should look like the following.</span></span> 

![page créée](media/clo365createplaylist2.png)

<span data-ttu-id="5029d-157">Votre sélection avec ce contenu sera désormais disponible n’importe où vous avez installé / incorporée du composant webpart personnalisé apprentissage.</span><span class="sxs-lookup"><span data-stu-id="5029d-157">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

#### <a name="things-to-think-about"></a><span data-ttu-id="5029d-158">Choses à envisager</span><span class="sxs-lookup"><span data-stu-id="5029d-158">Things to Think About</span></span>

<span data-ttu-id="5029d-p108">Sélections personnalisées peuvent servir à aider vos utilisateurs finaux dans un vareity des tâches.  Avez-vous besoin d’un formulaire de demande de congés ?  Un formulaire pour demander le matériel ?  Les ressources de formation existantes peuvent être programmées dans l’environnement.</span><span class="sxs-lookup"><span data-stu-id="5029d-p108">Custom playlists can be used to assist your end users in a vareity of tasks.  Do you have a time off request form?  A form to request hardware equipment?  Any existing training assets can be programmed into the experience.</span></span>  
