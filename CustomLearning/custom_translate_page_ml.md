---
author: pkrebs
ms.author: pkrebs
title: Traduire les pages du site
ms.date: 07/06/2020
description: Traduire les pages du site
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: baa46deda7d7e10f3a7655fc6da076d37607e29f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000290"
---
# <a name="translate-site-pages"></a>Traduire les pages du site
Avant de commencer à traduire le site du parcours d'apprentissage, il est important de comprendre quelques concepts clés du fonctionnement de la fonctionnalité multilingue avec les parcours d'apprentissage. 
- Informations sur le site : les traductions de nom de site, de logo et de navigation nécessitent l'affichage et la traduction du site dans le profil linguistique de l'utilisateur.  
- Le volet Web Du parcours d'apprentissage doit être vu avec le profil de langue de l'utilisateur pour qu'il apparaisse dans une langue autre que l'anglais. Le site Web Et le contenu fourni par Microsoft sont déjà traduits pour vous. Pour plus d'informations sur les profils de langues, voir Modifier votre [langue personnelle et les paramètres régionaux.](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7)
- La façon dont vous définissez le parcours d'apprentissage détermine si des pages traduites sont disponibles. Les nouveaux sites mis en service avec le service de carnet d'informations Microsoft 365 disposeront de pages traduites dans neuf langues disponibles. Les sites ou sites mis à jour que vous créez nécessitent une traduction manuelle. Consultez [les options d'installation pour les parcours d'apprentissage multilingues.](custom_setupoptions_ml.md)
- La prise en charge multilingue des parcours d'apprentissage est activée par les fonctionnalités multilingues de SharePoint Online pour les sites de communication. Pour en savoir plus sur les fonctionnalités multilingues de SharePoint Online, voir [Créer des sites de communication multilingues, des pages et des actualités.](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c) 

## <a name="working-with-a-newly-provisioned-site"></a>Working with a newly provisioned site
Si vous avez mis en service un nouveau site de parcours d'apprentissage à partir du service de carnet d'informations Microsoft 365, les pages traduites sont déjà disponibles. Par défaut, le site fournit les pages suivantes :

- Home.aspx
- Start-with-Six-Simple-Steps.aspx
- Get-started-with-Microsoft-365.aspx
- Get-started-with-Microsoft-Teams.aspx
- Get-started-with-SharePoint.aspx
- Get-started-with-OneDriive.aspx
- Ask-questions-and-get-help.aspx
- Événements de formation calendar.aspx
- Become-a-Champion.aspx
- Recommended-Playlists.aspx
- Parcours d'apprentissage Centre de réussite d'administration

## <a name="view-translated-pages-from-the-newly-provisioned-site"></a>Afficher les pages traduites à partir du site nouvellement provisioné
Pour vous familiariser avec le site du parcours d'apprentissage traduit, examinons quelques pages traduites.

### <a name="view-the-translated-home-page"></a>Afficher la page d'accueil traduite
Dans la page d'accueil du parcours d'apprentissage, sélectionnez une langue dans la liste des langues, comme illustré dans l'exemple suivant. Dans l'exemple, l'italien est sélectionné dans le coin supérieur droit et tous les éléments de page sont traduits.

