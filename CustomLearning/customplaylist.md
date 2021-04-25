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
# <a name="customize-and-share-playlists"></a>Personnaliser et partager des playlists

## <a name="create-a-playlist"></a>Créer une playlist

Une playlist est une compliation des « ressources ». Une « ressources » est une page SharePoint ou un élément existant de contenu de formation Microsoft. Lorsque vous créez une playlist, vous sélectionnez les ressources qui vont ensemble pour créer un parcours d'apprentissage pour votre utilisateur.  

L'avantage de l'ajout de pages SharePoint est que vous pouvez créer des pages SharePoint avec des vidéos YouTube ou des vidéos hébergées dans votre organisation. Vous pouvez également créer des pages avec des formulaires ou d'autres contenus Office 365.  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a>Étape 1 : Créer une page SharePoint pour votre playlist
Dans cet exemple, nous allons d'abord créer une page SharePoint à ajouter à la playlist. Nous allons créer une page avec un partie web de vidéo YouTube et un élément Web Part Texte.  Ces instructions supposent que vous utilisez le service SharePoint Online. 

#### <a name="create-a-new-page"></a>Créez une page.
1.  Sélectionnez le menu Paramètres > contenu du site > Pages du site > Page > Site.
2.  Dans la zone de titre, tapez Utiliser la zone de commande Teams
3.  Sélectionnez la section Ajouter une nouvelle section, puis deux colonnes.

![ajouter deux colonnes](media/clo365addtwocolumn.png)

4.  Dans la zone de gauche, sélectionnez Ajouter un nouveau site Web, puis Incorporer. 
5.  Dans un navigateur Web, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video. 
6.  Dans le partie Web Part SharePoint, sélectionnez Ajouter du code d'incorporation, puis collez-le dans la zone Incorporer. 
7.  Dans la zone de droite, sélectionnez Ajouter un nouveau site Web, puis sélectionnez Texte. 
8.  Dans un navigateur Web, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it! Instructions de la page et collez-les dans le volet Texte. Votre page doit ressembler à ce qui suit. 
![Page Incorporer](media/clo365teamscommandbox.png)
9.  Cliquez **sur** Publier, puis copiez l'URL de la page et collez-la dans le Bloc-notes

#### <a name="step-2-create-the-playlist"></a>Étape 2 : Créer la playlist

1. Accédez à la page **Administration de l'apprentissage personnalisé** dans votre expérience de site.
![Écran dans lequel vous sélectionnez Administration de l'apprentissage personnalisé.](media/custom_admin.png)
1. Assurez-vous **que la** catégorie est sélectionnée 
1. Cliquez sur la catégorie dans laquelle vous souhaitez que votre nouvelle playlist apparaisse
1. En dehors du nom de la catégorie, cliquez sur la fenêtre symbole plus avec l'option Catégorie et le ![ signe Plus mis en surbrill valeur.](media/custom_addplay.png)

1. Remplissez les valeurs comme indiqué dans l'exemple ci-dessous, puis sélectionnez **Créer.** 
![Page dans laquelle vous entrez les détails de la sélection.](media/custom_details.png)
- **Titre** - Nom complet de la playlist
- **Description** : informations sur ce qui sera appris
- **Catégorie** : pré-sélectionné en fonction de votre sélection initiale
- **Sous-catégorie** : pré-sélectionné en fonction de votre sélection intial
- **Technologie** : sélectionnez le cas échéant
- **Niveau** - Débutant, Intermidate ou Avancé
- **Audience** : cela vous permet de cibler du contenu en fonction d'une liste prédéfinë de rôles fournis par Microsoft.

6. Cliquez sur **Enregistrer les détails**

> [!TIP]
> Vous pouvez personnaliser l'image d'icône de votre playlist.  Cliquez sur l'icône d'image et insérez l'URL d'une image précédemment téléchargée.  Assurez-vous que l'image se trouve dans la collection de sites d'apprentissage personnalisé ou dans un autre emplacement où tous les utilisateurs auront accès au fichier.  
![Choisissez une fenêtre d'image.](media/custom_image.png)

#### <a name="step-3-add-assets-to-the-playlist"></a>Étape 3 : Ajouter des ressources à la playlist
Dans cette étape, vous allez ajouter des ressources existantes de Microsoft et de la page SharePoint que vous avez créée à la playlist. 

1. Une fois que vous avez enregistré les détails de votre playlist, vous pouvez utiliser la recherche de ressources existantes.
1. **Entrez n'importe quel terme de** recherche pour voir une liste des ressources prédéfines disponibles à partir d'autres playlists. **Cliquez sur le nom d'un** bien pour l'inclure dans votre nouvelle playlist.<br/>
![Page Des ressources de sélection](media/custom_slist.png)

Vous pouvez également ajouter la page SharePoint que vous avez créée précédemment ou en créer une à partir de zéro dans l'expérience.

1. Cliquez sur **l'option Nouvel** actif dans la boîte de dialogue Playlist Assets.
1. Donnez un titre à votre **bien.** Une fois entrées, des options supplémentaires s'affichent.
![Formulaire dans lequel vous entrez votre titre et des détails supplémentaires.](media/custom_newpage.png)
1. Vous pouvez désormais créer une page de biens dans SharePoint Online ou entrer l'URL d'une page existante pour l'ajouter à votre playlist personnalisée. 
1. **Les** champs Catégorie, **Sous-catégorie** et Technologie seront pré-remplis en fonction de vos sélections précédentes pour cette playlist. 
1. Effectuer les sélections appropriées pour le niveau et l'audience pour cette bien individuelle.  
1. Cliquez **sur Enregistrer le bien** pour l'ajouter à la sélection personnalisée
1. Répétez ces étapes, en recherchant ou en ajoutant des pages individuelles, jusqu'à ce que votre playlist soit terminée. 
1. Cliquez **sur Fermer la playlist** pour enregistrer

Votre playlist avec ce contenu sera désormais disponible partout où vous avez installé/incorporé le site web d'apprentissage personnalisé. 

> [!NOTE]
> Si vous faites une erreur une fois que vous avez fermé la playlist, vous pouvez la supprimer de la catégorie en cliquant sur le X à côté du nom de la playlist.  

#### <a name="things-to-think-about"></a>Éléments à prendre en pense

Les playlists personnalisées peuvent être utilisées pour aider vos utilisateurs finaux dans diverses tâches.  Avez-vous un formulaire de demande de congé ?  Un formulaire pour demander de l'équipement matériel ?  Les ressources de formation existantes peuvent être programmées dans l'expérience.  

## <a name="share-playlists"></a>Partager des playlists

1. Accéder à n'importe quelle playlist dans l'expérience de site ou de webpart
1. Dans le coin supérieur gauche, vous verrez trois icônes
1. Cliquez sur l'icône représentant un lien
1. Copiez l'URL sur l'écran de sélection ![ où vous cliquez sur Copier en côté de l'URL.](media/share.png)
Cette URL peut désormais être insérée dans la navigation de votre site ou utilisée dans d'autres communications pour diriger vos employés directement vers cette playlist. 

### <a name="next-steps---drive-adoption"></a>Étapes suivantes : [stimuler l'adoption](driveadoption.md)
