---
author: karuanag
ms.author: karuanag
title: Forum aux questions sur les solutions de formation personnalisée pour Office 365
ms.date: 02/10/2019
description: Forum aux questions informations sur la formation personnalisée pour Office 365
ms.openlocfilehash: 7da1f3da197fc298c83eac89e3455312cba7a851
ms.sourcegitcommit: c60ca83b784f36b6f41b56ac193f7d58c750984e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/12/2019
ms.locfileid: "30543764"
---
# <a name="frequently-asked-questions"></a>Forum Aux Questions

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a>1. Quelles sont les conditions requises pour l'installation personnalisée de formation pour Office 365 dans mon environnement de client?

- SharePoint Online et sites de communication activés.
- La personne qui mettra en service CLO365 doit être l'administrateur client du client cible pour l'installation.
- Un client «catalogue d'applications» doit être disponible dans l'option «applications» du centre d'administration SharePoint.
- La personne qui mettra en service CLO365 doit être un administrateur de collection de sites du catalogue d'applications dans le client cible pour l'installation.

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a>2. Quelles sont les langues disponibles pour Office 365?

Custom Learning for Office 365 est actuellement disponible uniquement en anglais. La mise en service automatique de bout en bout ne fonctionne qu'avec les locataires anglais. Des langues supplémentaires peuvent être ajoutées dans les versions ultérieures.

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>3. combien de temps faut-il pour installer le site dans notre environnement client?

En fonction de nos tests de l'installation, elle doit prendre moins de 15 minutes. Cela n'inclut pas le temps nécessaire pour personnaliser le site en fonction de vos besoins.

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a>4. pouvons-nous créer une formation personnalisée pour Office 365 d'un sous-site de notre collection de sites SharePoint principale?

Non. Le site est basé sur un modèle de site de communication, qui est toujours destiné à être une collection de sites racine.

> [!NOTE]
> Il est important de prendre en compte les autorisations dont les utilisateurs finaux auront besoin pour accéder au site. La plupart des organisations ont des groupes de sécurité ou d'utilisateurs définis. Vous devez ajouter les groupes de sécurité appropriés à votre nouveau portail de formation une fois que vous êtes prêt à le lancer dans votre communauté d'employés.

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a>5. j'ai besoin de réinstaller le site; que dois-je faire?

Suivez les instructions d'installation publiées [ici](custom_provision.md).

> [!NOTE]
> Si vous aviez désactivé la télémétrie dans votre installation précédente et souhaitez continuer à désactiver la télémétrie, vous devrez suivre les instructions relatives à la désactivation de la télémétrie ici.

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>6. nous avons apporté des mises à jour à notre implémentation de la formation personnalisée pour Office 365. Seront-nous perdus ces mises à jour (apportées au modèle de site, playlists) si nous réinstallons le site?

Les personnalisations apportées à des pages individuelles et des playlists personnalisées seront perdues si vous réinstallez le site sur votre installation actuelle.  