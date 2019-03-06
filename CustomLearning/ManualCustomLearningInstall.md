# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>Installation et configuration manuelles de l'apprentissage personnalisé pour Office 365

Le composant WebPart formation personnalisée Microsoft est créé à l'aide de la version 1.7.1 de [SharePoint Framework](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/sharepoint-framework-overview) .

Pour installer et configurer manuellement le composant WebPart et la collection de sites, vous devez effectuer les étapes suivantes:

1. Vérifiez que vous remplissez toutes les conditions préalables.
1. Installez le fichier customlearning. sppkg dans votre catalogue d'applications client 365 Office.
1. Approvisionner/identifier un site de communication moderne qui sert de formation personnalisée pour votre site d'accueil Office 365.
1. Exécutez un script PowerShell qui configurera votre client avec les artefacts appropriés dont dépend l'apprentissage personnalisé.
1. Accédez à la page de site CustomLearningAdmin. aspx pour charger le composant WebPart d'administration afin d'initialiser la configuration de contenu personnalisé.

## <a name="prerequisites"></a>Conditions préalables

Vous devez avoir configuré et configuré le catalogue d'applications à l'échelle du client. Consultez la rubrique [configurer votre client Office 365](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) et suivez la section créer un site de catalogue d'applications. Si votre catalogue d'applications à l'échelle du client a déjà été mis en service, vous aurez besoin d'accéder à un compte disposant de droits de chargement d'un package vers celui-ci pour terminer le processus d'installation. Il s'agit généralement d'un compte doté du rôle d'administrateur SharePoint. Si un compte associé à ce rôle ne fonctionne pas, accédez au centre d'administration SharePoint et recherchez les administrateurs de collections de sites pour la collection de sites de catalogue d'applications, puis connectez-vous en tant qu'administrateur de collection de sites ou ajoutez le compte d'administrateur SharePoint. les administrateurs de collections de sites ont échoué. Vous aurez également besoin d'un accès à un compte qui est un administrateur de client SharePoint.

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>Télécharger le composant WebPart dans le catalogue d'applications client

Pour configurer la formation personnalisée pour Office 365, téléchargez le fichier customlearning. sppkg dans le catalogue d'applications à l'échelle du client et déployez-le. Pour obtenir des instructions détaillées sur l'ajout d'une application au catalogue d'applications, voir [utiliser le catalogue d'applications pour mettre à disposition des applications d'entreprise personnalisées pour votre environnement SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) .

## <a name="provisionidentify-modern-communication-site"></a>Mettre en service/identifier un site de communication moderne

Identifiez un site de communication SharePoint existant ou approvisionnez-en un nouveau dans votre client SharePoint Online. Pour plus d'informations sur la mise en service d'un site de communication, voir [créer un site de communication dans SharePoint Online](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) et suivre les étapes de création d'un site de communication.

## <a name="set-permissions-for-the-site"></a>Définir des autorisations pour le site

Vous pouvez ajouter tout le monde qui doit être en mesure d'afficher le contenu au groupe visiteurs et à toutes les personnes qui doivent être en mesure d'administrer les playlists personnalisées au groupe membres. Pour configurer le site pour la formation personnalisée la première fois, l'utilisateur doit être administrateur de collection de sites ou appartenir au groupe propriétaires.

Ajoutez une application personnalisée d'application Office 365 à la collection de sites.

## <a name="execute-powershell-configuration-script"></a>Exécuter un script de configuration PowerShell

Un script `CustomLearningConfiguration.ps1` PowerShell est inclus que vous devrez exécuter pour créer trois propriétés de [client](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) utilisées par la solution. De plus, le script crée deux [pages d'application à composant unique](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) dans la bibliothèque pages de site pour héberger les composants WebPart administrateur et utilisateur à un emplacement connu.

### <a name="disabling-telemetry-collection"></a>DésActivation de la collection de télémétrie

Une partie de cette solution inclut le suivi des télémétries anonyme, qui est défini par défaut sur activé. Si vous effectuez une installation manuelle et que vous souhaitez désactiver le suivi de la télémétrie, modifiez le `CustomlearningConfiguration.ps1` script de manière à définir la variable $optInTelemetry sur $false.

Si vous n'effectuez pas une installation manuelle et souhaitez désactiver le suivi de la télémétrie, un script `TelemetryOptOut.ps1` distinct a été inclus, lorsque l'exécution désactivera le suivi de télémétrie.

## <a name="initialize-web-part-custom-configuration"></a>Initialiser la configuration personnalisée du composant WebPart

Une fois le script PowerShell exécuté, accédez à `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. Cela initialise l'élément de liste CustomConfig qui configure la formation personnalisée pour sa première utilisation.

La configuration est maintenant terminée et vous pouvez passer à l'aide de la formation personnalisée pour Office 365. Pour plus d'informations, reportez-vous à la documentation de l'utilisateur.