![Photos parcours d'apprentissage utilisés](media/custom_ml_pages_home.png)

### <a name="view-the-translated-microsoft-365-training-page"></a>Afficher la page de formation Microsoft 365 traduite
Examinons maintenant la page de formation Microsoft 365. 

1. Dans la **page** d'accueil du site du parcours d'apprentissage, cliquez sur Formation **Microsoft 365.**
2. Dans le coin supérieur droit de la page, sélectionnez une langue. Dans cet exemple, l'italien est sélectionné.

![Exemple de page de parcours d'apprentissage pour l'italien.](media/custom_ml_pages_training.png)

Quelles traductions sont visibles lorsque la langue est sélectionnée ?
- La page SharePoint est traduite comme illustré dans le graphique ci-dessus. Notez que le texte de la bannière de page est désormais en italien.

Quelles sont les traductions qui ne sont pas visibles ?
- Le nom du site est en anglais
- La navigation du site est en anglais
- Le volet Web du parcours d'apprentissage est en anglais

## <a name="view-the-fully-translated-site"></a>Afficher le site entièrement traduit 
Pour afficher un site entièrement traduit dans une langue spécifique, y compris les pages du site, la navigation et le site Web, la langue personnelle et les paramètres régionaux de l'utilisateur doivent être définies pour cette langue. Pour plus d'informations sur la définition de la langue et des paramètres régionaux, voir Modifier votre [langue personnelle et vos paramètres régionaux.](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7) Il est recommandé d'utiliser un compte distinct ou d'avoir un autre utilisateur avec les différents paramètres de langue pour afficher les pages traduites.  

## <a name="working-with-an-updated-or-manually-installed-learning-pathways-site"></a>Utilisation d'un site de parcours d'apprentissage mis à jour ou installé manuellement
Si vous avez mis à jour un site de parcours d'apprentissage existant ou installé manuellement le site Web Sur un site existant, vous devez traduire manuellement les pages du site. Le contenu et le volet Web du parcours d'apprentissage sont déjà traduits et apparaissent dans la langue préférée de l'utilisateur. Pour traduire des pages, consultez les instructions suivantes « Créer des pages pour les langues que vous souhaitez ». 

## <a name="create-pages-for-the-languages-you-want"></a>Créer des pages pour les langues que vous souhaitez
Une fois que vous avez activé votre site pour les fonctionnalités multilingues et que vous avez choisi les langues que vous souhaitez rendre disponibles, vous pouvez créer les pages de traduction de votre choix. 

1. Go to the default language page you want to make available in another language.
2. Dans la barre supérieure, sélectionnez **Traduction.**
3. Sélectionnez **Créer** pour les langues de votre choix.

> [!IMPORTANT]
> Après avoir créé les pages de traduction, vous devez publier (ou republier) la page de langue par défaut pour vous assurer que :
>- Les pages de traduction sont affichées dans le site de langue correspondant.
>- Les pages de traduction s'affichent correctement dans le composant Web Part Actualités et les composants Web Parts de contenu mis en surbrillant.
>- La liste des langues en haut du site inclut toutes les langues que vous avez activées.
>- Les traducteurs sont avertis de la demande de traduction.

Une fois que vous avez créé la ou les pages, l'état de la page (brouillon enregistré, publié, etc.) s'affiche dans le volet de traduction à côté de chaque langue. En outre, les traducteurs que vous avez affectés seront avertis par courrier électronique qu'une traduction est demandée.

### <a name="view-the-fully-translated-site-in-a-specific-language"></a>Afficher le site entièrement traduit dans une langue spécifique
Pour afficher un site entièrement traduit dans une langue spécifique, y compris les pages du site, la navigation et le site Web, la langue personnelle et les paramètres régionaux de l'utilisateur doivent être définies pour cette langue. Pour plus d'informations sur la définition de la langue et des paramètres régionaux, voir Modifier votre [langue personnelle et vos paramètres régionaux.](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7) Notez qu'il est préférable d'utiliser un compte distinct ou d'avoir un autre utilisateur avec les différents paramètres de langue pour afficher les pages traduites.

## <a name="what-does-a-translator-do"></a>Qu’est-ce qu’un traducteur fait ?
 Une fois le site installé en anglais, un utilisateur ayant l'espagnol comme langue personnelle préférée, par exemple, modifie et traduit manuellement le titre, la navigation et le contenu du pied de page en espagnol. Un utilisateur ayant l’allemand comme langue personnelle par défaut fait de même pour l’allemand. Une fois le contenu traduit, celui-ci s’affiche pour tous les utilisateurs des langues par défaut. Le partie Web Part sélectionne la langue préférée de l'utilisateur et affiche le contenu traduit dans cette langue. 

Les traducteurs traduisent manuellement les copies de la page de langue par défaut dans la ou les langues spécifiées. Lorsque les copies des pages sont créées, les traducteurs sont avertis par courrier électronique si un traducteur a été spécifié. Le message électronique inclut un lien vers la page de langue par défaut et la page de traduction nouvellement créée. Le traducteur :
1. Sélectionnez **le bouton Démarrer la traduction** dans l'e-mail.
2. Sélectionnez **Modifier** en haut à droite de la page et traduisez le contenu.
3. Lorsque vous avez terminé, sélectionnez Enregistrer en tant que brouillon **(si** vous n'êtes pas prêt à le rendre  visible pour les lecteurs) ou si la page est prête à être visible par toutes les personnes qui utilisent cette langue sur le site, sélectionnez Publier ou publier des **actualités.**

Pour plus d'informations sur le processus de traduction, voir Créer des sites de [communication multilingues, des pages et des actualités.](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c) 

## <a name="updating-the-default-language-page"></a>Mise à jour de la page de langue par défaut
Lorsque la page de langue par défaut est mise à jour, la page doit être republiée. Ensuite, les traducteurs des pages de traduction sont avertis par courrier électronique qu'une mise à jour a été réalisée afin que des mises à jour soient mises à jour sur les pages de traduction individuelles.

## <a name="set-up-a-multilingual-site-name-navigation-and-footer"></a>Configurer un nom de site multilingue, la navigation et le pied de liste
Pour afficher le nom du site, la navigation et le pied de page de votre site dans les différentes langues que vous avez mises à disposition, vous devez traduire manuellement chacun d’entre eux.

Par exemple, supposons que vous avez créé un site de communication en anglais comme langue par défaut et que vous avez activé le site pour les langues espagnole et allemande. Lorsque vous créez un site, vous configurez le nom et la description du site dans la langue par défaut (en l’occurrence, l’anglais). Vous pouvez également mettre à jour le nom et la description du site après la création de ce site. Ensuite, vous créez les nœuds de navigation et le contenu du pied de page en anglais.

Une fois le site configuré en anglais, un utilisateur ayant l’espagnol comme langue personnelle par défaut modifie et traduit manuellement le titre, la description, la navigation et le contenu du pied de page en espagnol. Un utilisateur ayant l’allemand comme langue personnelle par défaut fait de même pour l’allemand. Une fois le contenu traduit, celui-ci s’affiche pour tous les utilisateurs des langues par défaut. 

> [! REMARQUES]
>- Les utilisateurs qui traduisent le contenu du site pour leurs langues préférées doivent être membres du groupe Propriétaires du site ou avoir des autorisations de site équivalentes.
>- Si une modification est apporté au nom du site, à la navigation ou au pied de liste dans la langue par défaut, l'élément traduit correspondant dans une autre langue n'est pas automatiquement mis à jour, sauf si vous choisissez de modifier les traductions de site existantes. Dans ce cas, l'élément traduit est remplacé par la mise à jour dans la langue par défaut et doit être traduit manuellement à nouveau. Pour réécrire les traductions, sélectionnez Afficher les paramètres avancés dans la page Langues du site pour la langue par défaut. Ensuite, faites glisser le basculement pour les traductions de overwrite sur On. Cette option ne s'applique pas au contenu de page ou d'actualités.

### <a name="to-view-the-fully-translated-site-in-a-specific-language"></a>Pour afficher le site entièrement traduit dans une langue spécifique
Pour afficher un site entièrement traduit dans une langue spécifique, y compris les pages du site, la navigation et le site Web, la langue personnelle et les paramètres régionaux de l'utilisateur doivent être définies pour cette langue. Pour plus d'informations sur la définition de la langue et des paramètres régionaux, voir Modifier votre [langue personnelle et vos paramètres régionaux.](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7) Il est recommandé d'utiliser un compte distinct ou d'avoir un autre utilisateur avec les différents paramètres de langue pour afficher les pages traduites.

## <a name="for-more-information"></a>Pour plus d’informations
- Pour plus d'informations sur la traduction des pages de site de communication SharePoint, voir Créer des [sites de communication multilingues, des pages et des actualités.](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)
- Pour plus d'informations sur la personnalisation des parcours d'apprentissage, voir [Personnaliser les parcours d'apprentissage.](custom_overview.md)  
