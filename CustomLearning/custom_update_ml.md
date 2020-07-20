---
author: pkrebs
ms.author: pkrebs
title: Mettre à jour les voies de formation pour la prise en charge multilingue
ms.date: 05/20/2019
description: Mettre à jour les voies de formation pour la prise en charge multilingue
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: 37a9b77ee45b8ae1ae4973f171c32de11fb530e1
ms.sourcegitcommit: 1f080ed4cf3687f922907304db3fd7a06aa9d501
ms.translationtype: Auto
ms.contentlocale: fr-FR
ms.lasthandoff: 07/02/2020
ms.locfileid: "45031700"
---
# <a name="update-learning-pathways-for-multilingual-support"></a>Mettre à jour les voies de formation pour la prise en charge multilingue
Si vous disposez d’un site de voies d’apprentissage existant, vous pouvez le mettre à jour pour la prise en charge multilingue. Pour mettre à jour les voies de formation vers la version multilingue 4,0, téléchargez le package de composants WebPart, customlearning. sppkg, dans le catalogue d’applications clientes SharePoint. Lorsque vous mettez à jour les voies de formation :  

- Tous les éléments et playlists personnalisés créés précédemment sont conservés
- Les paramètres permettant de masquer ou d’afficher le contenu sont conservés
- Le modèle de chemin d’apprentissage SharePoint reste inchangé.
- Les pages de site des voies d’apprentissage ne sont pas traduites. Ce travail doit être réalisé manuellement.

## <a name="read-the-learning-pathways-multilingual-overview"></a>Découvrez la vue d’ensemble des voies d’apprentissage
Pour en savoir plus sur le fonctionnement de la prise en charge multilingue pour les voies de formation, consultez la [rubrique formation : vue d’ensemble multilingue](custom_overview_ml.md). 

## <a name="prerequisites-to-update"></a>Conditions préalables à la mise à jour
Avant de mettre à jour les voies de formation, les conditions préalables suivantes doivent être remplies :
- La personne qui met à jour les voies de formation doit être un propriétaire de collection de sites du catalogue d’applications client. Si la personne chargée de la mise en service des chemins d’apprentissage n’est pas un propriétaire de collection de sites du catalogue d’applications, [suivez ces instructions](addappadmin.md) et continuez. 

## <a name="set-language-settings"></a>Définir les paramètres de langue 
Avant de mettre à jour les voies de formation, définissez les paramètres de langue du site. Pour activer la prise en charge multilingue pour le site des voies d’apprentissage, vous pouvez définir la **traduction des pages et des actualités en plusieurs langues** **, puis**ajouter les langues que vous souhaitez prendre en charge pour le site.
1.  Sur le site des voies d’apprentissage, sélectionnez **paramètres** dans la partie supérieure droite, puis sélectionnez **informations sur le site**.
2.  En bas du volet informations sur le site, sélectionnez **Afficher tous les paramètres du site**.
3.  Sous **administration du site**, sélectionnez **paramètres de langue**.
4.  Sous **activer la traduction des pages et des News en plusieurs langues**, définissez le commutateur bascule. 
- Pour un site multiligual, faites glisser le bouton bascule sur **activé**, puis passez à la section ajouter des langues. 
- Pour un site en anglais uniquement, faites glisser le bouton bascule sur **désactivé**.

### <a name="add-languages"></a>Ajouter des langues
Les voies d’apprentissage prennent en charge neuf langues, mais vous devez ajouter uniquement les langues dont vous avez besoin. Dans les exemples utilisés dans cette documentation, l’italien est ajouté. 
- Sous **Ajouter ou supprimer des langues de site**, commencez à taper un nom de langue dans **Sélectionner ou tapez une langue**, ou choisissez une langue dans la liste déroulante. Vous pouvez répéter cette étape pour ajouter plusieurs langues. Vous pouvez ajouter ou supprimer des langues de votre site à tout moment en revenant à cette page.
 
### <a name="assign-translators"></a>Affecter des traducteurs
Lors de la définition des paramètres de langue pour les voies de formation, vous pouvez attribuer des traducteurs. Un profil de langue étrangère doit être configuré pour les traducteurs. Pour plus d’informations sur les profils de langue étrangère, consultez la rubrique [créer des sites, des pages et des actualités de communication multilingue](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).  
- Pour une langue prise en charge, cliquez sur **Sélectionner ou tapez un traducteur** , puis sélectionnez un convertisseur. 

## <a name="update-the-learning-pathways-web-part-package"></a>Mettre à jour le package de composants WebPart des chemins d’apprentissage
Dans cette étape, vous téléchargez le composant WebPart voies d’apprentissage 4,0 dans le catalogue d’applications SharePoint, puis accédez à la page d’administration des voies d’apprentissage pour démarrer le processus de mise à jour.

### <a name="upload-the-web-part-package"></a>Télécharger le package de composants WebPart
1.  Accédez à l’emplacement de partage multilingue dans teams et téléchargez **customlearning. sppkg** sur un lecteur local de votre PC. 
2.  Si vous n’êtes pas déjà connecté, connectez-vous à votre client auprès d’un administrateur client ou d’un compte d’administrateur de collection de sites. 
3.  Cliquez sur **admin**  >  **afficher toutes les**  >  **SharePoint**  >  **fonctionnalités**SharePoint. 
4.  Sous **applications**, cliquez sur **ouvrir**. 
5.  Cliquez sur **catalogue**  >  **d’applications distribuer les applications pour SharePoint**. 
6.  Cliquez sur **Télécharger**  >  **Choose Files**. 
7.  Sélectionnez le fichier **customlearning. sppkg** que vous avez téléchargé, puis cliquez sur **OK**  >  **Deploy**. 

### <a name="complete-the-update"></a>Terminer la mise à jour
1.  À partir du site des voies d’apprentissage, sélectionnez **administration des voies** d’apprentissage dans le menu **Accueil** . 
2.  Un message vous demande si vous souhaitez effectuer une mise à jour. 
![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)
3.  Cliquez sur **Démarrer**. 
4. Lorsque la mise à jour est terminée, cliquez sur **Fermer**. 

### <a name="next-steps"></a>Étapes suivantes
- Explorez le [contenu par défaut](custom_exploresite.md) fourni dans le site et le composant WebPart.
- Pour plus d’informations sur la traduction des pages de site, voir [traduire des pages de site](custom_translate_page_ml.md). 

