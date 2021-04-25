---
author: pkrebs
ms.author: pkrebs
title: Résolution des problèmes liés aux parcours d’apprentissage de Microsoft 365
ms.date: 02/10/2019
description: Découvrez comment résoudre les problèmes du parcours d'apprentissage de Microsoft 365
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 7190688d574042c8a1b8dfb67c8b246dfbf8c927
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000300"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a>Résoudre les problèmes du parcours d'apprentissage de Microsoft 365

Voici des conseils de dépannage pour les problèmes qui peuvent se produire avec les parcours d'apprentissage de Microsoft 365 ou le service d'approvisionnement SharePoint Online.

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>Comment savoir si vous avez des autorisations d'administrateur client

Connectez-vous au service d'approvisionnement SharePoint Online et l'approvisionnement d'apprentissage personnalisé nécessite des autorisations d'administrateur client. Si vous rencontrez des problèmes de connect avec le service d'approvisionnement SharePoint Online, assurez-vous que le rôle d'administrateur général vous a été attribué. La solution d'apprentissage personnalisé nécessite des autorisations d'administrateur client, également appelées rôle d'administrateur général Office 365. Voici comment déterminer si le rôle Administrateur général vous a été attribué.

1.  Connectez-vous à Office.com.
2.  Cliquez sur **Administrateur**
3.  Sous **Utilisateurs**, sélectionnez **Utilisateurs actifs**
4.  Rechercher votre nom
5.  Cliquez sur votre nom dans les résultats de la recherche. Vous devez voir l'administrateur général pour votre rôle.
![Exemple de page répertoriant votre rôle, ainsi que les licences, les appartenances aux groupes et d'autres informations.](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>Si vous n'avez pas le rôle d'administrateur général
- Recherchez un administrateur général dans votre organisation et demandez à cette personne de se connectez au service ou demandez-lui de vous attribuer le rôle d'administrateur général.

## <a name="tenant-app-catalog-troubleshooting"></a>Résolution des problèmes du catalogue d'applications client
L'apprentissage personnalisé nécessite la mise en service d'un catalogue d'applications dans le client cible. La création d'un catalogue d'applications nécessite des autorisations d'administrateur général. Voici les étapes de résolution des problèmes courants du catalogue d'applications :

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>Comment savoir si vous avez un catalogue d'applications client 
Pour commencer, assurez-vous que vous avez des autorisations d'administrateur général. Consultez les étapes pour les autorisations d'administrateur client ci-dessus.

1. Dans Office 365, cliquez sur **Administrateur,** cliquez sur la flèche développer >, cliquez sur Afficher tous les  >  **centres d'administration**  >  **SharePoint**.
2. Cliquez **sur Catalogue d'applications SharePoint Center**  >  **d'administration**  >  **classique.**
3. Sous **Applications,** vous devriez voir une vignette intitulée **Distribuer des applications pour SharePoint.** Si vous voyez la vignette, vous avez un catalogue d'applications client. Consultez la section **Comment vous assurer qu'il s'agit d'une colllection de site...** ci-dessous. Si vous ne voyez pas la vignette, vous devrez créer un catalogue d'applications client pour votre client. Voir la **section Comment créer un catalogue d'applications client ci-dessous.**

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>Comment vous assurer que vous êtes propriétaire d'une collection de sites dans le catalogue d'applications client 
Pour mettre en service le parcours d'apprentissage de Microsoft 365, vous devez être propriétaire d'une collection de sites dans le catalogue d'applications client. Voici comment déterminer si vous êtes propriétaire.

1. Dans Office 365, cliquez sur **Administrateur,** cliquez sur la flèche développer >, cliquez sur Afficher tous les  >  **centres d'administration**  >  **SharePoint**.
2. Cliquez **sur Admin SharePoint Center** classique, puis sélectionnez le catalogue **d'applications.**
3. Sélectionnez **Propriétaire,** puis assurez-vous que vous êtes un propriétaire de collection de sites. Elle doit ressembler à ceci.
![Page Gérer les administrateurs.](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>Comment créer un catalogue d'applications client s'il n'en existe pas 
1. Connectez-vous à Office 365 avec votre compte d'administrateur SharePoint Online.
2. Cliquez sur **Admin**.
3. Sous **Centres d'administration,** cliquez **sur SharePoint.** 
4. Cliquez **sur Catalogue**  >  **d'applications.**
5. Cliquez **sur Créer un site de catalogue d'applications,** puis sur **OK.** 
6.  Entrez les informations du catalogue d'applications. Vous souhaitez peut-être inclure plusieurs administrateurs. Voici un exemple.  
![Formulaire pour entrer des informations pour un nouveau catalogue d'applications.](media/cg-appcatalogfinish.png)

7.  C’est fait. Vous avez terminé. Toutefois, avant de passer à la mise en service de l'apprentissage personnalisé, vous devez patienter au moins 30 minutes pour vous assurer que la création du catalogue d'applications est terminée. 

> [!IMPORTANT]
> Patientez au moins 30 minutes après la création du catalogue d'applications client avant de mettre en service l'apprentissage personnalisé. Cela garantit que le processus de mise en service du catalogue d'applications est terminé dans SharePoint. 