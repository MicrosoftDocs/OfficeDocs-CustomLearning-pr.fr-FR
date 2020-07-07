---
author: pkrebs
ms.author: pkrebs
title: Mettre en service une nouvelle solution de voies d’apprentissage
ms.date: 02/10/2019
description: Approvisionner le site des chemins d’apprentissage Microsoft 365 avec le service Microsoft 365 Look Book
ms.openlocfilehash: 2ab7ca9c7c66ce86be09fcfd95d3ccfd18682777
ms.sourcegitcommit: 0b56b96c215d4a5dd18fbeafc40b9fe63ff18b16
ms.contentlocale: fr-FR
ms.lasthandoff: 07/06/2020
ms.locfileid: "45048122"
---
# <a name="provision-a-new-learning-pathways-solution"></a>Mettre en service une nouvelle solution de voies d’apprentissage 
Les organisations qui n’ont pas de voies d’apprentissage configurées dans leur client peuvent utiliser le service de carnet d’adresses SharePoint pour ajouter la solution des chemins d’apprentissage multilingues. Avec cette option, le modèle SharePoint chemins d’apprentissage est traduit en neuf langues et peut être utilisé avec un minimum de modifications.

> [!IMPORTANT]
> Si vous avez déjà configuré des voies de formation dans votre client, il est recommandé de [mettre à jour](custom_update.md) les voies de formation. Si vous installez une nouvelle instance de voies de formation, vous devrez transférer manuellement toutes les personnalisations du site existant vers le nouveau site. 

## <a name="prerequisites-for-multilingual-support"></a>Conditions requises pour la prise en charge multilingue
 
Pour configurer correctement les voies d’apprentissage de Microsoft 365 avec le service de livres de recherche, la personne qui effectue la mise en service doit répondre aux conditions préalables suivantes : 
 
