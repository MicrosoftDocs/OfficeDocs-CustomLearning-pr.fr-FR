# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="6f894-101">Installation personnalisée du composant Webpart de Solution de formation</span><span class="sxs-lookup"><span data-stu-id="6f894-101">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="6f894-102">Conditions requises pour une installation de client à l’échelle</span><span class="sxs-lookup"><span data-stu-id="6f894-102">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="6f894-p101">Pour installer le composant webpart de formation personnalisé pour votre client entière, vous devez disposer des autorisations d’administration Office 365.  Si vous n’avez pas ces autorisations, vous pouvez l’administrateur Office 365 ou installez le composant webpart d’une collection de sites individuelles.</span><span class="sxs-lookup"><span data-stu-id="6f894-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="6f894-105">Votre administrateur ou vous Office 365 doit avoir le programme d’installation et configuré un [Catalogue d’applications](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) de client à l’échelle ou un [Catalogue d’applications de Collection de sites](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)pour recevoir le composant webpart.]</span><span class="sxs-lookup"><span data-stu-id="6f894-105">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="6f894-p102">Il prend en charge SharePoint Online uniquement. Le composant WebPart n’est pas prise en charge pour l’installation sur n’importe quelle version de SharePoint sur site.</span><span class="sxs-lookup"><span data-stu-id="6f894-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="6f894-108">Ajouter le composant webpart personnalisé apprentissage à votre client</span><span class="sxs-lookup"><span data-stu-id="6f894-108">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="6f894-p103">Téléchargez le composant webpart personnalisé apprentissage et enregistrez-le sur votre disque local.  Ce fichier est nommé « ms-personnalisé-learning.sppkg ».  Ne modifiez pas le nom ou le suffixe du fichier.</span><span class="sxs-lookup"><span data-stu-id="6f894-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="6f894-112">Accédez au [portail d’administration d’Office 365](https://admin.microsoft.com/AdminPortal/Home#/homepage) pour votre client</span><span class="sxs-lookup"><span data-stu-id="6f894-112">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="6f894-p104">Dans le volet de navigation gauche Sélectionnez centres d’administration de SharePoint. Il s’ouvre dans un nouvel onglet, dans le centre d’administration SharePoint sélectionnez applications, catalogue d’applications, les applications pour SharePoint</span><span class="sxs-lookup"><span data-stu-id="6f894-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="6f894-115">Sélectionnez Télécharger le composant webpart et choisissez le fichier « ms-personnalisé-learning.sppkg » que vous avez téléchargé</span><span class="sxs-lookup"><span data-stu-id="6f894-115">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="6f894-116">Pour cette vérification de l’installation du client à l’échelle la case en regard de « Rendre cette solution disponible pour tous les se trouve dans l’organisation ».</span><span class="sxs-lookup"><span data-stu-id="6f894-116">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  

![Déployer la Solution](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="6f894-118">Ajouter le composant webpart client formation à la Page SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6f894-118">Add the Customer Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="6f894-p105">Une fois l’apprentissage personnalisé est installé sur votre client, vous pouvez ajouter le composant WebPart à une page SharePoint. Lorsque vous le faites, formation Office 365 est soudainement à votre disposition.</span><span class="sxs-lookup"><span data-stu-id="6f894-p105">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do, suddenly Office 365 training is available to you.</span></span> 

1. <span data-ttu-id="6f894-121">Ajoutez le composant webpart personnalisé Learning dans une disposition de colonne pleine largeur :</span><span class="sxs-lookup"><span data-stu-id="6f894-121">Add the Custom Learning webpart in a full width column layout:</span></span>

![Mise en Page de SharePoint](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="6f894-p106">Dans la page SharePoint, sélectionnez la section Ajouter, puis sélectionnez colonne pleine chasse.  Vous verrez le message suivant :</span><span class="sxs-lookup"><span data-stu-id="6f894-p106">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="6f894-p107">Sélectionnez Microsoft Learning.  Vous devez maintenant voir les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="6f894-p107">Select Microsoft Learning.  You should now see the following:</span></span> 

![Personnalisé composant webpart de la formation](media/clo365addwebpart.png)

 <span data-ttu-id="6f894-129">Vous pouvez maintenant sur les mosaïques pour Explorer le contenu par défaut inclus dans la solution.</span><span class="sxs-lookup"><span data-stu-id="6f894-129">You can now click on the tiles to explore the default content included in the solution.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="6f894-130">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="6f894-130">Next Steps</span></span>
- <span data-ttu-id="6f894-131">Explorez le [contenu par défaut](webpartcontent.md) inclus dans le composant webpart.</span><span class="sxs-lookup"><span data-stu-id="6f894-131">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="6f894-132">[Personnaliser](customization.md) l’expérience de formation pour votre organisation.</span><span class="sxs-lookup"><span data-stu-id="6f894-132">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="6f894-133">[Lecteur d’adoption](driveadoption.md) de votre solution de formation.</span><span class="sxs-lookup"><span data-stu-id="6f894-133">[Drive adoption](driveadoption.md) of your training solution.</span></span>

