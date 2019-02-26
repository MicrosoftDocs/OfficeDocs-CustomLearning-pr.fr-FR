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
# <a name="installing-the-custom-learning-solution-webpart"></a>Installation du composant WebPart de la solution d'apprentissage personnalisée

## <a name="prerequisites-for-a-tenant-wide-installation"></a>Conditions préalables pour une installation à l'échelle du client

- Pour installer le composant WebPart de formation personnalisée pour l'ensemble de votre client, vous devez disposer des autorisations d'administration d'Office 365.  Si vous ne disposez pas de ces autorisations, vous pouvez travailler avec votre administrateur Office 365 ou installer le composant WebPart pour une collection de sites individuelle.
- Vous ou votre administrateur Office 365 devez avoir configuré et configuré un [catalogue d'applications](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) à l'échelle du client ou un catalogue d'applications de [collection de sites](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)pour recevoir le composant WebPart.
- Nous prenons en charge SharePoint Online uniquement. Le composant WebPart n'est pas pris en charge pour l'installation sur une version de SharePoint sur site.

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a>Ajouter le composant WebPart formation personnalisée à votre client 

1. Téléchargez le composant WebPart formation personnalisée et enregistrez-le sur votre lecteur local.  Ce fichier est nommé «MS-Custom-Learning. sppkg».  Ne modifiez pas le nom ou le suffixe du fichier. 
2. Accédez au [portail d'administration Office 365](https://admin.microsoft.com/AdminPortal/Home#/homepage) pour votre client.
3. Dans le volet de navigation de gauche, sélectionnez centres d'administration, SharePoint. Cette opération s'ouvre dans un nouvel onglet., dans le centre d'administration SharePoint, sélectionnez applications, catalogue d'applications, applications pour SharePoint 
4. Sélectionnez Télécharger le composant WebPart et sélectionnez le fichier «MS-Custom-Learning. sppkg» que vous avez téléchargé
5. Pour cette installation à l'échelle du client, cochez la case en regard de «mettre cette solution à disposition de tous les» dans l'organisation.  
 
> [!NOTE]
> Une fois le composant WebPart installé, vous le trouverez dans votre galerie de WebPart dans SharePoint Online.  **Dans la Galerie, le composant WebPart est nommé «Microsoft Learning»**

![Déployer la solution](media/trustapp_sm.png)


## <a name="add-the-microsoft-learning-webpart-to-a-sharepoint-online-page"></a>Ajouter le composant WebPart formation Microsoft à une page SharePoint Online

Une fois que l'apprentissage personnalisé est installé dans votre client, vous pouvez ajouter le composant WebPart à une page SharePoint. La formation Office 365 et Windows 10 est disponible pour votre site.

1. Ajoutez le composant WebPart formation personnalisée dans une mise en forme de colonne à pleine chasse:

![Mise en page SharePoint](media/clo365fullcolumnwidth.png)

2. Dans la page SharePoint, sélectionnez Ajouter une section, puis sélectionnez colonne pleine chasse.  L'invite suivante apparaît:

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. Sélectionnez Microsoft Learning.  Vous devez maintenant voir les éléments suivants: 

![Composant WebPart formation personnalisée](media/clo365addwebpart.png)

 Vous pouvez maintenant cliquer sur les vignettes pour explorer le contenu par défaut inclus dans la solution.  

### <a name="next-steps"></a>Étapes suivantes
- Explorez le [contenu par défaut](webpartcontent.md) inclus dans le composant WebPart.
- [Personnaliser](customization.md) l'expérience de formation pour votre organisation.
- Encouragez l' [adoption](driveadoption.md) de votre solution de formation.

