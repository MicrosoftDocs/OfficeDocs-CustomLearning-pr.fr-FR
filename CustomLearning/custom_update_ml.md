---
author: pkrebs
ms.author: pkrebs
title: Mettre à jour les parcours d'apprentissage pour la prise en charge multilingue
ms.date: 05/20/2019
description: Mettre à jour les parcours d'apprentissage pour la prise en charge multilingue
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 9344cd91e5b6718b1eb0e73e25fdc8311afed793
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000240"
---
# <a name="update-learning-pathways-for-multilingual-support"></a>Mettre à jour les parcours d'apprentissage pour la prise en charge multilingue
Si vous avez un site parcours d'apprentissage existant, vous pouvez le mettre à jour pour une prise en charge multilingue. Pour mettre à jour le parcours d'apprentissage vers la version multilingue 4.0, vous téléchargez le package de partie Web, customlearning.sppkg, dans le catalogue d'applications client SharePoint. Lorsque vous mettez à jour le parcours d'apprentissage :  

- Toutes les sélections et ressources personnalisées créées précédemment sont conservées
- Les paramètres de masque ou d'afficher le contenu sont conservés
- Le modèle SharePoint du parcours d'apprentissage reste inchangé
- Les pages du site du parcours d'apprentissage ne sont pas traduites. Ce travail doit être effectué manuellement

## <a name="read-the-learning-pathways-multilingual-overview"></a>Lire la vue d'ensemble multilingue du parcours d'apprentissage
Pour en savoir plus sur le fonctionnement de la prise en charge multilingue du parcours d'apprentissage, lisez la vue d'ensemble multilingue [du parcours d'apprentissage.](custom_overview_ml.md) 

## <a name="prerequisites-to-update"></a>Conditions préalables à la mise à jour
Avant de mettre à jour le parcours d'apprentissage, les conditions préalables suivantes doivent être remplies :
- La personne qui met à jour le parcours d'apprentissage doit être propriétaire de la collection de sites du catalogue d'applications client. Si le parcours d'apprentissage de mise en service de la personne n'est pas propriétaire de collection de sites du catalogue d'applications, complétez ces [instructions](addappadmin.md) et continuez. 

## <a name="set-language-settings"></a>Définir les paramètres de langue 
Avant de mettre à jour les parcours d'apprentissage, définissez les paramètres de langue du site. Pour activer la prise en charge multilingue du site du parcours d'apprentissage, vous pouvez définir les pages et actualités Activer pour qu'ils soient traduits dans plusieurs **langues** sur **Activé,** puis ajouter les langues que vous souhaitez prendre en charge pour le site.
1.  Dans le site Parcours d'apprentissage, sélectionnez **Paramètres** dans la partie supérieure droite, puis sélectionnez **Informations sur le site.**
2.  En bas du volet d'informations du site, sélectionnez **Afficher tous les paramètres du site.**
3.  Sous **Administration du site,** sélectionnez **Paramètres de langue.**
4.  Sous Activer les pages et les actualités à traduire dans **plusieurs langues,** définissez le bouton bascule. 
- Pour un site multiligif, faites glisser le curseur sur **Sur,** puis continuez à la section Ajouter des langues. 
- Pour un site en anglais uniquement, faites glisser le curseur vers **l'autre**.

### <a name="add-languages"></a>Ajouter des langues
Le parcours d'apprentissage prend en charge neuf langues; vous devez ajouter uniquement les langues dont vous avez besoin. Dans les exemples utilisés dans cette documentation, l'italien est ajouté. 
- Sous **Ajouter ou supprimer des langues de site,** commencez à taper un nom de langue dans Sélectionner ou **taper** une langue, ou choisissez une langue dans ladown. Vous pouvez répéter cette étape pour ajouter plusieurs langues. Vous pouvez ajouter ou supprimer des langues de votre site à tout moment en revenir à cette page.
 
### <a name="assign-translators"></a>Affecter des traducteurs
Lors de la définition des paramètres de langue pour le parcours d'apprentissage, vous pouvez affecter des traducteurs. Un profil de langue étrangère doit être installé pour les traducteurs. Pour plus d'informations sur les profils de langue étrangère, voir [Créer des sites de communication multilingues, des pages et des actualités.](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)  
- Pour une langue prise en charge, cliquez sur **Sélectionner ou tapez un** traducteur, puis sélectionnez un traducteur. 

## <a name="update-the-learning-pathways-web-part-package"></a>Mettre à jour le package de la partie Web Du parcours d'apprentissage
Dans cette étape, vous téléchargez le volet Web Parcours d'apprentissage 4.0 dans le catalogue d'applications SharePoint, puis accédez à la page d'administration du parcours d'apprentissage pour démarrer le processus de mise à jour.

### <a name="upload-the-web-part-package"></a>Télécharger le package de la partie Web
1.  Go to the [GitHub custom learning repository,](https://github.com/pnp/custom-learning-office-365/tree/master/webpart)select **customlearning.sppkg** and then download it to a local drive on your PC. 
2.  Si vous n’êtes pas encore connecté, connectez-vous à votre client avec un administrateur de client ou un compte d’administrateur de collection de sites. 
3.  Cliquez **sur Admin** Show  >  **all**  >  **SharePoint** More  >  **Features**. 
4.  Sous **Applications,** cliquez sur **Ouvrir.** 
5.  Cliquez **sur Catalogue**  >  **d'applications Distribuer des applications pour SharePoint.** 
6.  Cliquez **sur Télécharger** choisir des  >  **fichiers.** 
7.  Sélectionnez **le fichier customlearning.sppkg** que vous avez téléchargé, cliquez sur **OK**  >  **Déployer.** 

### <a name="complete-the-update"></a>Terminer la mise à jour
1.  Dans le site Parcours d'apprentissage, sélectionnez Administration du parcours **d'apprentissage** **dans** le menu Accueil. 
2.  Vous verrez une invite vous demandant si vous souhaitez mettre à jour. 
![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)
3.  Cliquez sur **Démarrer**. 
4. Lorsque la mise à jour est terminée, cliquez sur **Fermer.** 

### <a name="next-steps"></a>Étapes suivantes
- Explorez le [contenu par défaut](custom_exploresite.md) fourni dans le site et le site Web.
- Pour plus d'informations sur la traduction des pages de site, voir [Traduire les pages du site.](custom_translate_page_ml.md) 

