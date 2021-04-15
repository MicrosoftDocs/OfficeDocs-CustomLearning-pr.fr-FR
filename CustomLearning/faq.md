---
title: FAQ sur le parcours d’apprentissage Microsoft 365
author: karuanag
ms.author: karuanag
ms.date: 02/10/2019
ms.topic: article
manager: alexb
audience: itpro
description: Informations fréquemment posées sur le parcours d’apprentissage de Microsoft 365.
ms.service: sharepoint-online
ms.openlocfilehash: f791d6421740c3458be525a7e306b10edab58259
ms.sourcegitcommit: 96ad347dc08694ce2af5a5d42bf1f753d1c30a65
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51749402"
---
# <a name="frequently-asked-questions"></a>Foire aux questions

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>J’ai récemment vu un billet de blog que l’apprentissage personnalisé pour Office 365 est renommé en parcours d’apprentissage Microsoft 365. D’autres modifications sont-elles ajoutées à la solution dans le cadre de l’effort de changement de nom ? Dois-je mettre à jour la solution dans mon organisation ?

La publication du parcours d’apprentissage Microsoft 365 est un effort de changement de nom dédié à la modification du nom de la solution afin de s’aligner sur la marque Microsoft 365. Si vous disposez de l’apprentissage personnalisé pour Office 365 en cours d’exécution dans votre organisation, il n’est pas nécessaire de mettre à jour la solution pour le moment.  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>Quelles sont les conditions requises pour l’installation du parcours d’apprentissage Microsoft 365 dans mon environnement client ?

- SharePoint Online et sites de communication activés.
- La personne qui sera en mesure de mettre en service LE PROGRAMME D’INSTALLATION365 doit être l’administrateur client du client cible pour l’installation.
- Un « catalogue d’applications » client doit être disponible dans l’option « Applications » du Centre d’administration SharePoint.
- Si un nouveau catalogue d’applications est créé, un délai d’attente de 30 minutes ou plus est nécessaire pour que le catalogue d’applications soit entièrement mis en service. Toute tentative de mise en service des parcours d’apprentissage Microsoft 365 directement après la création du catalogue d’applications client entraîne une erreur de mise en service de la solution de parcours d’apprentissage. 
- La personne qui va mettre en service LE PROGRAMME DNS365 doit être un administrateur de collection de sites du catalogue d’applications dans le client cible pour l’installation.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Pourquoi Microsoft demande-t-il des autorisations client lors de l’installation du parcours d’apprentissage microsoft 365 ? 

- Le service d’approvisionnement SharePoint Online utilise les autorisations pour mettre en service le site SharePoint du parcours d’apprentissage, créer les pages du site et installer l’application de parcours d’apprentissage Microsoft 365 au sein de son client. C’est la seule raison pour laquelle nous demandons les autorisations. Sans les autorisations demandées, le service d’approvisionnement SharePoint ne peut pas exécuter les commandes qui installent automatiquement le modèle de site et le volet Web du parcours d’apprentissage. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>Quelles sont les implications du parcours d'apprentissage de Microsoft 365 dans une version bêta ? 

Le parcours d'apprentissage de Microsoft 365 est actuellement en version bêta. Prenez en compte les considérations suivantes lorsque vous évaluez, planifiez et implémentez le parcours d'apprentissage de Microsoft 365 :

- Comme pour toute solution bêta, notre équipe de gestion des services se réserve le droit d'apporter des modifications au service et à ses composants. Comme vous résolvrez activement les bogues et les problèmes d'UX, vous devrez probablement mettre à jour le webpart.
- Pour mettre à jour le site Web Part, vous devez le télécharger à partir de notre référentiel GitHub et le télécharger dans votre catalogue d'applications client. Consultez la section « Mise à jour de la solution » du fichier [Lisez-me](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) du parcours d'apprentissage Microsoft 365. 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>Dans quelles langues le parcours d'apprentissage Microsoft 365 est-il disponible ?

Le parcours d'apprentissage de Microsoft 365 est actuellement disponible uniquement en anglais. L'approvisionnement automatique de bout en bout fonctionne uniquement avec les locataires anglais. Nous prévoyons de déployer la prise en charge multilingue pour les langues suivantes au deuxième trimestre 2020. 

- Chinois (simplifié) 
- Français  
- Allemand 
- Italien (Italie) 
- Japonais (Japon)  
- Portugais (Brésil) 
- Russe (russe)  
- Espagnol 