- Les voies d’apprentissage de mise en service de la personne doivent être un administrateur client du client où les voies d’apprentissage seront mises en service.  
- Un catalogue d’applications client doit être disponible dans l’option apps du centre d’administration SharePoint. Si votre organisation ne dispose pas d’un catalogue d’applications client SharePoint, reportez-vous à la [documentation SharePoint Online](https://docs.microsoft.com/sharepoint/use-app-catalog) pour en créer une. Vous devez attendre au moins deux heures après avoir créé le catalogue d’applications avant de procéder à la mise en service des voies d’apprentissage.  
- La mise en service des chemins d’apprentissage doit être un propriétaire de collection de sites du catalogue d’applications client. Si la personne chargée de la mise en service des chemins d’apprentissage n’est pas un propriétaire de collection de sites du catalogue d’applications, [suivez ces instructions](addappadmin.md) et continuez. 

## <a name="ensure-the-tenant-admin-account-doesnt-have-a-language-selected"></a>Vérifier que la langue du compte d’administrateur client n’est pas sélectionnée
Avant de mettre en service les voies de formation, vérifiez que la langue sélectionnée pour le compte administrateur du client n’est pas sélectionnée. Voici comment vérifier si une langue n’a pas été sélectionnée pour le compte administrateur. 
1.  Avec votre profil d’administrateur Edge, accédez à office.com.
2.  Entrez les informations d’identification de l’utilisateur (le cas échéant).
3.  Dans Microsoft 365, cliquez sur **toutes les applications** > Delve. 
4.  Cliquez **sur**  >  **mettre à jour le profil**.
5.  Faites défiler la page vers le bas et cliquez sur **Comment modifier les paramètres régionaux et linguistiques**.
6.  Cliquez **ici**, puis cliquez sur les ellipses **...**.
7.  Dans **mes langues d’affichage**, **aucune langue n’est sélectionnée**. Si une langue est sélectionnée, désélectionnez-la.

### <a name="to-provision-learning-pathways"></a>Pour mettre en service des chemins d’apprentissage

1. Accédez à la [page des solutions de formation Microsoft 365](https://lookbook.microsoft.com/details/3df8bd55-b872-4c9d-88e3-6b2f05344239).
2. Cliquez sur **Ajouter à votre client**. Si vous n’êtes pas connecté à votre client, le service de mise en service vous demandera vos informations d’identification d’administrateur client. 
3. Dans la boîte de dialogue autorisations demandées, sélectionnez **consentement au nom de votre organisation** , puis sélectionnez **accepter**.

Le service de carnet d’adresses nécessite ces autorisations pour créer le catalogue d’applications client, installer l’application dans le catalogue d’applications client et approvisionner le modèle de site. Il n’y a aucun impact global sur votre client. Ces autorisations sont utilisées de manière explicite pour l’installation de la solution. Vous devez accepter ces autorisations pour poursuivre l’installation.

4. Renseignez les champs de la page informations de mise en service en fonction de votre installation. Au minimum, entrez l’adresse de messagerie à laquelle vous souhaitez obtenir des notifications sur le processus de mise en service et l’URL de destination de votre site à mettre en service.  
> [!NOTE]
> Faites en sorte que l’URL de destination de votre site soit conviviale pour vos employés, par exemple « /sites/MyTraining » ou « /teams/LearnMicrosoft365 ».

![inst_options.png](media/inst_options.png)

6. Cliquez sur **mettre en service** lorsque vous êtes prêt à installer les voies de formation dans votre environnement de client.  Le processus de mise en service peut prendre jusqu’à 15 minutes. Vous serez averti par courrier électronique lorsque le site sera prêt. 

> [!IMPORTANT]
> L’administrateur client qui met en service le site des voies d’apprentissage doit accéder au site, puis ouvrir **CustomLearningAdmin. aspx** pour initialiser les propriétés d’administration des voies d’apprentissage. Pour l’instant, l’administrateur client doit également affecter des propriétaires au site. 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Valider la réussite de la mise en service et initialiser la liste CustomConfig

Lorsque la mise en service est terminée, l’administrateur client qui a configuré le site reçoit un courrier électronique à partir du service de carnet d’adresses. Le courrier électronique contient un lien vers le site. À ce stade, l’administrateur client doit accéder au site en utilisant le lien fourni dans le message électronique et configurer le site pour la première utilisation :

- Accédez à `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`. L’ouverture de **CustomLearningAdmin. aspx** Initialise l’élément de liste **CustomConfig** qui configure les voies de formation pour la première utilisation. Vous devriez voir une page semblable à celle-ci :

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Ajouter des propriétaires au site
En tant qu’administrateur client, il est peu probable que vous soyez la personne qui personnalise le site ; vous devrez donc affecter quelques propriétaires au site. Les propriétaires disposent de privilèges d’administrateur sur le site afin qu’ils puissent modifier les pages du site et repersonnaliser le site. Ils ont également la possibilité de masquer et d’afficher du contenu et de créer une playlist et des sous-catégories personnalisées.  

1. Dans le menu **paramètres** SharePoint, cliquez sur **autorisations de site**.
2. Cliquez sur **paramètres d’autorisation avancés**.
3. Cliquez sur **propriétaires de voies d’apprentissage Microsoft 365**.
4. Cliquez sur **nouveau**  >  **Ajouter des utilisateurs à ce groupe**, puis ajoutez les personnes que vous souhaitez être propriétaires. 
5. Ajoutez un lien pour [Explorer le site](custom_exploresite.md) dans le message de partage, puis cliquez sur **partager**.

## <a name="add-translators-to-the-site"></a>Ajouter des traducteurs au site
Si vous utilisez des traducteurs pour le site, vous pouvez leur attribuer des autorisations. Les traducteurs nécessitent des autorisations de membre ou une version ultérieure. 

## <a name="choose-options-for-using-multiple-languages-on-the-site"></a>Choisir les options d’utilisation de plusieurs langues sur le site
Le service de carnet d’adresses SharePoint crée le site des voies d’apprentissage dans neuf langues. Les recommandations suivantes s’appliquent :
- Désactiver les langues que vous ne voulez pas prendre en charge
- Si vous ne prenez pas en charge un site multilingue, désactivez la fonctionnalité multilingue. Consultez la section « désactiver la prise en charge multilingue » plus loin dans cette rubrique.

### <a name="remove-languages-you-dont-want-to-support"></a>Supprimer les langues que vous ne voulez pas prendre en charge
Pour les organisations qui choisissent de prendre en charge une seule langue, en plus de la langue anglaise par défaut, nous vous recommandons de supprimer les langues qui ne sont pas prises en charge. 
1. Sur le site des voies d’apprentissage, sélectionnez les **paramètres** dans la partie supérieure droite de la page, puis sélectionnez **informations sur le site**.
2. En bas du volet informations sur le site, sélectionnez **Afficher tous les paramètres du site**.
3. Sous **administration du site**, sélectionnez **paramètres de langue**.
4. Sous **activer la traduction des pages et des informations en plusieurs langues**, faites glisser le bouton bascule **sur activé**. Il doit être activé par défaut.
5. Sous ajouter ou supprimer des langues de site, cliquez sur **supprimer** pour supprimer les langues dont vous n’avez pas besoin pour le site. Voici un exemple de la page Paramètres de langue pour afficher l’italien pris en charge pour le site, en plus de la langue par défaut en anglais.

![custom_update_ml_langsettings.png](media/custom_update_ml_langsettings.png)

> [!NOTE]
> Lors de la suppression des langues, vous ne pouvez pas supprimer la langue par défaut de l’anglais. 

### <a name="assign-translators"></a>Affecter des traducteurs
Si vous envisagez de traduire des pages, affectez éventuellement un ou plusieurs traducteurs pour chaque langue (à l’exception de la langue par défaut du site). 
- Dans la colonne **traducteur** , commencez à taper le nom d’une personne comme traducteur, puis sélectionnez le nom dans la liste. 

> [!NOTE]
> Tous les utilisateurs de l’annuaire Active Directory de votre organisation peuvent être affectés en tant que traducteur. Les personnes affectées en tant que traducteurs ne reçoivent pas automatiquement les autorisations appropriées. Quand un utilisateur sans autorisation de modification sur un site tente d’accéder au site, il est dirigé vers une page Web où il peut demander l’accès.

## <a name="turn-off-multilingual-support"></a>Désactiver la prise en charge multilingue
Si vous ne souhaitez pas un site multilingue, par exemple, si vous souhaitez un site en anglais uniquement, il est recommandé de désactiver la fonctionnalité multilingue. 

1. Sur le site des voies d’apprentissage, sélectionnez les **paramètres** dans la partie supérieure droite de la page, puis sélectionnez **informations sur le site**.
2. En bas du volet informations sur le site, sélectionnez **Afficher tous les paramètres du site**.
3. Sous **administration du site**, sélectionnez **paramètres de langue**.
4. Sous **activer la traduction des pages et des informations en plusieurs langues**, faites glisser le bouton bascule **sur activé**. Il doit être activé par défaut.
- Sous **activer la traduction des pages et des news**, sélectionnez **désactivé**. 

### <a name="add-languages"></a>Ajouter des langues
Les voies d’apprentissage prennent en charge 9 langues, mais il est recommandé d’ajouter uniquement les langues que vous devez prendre en charge pour le site des voies d’apprentissage. Vous pouvez ajouter langues à tout moment. 
- Sous **Ajouter ou supprimer des langues de site**, commencez à taper un nom de langue dans **Sélectionner ou tapez une langue**, ou choisissez une langue dans la liste déroulante. Vous pouvez répéter cette étape pour ajouter plusieurs langues. Vous pouvez ajouter ou supprimer des langues de votre site à tout moment en revenant à cette page.