---
author: pkrebs
ms.author: pkrebs
title: Traduire des pages de site
ms.date: 02/10/2019
description: Traduire des pages de site
ms.openlocfilehash: 32dc0928d12074575c8608cef38e4b4d0e5e5cf3
ms.sourcegitcommit: 46caa9fa9d129bee107a8c9a7c5bc70a7f9af087
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2020
ms.locfileid: "44699067"
---
# <a name="translate-site-pages"></a>Traduire des pages de site
Que vous avez mis à jour une version existante des voies d’apprentissage vers la version 4,0 ou que vous avez configuré un nouveau site, le processus de traduction des pages du site est le même. Toutefois, certains éléments doivent être pris en compte. 
- Lorsqu’une nouvelle version 4,0 multilingue est mise en service, les pages du site sont traduites en 9 langues. 
- Lorsque la solution de voies d’apprentissage est mise à jour vers la version multilingue 4,0, les pages de site SharePoint des chemins d’apprentissage demeurent inchangées. Les traductions doivent être réalisées manuellement. 

Le site des voies d’apprentissage, par défaut, fournit les pages suivantes :

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

## <a name="create-pages-for-the-languages-you-want"></a>Créer des pages pour les langues souhaitées
Une fois que vous avez activé votre site pour les fonctionnalités multilingues et que vous avez choisi les langues que vous souhaitez mettre à disposition, vous pouvez créer les pages de traduction de votre choix. Pour vous aider à illustrer certains concepts importants, nous allons utiliser la page de formation Microsoft 365 en guise d’exemple. Pour ce faire :

1.  Sur la page d' **Accueil** des chemins d’apprentissage, cliquez sur **formation Microsoft 365**.  
2.  Dans la barre supérieure, sélectionnez **traduction**.
![custom_update_ml_transbutton.png](media/custom_update_ml_transbutton.png)
3. Si vous souhaitez créer une page pour la traduction dans toutes les langues disponibles pour votre site, sélectionnez **créer pour toutes les langues**. Dans le cas contraire, sélectionnez **créer** uniquement pour les langues de votre choix. Dans cet exemple, nous allons sélectionner italien.
4.  Cliquez sur **Affichage**. La page est maintenant prête pour la traduction. 

### <a name="an-important-concept-to-know"></a>Un concept important à comprendre
Notez que dans l’exemple suivant, la page a été traduite en italien. Toutefois, le titre du site, la navigation et le composant WebPart, apparaissent toujours en anglais. 

![custom_update_ml_transpgconcept.png](media/custom_update_ml_transpgconcept.png)

 Une fois le site configuré en anglais, un utilisateur avec espagnol, par exemple, comme langue personnelle préférée, modifie et traduit le titre, la navigation et le contenu du pied de page en espagnol. Un utilisateur dont la langue personnelle préférée est l’allemand effectue la même opération pour l’allemand. Une fois le contenu traduit, il s’affichera pour tous les utilisateurs de ces langues préférées. Le composant WebPart sélectionne la langue préférée de l’utilisateur et affiche le contenu traduit dans cette langue. 

> [!IMPORTANT]
> Important : une fois que vous avez créé les pages de traduction, vous devez publier (ou republier) la page par défaut de langue anglaise pour vous assurer que :
- Les pages de traduction s’affichent dans le site de langue correspondant.
- Les pages de traduction s’affichent correctement dans le composant WebPart d’actualité et les composants WebPart de contenu mis en surbrillance
- La liste déroulante de langue en haut du site inclut toutes les langues que vous avez activées.
- Les traducteurs sont avertis de la demande de traduction.

## <a name="what-does-a-translator-do"></a>Qu’est-ce qu’un traducteur fait ?
Les traducteurs traduisent manuellement les copies de la page de langue par défaut dans la ou les langues spécifiées. Lorsque les copies de la (des) page (s) sont créées, les traducteurs sont avertis par courrier électronique. Le courrier électronique inclut un lien vers la page langue par défaut et la page traduction nouvellement créée. Le traducteur effectuera les opérations suivantes :
1. Sélectionnez le bouton **lancer la traduction** dans le message électronique.
2. Sélectionnez **modifier** dans la partie supérieure droite de la page, puis traduisez le contenu.
3. Lorsque vous avez terminé, sélectionnez **enregistrer en tant que brouillon** (si vous n’êtes pas prêt à le faire apparaître pour les lecteurs) ou, si la page est prête à être visible par tous les utilisateurs de cette langue sur le site, sélectionnez **publier** ou publier des **News**.

Pour plus d’informations sur le processus de traduction, consultez la rubrique [créer des sites de communication multilingues, des pages et des actualités](https://support.office.com/en-us/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c). 

## <a name="updating-the-default-language-page"></a>Mise à jour de la page de langue par défaut
Lorsque la page langue par défaut est mise à jour, la page doit être republiée. Ensuite, le ou les traducteurs pour les pages de traduction sont avertis par e-mail qu’une mise à jour a été effectuée afin que les mises à jour soient effectuées sur les pages de traduction individuelles.

## <a name="next-steps"></a>Étapes suivantes
- [Traduire des playlists personnalisées](custom_translate_pl_ml.md)
- [Masquer et afficher le contenu multiligual](custom_translate_pl_ml.md)
