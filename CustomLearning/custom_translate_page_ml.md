---
author: pkrebs
ms.author: pkrebs
title: Traduire des pages de site
ms.date: 02/10/2019
description: Traduire des pages de site
ms.openlocfilehash: e26ec272641dc9ce9476e25c56007c76499b626a
ms.sourcegitcommit: 1f080ed4cf3687f922907304db3fd7a06aa9d501
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/02/2020
ms.locfileid: "45031783"
---
# <a name="translate-site-pages"></a>Traduire des pages de site
Avant de commencer à traduire le site des voies d’apprentissage, il est important de comprendre quelques concepts clés relatifs à la manière dont la fonctionnalité multilingue fonctionne avec les voies de formation. 
- Les informations de site : la navigation, le logo et les traductions de noms de sites nécessitent que le site soit affiché dans le profil de langue de l’utilisateur.  
- Le composant WebPart voies d’apprentissage doit être affiché avec le profil de la langue de l’utilisateur pour qu’il apparaisse dans une langue autre que l’anglais. Le composant WebPart et le contenu fourni par Microsoft sont déjà traduits pour vous.
- La méthode que vous avez utilisée pour mettre en service les chemins d’apprentissage détermine si les pages traduites sont déjà disponibles ou si vous devez convertir manuellement les pages. 

## <a name="working-with-a-newly-provisioned-site"></a>Utilisation d’un site nouvellement configuré
Si vous avez configuré un nouveau site de voies d’apprentissage à partir du service de mise en service SharePoint, les pages traduites sont déjà disponibles. Par défaut, le site fournit les pages suivantes :

- Home. aspx
- Start-with-Six-Simple-Steps. aspx
- Get-started-with-Microsoft-365. aspx
- Get-started-with-Microsoft-Teams. aspx
- Get-started-with-SharePoint. aspx
- Get-started-with-OneDriive. aspx
- Ask-Questions-and-Get-Help. aspx
- Événements de formation Calendar. aspx
- Become-a-Champion. aspx
- Recommended-Playlists. aspx
- Centre de réussite d’administration des voies d’apprentissage

## <a name="view-translated-pages-from-the-newly-provisioned-site"></a>Afficher les pages traduites à partir du site nouvellement mis en service
Pour vous familiariser avec le site des voies d’apprentissage traduites, examinons quelques pages traduites.

### <a name="view-the-translated-home-page"></a>Afficher la page d’accueil traduite
À partir de la page d’accueil des chemins d’apprentissage, sélectionnez une langue dans la liste déroulante langue, comme indiqué dans l’exemple suivant. Dans l’exemple, vous voyez l’italien sélectionné dans le coin supérieur droit.

![custom_ml_pages_home.png](media/custom_ml_pages_home.png)

### <a name="view-the-translated-microsoft-365-training-page"></a>Afficher la page de formation traduite Microsoft 365
Pour vous aider à illustrer certains concepts importants, examinons la page formation Microsoft 365. 

1. Sur la page d' **Accueil** du site des voies d’apprentissage, cliquez sur **formation Microsoft 365**.
2. Dans le coin supérieur droit de la page, sélectionnez une langue. Dans cet exemple, italien est sélectionné.

![custom_ml_pages_training.png](media/custom_ml_pages_training.png)

Quelles sont les traductions visibles lorsque la langue est sélectionnée ?
- La page SharePoint est traduite comme indiqué dans le graphique ci-dessus. Notez que le texte de la bannière de page est désormais en italien.

Quelles sont les traductions qui ne sont pas visibles ?
- Le nom du site est en anglais
- La navigation de site est en anglais
- Le composant WebPart voies d’apprentissage est en anglais

