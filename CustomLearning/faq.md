---
author: karuanag
ms.author: karuanag
title: Forum aux questions pour les voies d’apprentissage Microsoft 365
ms.date: 02/10/2019
description: Forum aux questions informations sur les voies d’apprentissage Microsoft 365
ms.openlocfilehash: 26d6c7140b4d387e13b907033ea53b752f5e20ea
ms.sourcegitcommit: 0077704d7edcc26eda76900115716fc5b7b1c518
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/21/2019
ms.locfileid: "34334718"
---
# <a name="frequently-asked-questions"></a>Forum Aux Questions

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>Quelles sont les conditions requises pour l’installation des chemins d’apprentissage Microsoft 365 dans mon environnement de client?

- SharePoint Online et sites de communication activés.
- La personne qui mettra en service CLO365 doit être l’administrateur client du client cible pour l’installation.
- Un client «catalogue d’applications» doit être disponible dans l’option «applications» du centre d’administration SharePoint.
- Si un nouveau catalogue d’applications est créé, une durée d’attente de 30 minutes ou plus est requise pour que le catalogue d’applications soit entièrement approvisionné. Toute tentative de mise en service des chemins d’apprentissage Microsoft 365 directement après la création du catalogue d’applications client entraînera une erreur de mise en service de la solution des voies d’apprentissage. 
- La personne qui mettra en service CLO365 doit être un administrateur de collection de sites du catalogue d’applications dans le client cible pour l’installation.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Pourquoi Microsoft demande-t-il des autorisations client lors de l’installation des chemins d’apprentissage Microsoft 365 

- Le service de mise en service SharePoint Online utilise les autorisations pour mettre en service le site SharePoint des chemins d’apprentissage, créer les pages du site et installer l’application des chemins d’apprentissage Microsoft 365 au sein de leur client. C’est la seule raison pour laquelle nous avons demandé les autorisations. Sans les autorisations demandées, le service de configuration SharePoint ne peut pas exécuter les commandes qui installent automatiquement le modèle de site et le composant WebPart des voies d’apprentissage. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>Quelles sont les implications des chemins d’apprentissage Microsoft 365 dans un aperçu bêta? 

Les chemins d’apprentissage Microsoft 365 sont actuellement en version bêta. Prenez en compte les éléments suivants lorsque vous évaluez, planifiez et implémentez des chemins d’apprentissage Microsoft 365:

- Comme pour toute solution bêta, notre équipe de gestion des services se réserve le droit de modifier le service et ses composants. Dans la mesure où nous résolvons activement les bogues et les problèmes d’expérience utilisateur, il est possible que vous deviez mettre à jour le composant WebPart.
- Pour mettre à jour le composant WebPart, vous devez le télécharger à partir de notre référentiel GitHub et le charger dans votre catalogue d’applications client. Consultez la section «mise à jour de la solution» du fichier [Lisez-moi](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) des chemins d’apprentissage Microsoft 365. 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>Quelles sont les langues disponibles pour les voies d’apprentissage Microsoft 365?

Les chemins d’apprentissage Microsoft 365 sont actuellement disponibles uniquement en anglais. La mise en service automatique de bout en bout ne fonctionne qu’avec les locataires anglais. Nous prévoyons de déployer la prise en charge multilingue pour ces neuf langues dans CY19 Q3: 

- Chinois (simplifié) 
- Néerlandais (Pays-Bas) 
- Français  
- Allemand 
- Italien (Italie) 
- Japonais (Japon)  
- Portugais (Brésil) 
- Russe (russe)  
- Espagnol 

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>Combien de temps faut-il pour installer le site dans notre environnement client?

En fonction de nos tests de l’installation, elle doit prendre moins de 15 minutes. Cela n’inclut pas le temps nécessaire pour personnaliser le site en fonction de vos besoins.

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Est-ce que les chemins d’apprentissage Microsoft 365 une solution open source et quelles en sont les implications?

Les voies d’apprentissage de Microsoft 365 sont une solution OSS (Open Source Software) et, à ce titre, présente un ensemble de avantages et de points à prendre en compte pour le OSS:

#### <a name="benefits"></a>Avantages 
- Les **chemins d’apprentissage Microsoft 365 sont une solution gratuite:** Les clients peuvent installer la solution dans leur client, la personnaliser et la mettre à la disposition des utilisateurs finaux.
- **OSS permet un développement et une collaboration rapides:**  Toutes les solutions open source sont disponibles pour une large communauté de contributeurs.  Microsoft s’engage à cette méthode d’innovation.  Pour garantir que nous offrons une expérience qui présente le plus grand nombre de clients, notre équipe de gestion de service principale se réserve le droit de déterminer les contributions à fusionner dans notre Build officielle.  
- **OSS permet la collaboration avec des partenaires:** Microsoft collabore avec plusieurs partenaires de formation afin de prendre en charge leurs efforts pour les futures extensions et contributions aux voies d’apprentissage de Microsoft 365. Nous fournirons des informations supplémentaires à mesure que ces plans seront finalisés. 
    
#### <a name="implications"></a>Implique
- **OSS n’est pas un produit disponible dans le commerce:** Les produits commerciaux incluent la mise à jour et l’application de correctifs et sont inclus dans les contrats de support payants. Bien que Microsoft propose actuellement de la documentation, la mise à jour et l’application de correctifs pour les chemins d’apprentissage Microsoft 365, il s’appuie sur notre engagement à améliorer ce scénario d’entreprise particulier. Nos plans doivent continuer à investir dans les voies de formation, mais les clients doivent savoir que notre équipe de gestion des services peut modifier les stratégies à l’avenir. Toutes les modifications futures apportées aux chemins d’apprentissage de Microsoft 365 seront communiquées avant de prendre effet. 
- **En tant que OSS, les voies d’apprentissage de microsoft 365 sont prises en charge par le biais d’une liste de problèmes en ligne sur GitHub**: les chemins d’apprentissage Microsoft 365 ne sont pas couverts par les contrats de support technique Microsoft existants. Les problèmes soumis sont triés par les propriétaires de services de la voie de formation Microsoft 365 et par la communauté. Les niveaux de service de résolution des problèmes ne sont pas au même niveau qu’un contrat de support technique Microsoft payant.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>Pouvons-nous faire en sorte que les chemins d’apprentissage Microsoft 365 soient un sous-site de notre collection de sites SharePoint principale?

Non. Le site est basé sur un modèle de site de communication, qui est toujours destiné à être une collection de sites racine.

> [!NOTE]
> Il est important de prendre en compte les autorisations dont les utilisateurs finaux auront besoin pour accéder au site. La plupart des organisations ont des groupes de sécurité ou d’utilisateurs définis. Vous devez ajouter les groupes de sécurité appropriés à votre nouveau portail de formation une fois que vous êtes prêt à le lancer dans votre communauté d’employés.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>J’ai besoin de réinstaller le site; que dois-je faire?

Suivez les instructions d’installation publiées [ici](custom_provision.md).

> [!NOTE]
> Si vous aviez désactivé la télémétrie dans votre installation précédente et souhaitez continuer à désactiver la télémétrie, vous devrez suivre les instructions relatives à la désactivation de la télémétrie ici.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Nous avons apporté des mises à jour à notre implémentation des chemins d’apprentissage Microsoft 365. Seront-nous perdus ces mises à jour (apportées au modèle de site, playlists) si nous réinstallons le site?

Les personnalisations apportées à des pages individuelles et des playlists personnalisées seront perdues si vous réinstallez le site sur votre installation actuelle.  