> La prise en charge du néerlandais ne sera pas incluse dans la prochaine version de la prise en charge multi-langue du parcours d'apprentissage. Nous continuerons à évaluer les nouvelles options linguistiques à l'avenir.

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>Combien de temps faut-il pour installer le site dans notre environnement client ?

En fonction de nos tests de l'installation, cela devrait prendre moins de 15 minutes. Ceci n’inclut pas le temps nécessaire pour personnaliser le site en fonction de vos besoins.

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Le parcours d'apprentissage de Microsoft 365 est-il une solution open source et quelles en sont les implications ?

Le parcours d'apprentissage de Microsoft 365 est une solution de logiciel open source (OSS) qui, en tant que telle, offre un ensemble d'avantages et de considérations qui s'ad communent à OSS :

#### <a name="benefits"></a>Avantages 
- **Le parcours d'apprentissage de Microsoft 365 est une solution gratuite :** Les clients peuvent installer la solution dans leur client, la personnaliser et la mettre à la disposition des utilisateurs finaux
- **OSS permet un développement et une collaboration rapides :**  Toutes les solutions open source sont disponibles pour une large communauté de collaborateurs.  Microsoft s'engage à mettre en place cette méthode d'innovation.  Pour nous assurer que nous apportons une expérience qui bénéficie au plus grand nombre de nos clients, notre équipe de gestion des services de base se réserve le droit de déterminer les contributions qui sont fusionnées dans notre build officiel.  
- **OSS permet la collaboration avec des partenaires :** Microsoft travaille avec plusieurs partenaires d'apprentissage pour soutenir leurs efforts en matière de futurs extensions et contributions au parcours d'apprentissage de Microsoft 365. Nous fournirons plus d'informations à mesure que ces plans seront finalisés. 
    
#### <a name="implications"></a>Implications
- **OSS n'est pas un produit disponible sur le marché :** Les produits commerciaux incluent la mise à jour et l'application de correctifs et sont inclus dans les contrats de support basés sur les frais. Bien que Microsoft propose actuellement de la documentation, des mises à jour et des correctifs pour le parcours d'apprentissage de Microsoft 365, il est basé sur notre engagement à améliorer ce scénario d'entreprise particulier. Nous envisageons de continuer à investir dans le parcours d'apprentissage, sachez que notre équipe de gestion des services peut modifier les stratégies à l'avenir. Toute modification future apportée au parcours d'apprentissage de Microsoft 365 sera communiquée avant de prendre effet. 
- En tant que système d'exploitation, le parcours d'apprentissage **de Microsoft 365** est pris en charge par le biais d'une liste de problèmes en ligne sur GitHub : le parcours d'apprentissage Microsoft 365 n'est couvert par aucun contrat de support Microsoft existant. Les problèmes soumis sont triés par les propriétaires du service du parcours d'apprentissage Microsoft 365 et la communauté. Les niveaux de service de résolution des problèmes ne sont PAS au même niveau qu'un contrat de support Microsoft payant.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>Pouvons-nous faire du parcours d'apprentissage De Microsoft 365 un sous-site de notre collection de sites SharePoint principale ?

Non. Le site est basé sur un modèle de site de communication, qui est toujours destiné à être une collection de sites racine.

> [!NOTE]
> Il est important de prendre en compte les autorisations dont vos utilisateurs finaux auront besoin pour accéder au site. La plupart des organisations ont défini des groupes de sécurité ou des groupes d'utilisateurs. Vous devez ajouter les groupes de sécurité appropriés à votre nouveau portail de formation une fois que vous êtes prêt à le lancer pour votre communauté d'employés.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>Je dois réinstaller le site . Que dois-je faire ?

Suivez les instructions d'installation publiées [ici.](custom_provision.md)

> [!NOTE]
> Si vous avez désactivé la télémétrie dans votre installation précédente et que vous souhaitez continuer avec la télémétrie désactivée, vous devez suivre les instructions de désactivation de la télémétrie ici.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Nous avons mis à jour notre implémentation du parcours d'apprentissage de Microsoft 365. Allons-nous perdre ces mises à jour (mises à jour de modèles de site, playlists) si nous réinstallons le site ?

Les personnalisations des pages individuelles et des playlists personnalisées seront perdues si vous réinstallez le site sur votre installation actuelle.  