## <a name="view-the-fully-translated-site"></a>Afficher le site entièrement traduit 
Pour afficher un site entièrement traduit dans une langue spécifique, y compris les pages de site, la navigation et le composant WebPart, la langue personnelle et les paramètres régionaux de l’utilisateur doivent être définis pour cette langue. Pour plus d’informations sur la définition des paramètres linguistiques et régionaux, voir [modifier vos paramètres régionaux et de langue personnelle](https://support.microsoft.com/en-us/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7). Notez qu’il est préférable d’utiliser un compte distinct ou d’avoir un autre utilisateur disposant des mêmes paramètres de langue pour afficher les pages traduites. 

## <a name="working-with-an-updated-or-manually-installed-learning-pathways-site"></a>Utilisation d’un site de chemins d’apprentissage mis à jour ou installés manuellement
Si vous avez mis à jour un site de voies d’apprentissage existant ou installé manuellement le composant WebPart sur un site existant, vous devrez convertir manuellement les pages du site. Le composant WebPart voies d’apprentissage et le contenu sont déjà traduits et s’affichent dans la langue préférée de l’utilisateur. Pour traduire des pages, consultez les instructions suivantes « créer des pages pour les langues souhaitées ». 

## <a name="create-pages-for-the-languages-you-want"></a>Créer des pages pour les langues souhaitées
Une fois que vous avez activé votre site pour les fonctionnalités multilingues et que vous avez choisi les langues que vous souhaitez mettre à disposition, vous pouvez créer les pages de traduction de votre choix. 

1. Accédez à la page de langue par défaut que vous souhaitez rendre disponible dans une autre langue.
2. Dans la barre supérieure, sélectionnez traduction.
3. Sélectionnez créer pour les langues souhaitées.

> [!IMPORTANT]
> Après avoir créé les pages de traduction, vous devez publier (ou republier) la page langue par défaut pour vous assurer que :
>- Les pages de traduction s’affichent dans le site de langue correspondant.
>- Les pages de traduction s’affichent correctement dans le composant WebPart d’actualité et les composants WebPart de contenu mis en surbrillance
>- La liste déroulante de langue en haut du site inclut toutes les langues que vous avez activées.
>- Les traducteurs sont avertis de la demande de traduction.

Une fois que les pages sont créées, l’état de la page (brouillon enregistré, publié, etc.) est affiché dans le volet traduction en regard de chaque langue. De plus, le ou les traducteurs que vous avez attribués seront avertis par courrier électronique qu’une traduction est demandée.

### <a name="view-the-fully-translated-site-in-a-specific-language"></a>Afficher le site entièrement traduit dans une langue spécifique
Pour afficher un site entièrement traduit dans une langue spécifique, y compris les pages de site, la navigation et le composant WebPart, la langue personnelle et les paramètres régionaux de l’utilisateur doivent être définis pour cette langue. Pour plus d’informations sur la définition des paramètres linguistiques et régionaux, voir [modifier vos paramètres régionaux et de langue personnelle](https://support.microsoft.com/en-us/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7). Notez qu’il est préférable d’utiliser un compte distinct ou d’avoir un autre utilisateur disposant des mêmes paramètres de langue pour afficher les pages traduites.

## <a name="what-does-a-translator-do"></a>Qu’est-ce qu’un traducteur fait ?
 Une fois le site configuré en anglais, un utilisateur avec espagnol, par exemple, comme langue personnelle préférée, modifie et traduit le titre, la navigation et le contenu du pied de page en espagnol. Un utilisateur dont la langue personnelle préférée est l’allemand effectue la même opération pour l’allemand. Une fois le contenu traduit, il s’affichera pour tous les utilisateurs de ces langues préférées. Le composant WebPart sélectionne la langue préférée de l’utilisateur et affiche le contenu traduit dans cette langue. 

Les traducteurs traduisent manuellement les copies de la page de langue par défaut dans la ou les langues spécifiées. Lorsque les copies de la (des) page (s) sont créées, les traducteurs sont avertis par courrier électronique. Le courrier électronique inclut un lien vers la page langue par défaut et la page traduction nouvellement créée. Le traducteur effectuera les opérations suivantes :
1. Sélectionnez le bouton **lancer la traduction** dans le message électronique.
2. Sélectionnez **modifier** dans la partie supérieure droite de la page, puis traduisez le contenu.
3. Lorsque vous avez terminé, sélectionnez **enregistrer en tant que brouillon** (si vous n’êtes pas prêt à le faire apparaître pour les lecteurs) ou, si la page est prête à être visible par tous les utilisateurs de cette langue sur le site, sélectionnez **publier** ou publier des **News**.

Pour plus d’informations sur le processus de traduction, consultez la rubrique [créer des sites de communication multilingues, des pages et des actualités](https://support.office.com/en-us/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c). 

## <a name="updating-the-default-language-page"></a>Mise à jour de la page de langue par défaut
Lorsque la page langue par défaut est mise à jour, la page doit être republiée. Ensuite, le ou les traducteurs pour les pages de traduction sont avertis par e-mail qu’une mise à jour a été effectuée afin que les mises à jour soient effectuées sur les pages de traduction individuelles.

## <a name="set-up-a-multilingual-site-name-navigation-and-footer"></a>Configurer un nom de site multilingue, une navigation et un pied de page
Pour afficher le nom du site, la navigation et le pied de page de votre site dans les différentes langues que vous avez mises à disposition, chacune doit être traduite manuellement.

Par exemple, imaginons que vous avez créé un site de communication avec une langue par défaut de l’anglais et que vous avez activé le site en espagnol et en allemand. Lorsque vous créez un site, vous configurez le nom et la description du site dans la langue par défaut (dans ce cas, l’anglais). Vous pouvez également mettre à jour le nom et la description du site après la création du site. Ensuite, vous créez les nœuds de navigation et le contenu de pied de page en anglais.

Une fois le site configuré en anglais, un utilisateur avec espagnol comme langue personnelle préférée modifie et convertit manuellement le titre, la description, le contenu de navigation et de pied de page en espagnol. Un utilisateur dont la langue personnelle préférée est l’allemand effectue la même opération pour l’allemand. Une fois le contenu traduit, il s’affichera pour tous les utilisateurs de ces langues préférées. 

> [! BÊTE
>- Les utilisateurs qui traduisent le contenu de site pour leurs langues préférées doivent être membres du groupe propriétaires du site ou avoir des autorisations de site équivalentes.
>- Si une modification est apportée au nom du site, à la navigation ou au pied de page dans la langue par défaut, l’élément traduit correspondant dans une autre langue n’est pas automatiquement mis à jour, sauf si vous choisissez de remplacer les traductions de sites existantes. Dans ce cas, l’élément traduit est remplacé par la mise à jour dans la langue par défaut et doit être de nouveau traduit manuellement. Pour remplacer les traductions, accédez à la page langues du site pour la langue par défaut, puis sélectionnez Afficher les paramètres avancés. Ensuite, faites glisser le bouton bascule pour remplacer les traductions sur activé. Cette option ne s’applique pas au contenu de page ou de News.

### <a name="to-view-the-fully-translated-site-in-a-specific-language"></a>Pour afficher le site entièrement traduit dans une langue spécifique
Pour afficher un site entièrement traduit dans une langue spécifique, y compris les pages de site, la navigation et le composant WebPart, la langue personnelle et les paramètres régionaux de l’utilisateur doivent être définis pour cette langue. Pour plus d’informations sur la définition des paramètres linguistiques et régionaux, voir [modifier vos paramètres régionaux et de langue personnelle](https://support.microsoft.com/en-us/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7). Notez qu’il est préférable d’utiliser un compte distinct ou d’avoir un autre utilisateur disposant des mêmes paramètres de langue pour afficher les pages traduites.

## <a name="for-more-information"></a>Pour plus d'informations
- Pour plus d’informations sur la traduction des pages de site de communication SharePoint, consultez la rubrique [créer des sites, des pages et des informations de communication multilingue](https://support.office.com/en-us/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).
- Pour plus d’informations sur la personnalisation des voies de formation, voir [Customize Learning voies](custom_overview.md).  
