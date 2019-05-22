---
author: pkrebs
ms.author: pkrebs
title: Options de configuration des chemins d’apprentissage Microsoft 365
ms.date: 02/11/2019
description: Option de configuration de la configuration de formation personnalisée
ms.openlocfilehash: 260480e69188995b46a8d22df305bf68997a921d
ms.sourcegitcommit: 0077704d7edcc26eda76900115716fc5b7b1c518
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/21/2019
ms.locfileid: "34334699"
---
# <a name="learning-pathways-setup-options"></a>Options de configuration des voies d’apprentissage
Les voies de formation permettent de configurer la solution de différentes manières. Les sections suivantes décrivent les options disponibles.

> [!IMPORTANT]
> À 5/21/2019, les voies d’apprentissage Microsoft 365 sont le nouveau nom de la solution anciennement appelée formation personnalisée pour Office 365. Si vous avez déjà mis en service une formation personnalisée pour Office 365 dans votre organisation et que vous souhaitez mettre à jour la solution, suivez les instructions «mise à jour de la solution» dans le [fichier Lisez-moi des chemins d’apprentissage Microsoft 365](https://github.com/pnp/custom-learning-office-365). Si vous configurez les voies d’apprentissage de Microsoft 365 pour la première fois, reportez-vous à la rubrique [provision microsoft 365 Learning voies instructions]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision) dans la documentation Microsoft 365 Learning voies.  


## <a name="recommended---sharepoint-online-provisioning-service-setup"></a>Recommandé: configuration du service de mise en service SharePoint Online 
Le service de mise en service SharePoint Online offre la méthode la plus rapide, la plus facile et recommandée pour la configuration de l’apprentissage personnalisé. Avec le service de mise en service SharePoint Online, un administrateur client Office 365 se connecte au service, effectue quelques choix, puis clique sur **Ajouter au client** pour mettre en service le site de formation personnalisé et le composant WebPart formation personnalisée. Lorsque la mise en service est terminée, l’administrateur de client reçoit un message électronique indiquant que le site est prêt. 

- Pour commencer à utiliser le service de mise en service SharePoint, rendez-vous sur [provision avec le service de mise en service PNP](custom_provision.md) .   

## <a name="stand-alone-learning-pathways-web-part-setup"></a>Configuration autonome des composants WebPart voies d’apprentissage
Pour les organisations qui disposent déjà d’un portail de formation de communication moderne SharePoint Online moderne, les voies d’apprentissage permettent d’installer manuellement le composant WebPart des chemins d’apprentissage Microsoft 365 dans un site SharePoint Online existant. Notez que le site doit être un site SharePoint Online moderne. Cette méthode requiert des autorisations d’administrateur client et une expérience avec Windows PowerShell ou SharePoint Online Management Shell. Notez que cette méthode nécessite une expertise technique plus approfondie, puis la configuration du service de mise en service SharePoint Online.

- Pour obtenir les instructions d’installation manuelle des composants WebPart, consultez [la rubrique installer manuellement le composant WebPart](custom_manualsetup.md). 

## <a name="update-learning-pathways"></a>Mettre à jour les chemins d’apprentissage
Les organisations qui ont utilisé le service de mise en service SharePoint Online pour installer des versions antérieures des voies de formation Microsoft 365, précédemment appelées formation personnalisée pour Office 365, peuvent mettre à jour la solution vers la dernière version. Pour obtenir des instructions sur la manière de vérifier la version déployée par rapport à la version la plus récente de la solution, ainsi que des instructions sur la mise à jour de la solution, consultez la section «mise à jour de la solution» du [fichier Lisez-moi](https://github.com/pnp/custom-learning-office-365/blob/master/README.md).

### <a name="next-steps---provision-microsoft-365-learning-pathwayscustomprovisionmd"></a>Étapes suivantes- [approvisionner les chemins d’apprentissage Microsoft 365](custom_provision.md)
