---
author: pkrebs
ms.author: pkrebs
title: Mise en service du site d’apprentissage personnalisé
ms.date: 02/10/2019
description: Mettre en service le site d’apprentissage personnalisé pour Office 365 via le moteur d’approvisionnement SharePoint
ms.service: sharepoint online
ms.openlocfilehash: be45ade7588f08801062710d310ca967ddd23926
ms.sourcegitcommit: 907c657e7cc5a4a44d2b9f38cc35fea9ac5c5943
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2021
ms.locfileid: "51162921"
---
# <a name="provision-custom-learning"></a>Mise en service de l’apprentissage personnalisé

Avec le service d’approvisionnement SharePoint Online, un administrateur client Office 365 peut démarrer le processus d’approvisionnement en quelques clics simples. Le service d’approvisionnement est le moyen recommandé pour mettre en service l’apprentissage personnalisé. Il est rapide, facile et ne prend que quelques minutes pour démarrer le processus. Toutefois, avant de commencer à mettre en service le service d’approvisionnement, assurez-vous que vous avez satisfait aux conditions préalables à l’approvisionnement.

## <a name="prerequisites"></a>Conditions préalables
 
Pour configurer l’apprentissage personnalisé avec le service d’approvisionnement [SharePoint Online Provisioning Service,](https://provisioning.sharepointpnp.com)la personne qui a mis en service doit respecter les conditions préalables suivantes : 
 
- La personne qui approvisionnement l’apprentissage personnalisé doit être un administrateur client du client où l’apprentissage personnalisé sera mise en service.  
- Un catalogue d’applications client doit être disponible dans l’option Applications du Centre d’administration SharePoint. Si votre organisation n’a pas de catalogue d’applications client SharePoint, reportez-vous à la [documentation SharePoint Online](/sharepoint/use-app-catalog) pour en créer un.  
- La personne qui approvisionnement l’apprentissage personnalisé doit être propriétaire de collection de sites du catalogue d’applications client. Si la personne qui approvisionnement l’apprentissage personnalisé n’est pas un propriétaire de collection de sites du catalogue d’applications, complétent ces [instructions](addappadmin.md) et poursuivez. 

### <a name="to-provision-custom-learning"></a>Pour mettre en service l’apprentissage personnalisé

1. Go to http://provisioning.sharepointpnp.com and **sign in** from the upper right hand corner of the home page.  Connectez-vous avec les informations d’identification du client ciblé où vous prévoyez d’installer le modèle de site.

![pnphome.png](media/inst_signin.png)

2. Clear the **Consent on behalf of your organization** and select **Accept**.

![dans ](media/inst_perms.png)

3. Sélectionnez **Apprentissage personnalisé pour Office 365 dans** la galerie de solutions.

![dans ](media/inst_select.png)

4. Dans la page d’accueil de la solution, **sélectionnez Ajouter à votre client**

![inst_select.png](media/inst_add.png)

5. Renseignez les champs de la page informations de configuration en fonction de votre installation. Entrez au minimum l’adresse de messagerie dans laquelle vous souhaitez recevoir des notifications sur le processus de mise en service et l’URL de destination de votre site.  
> [!NOTE]
> Rendez l’URL de destination de votre site conviviale pour vos employés, par exemple « /sites/MyTraining » ou « /teams/LearnOffice365 ».

![inst_options.png](media/inst_options.png)

6. Sélectionnez **Provision** lorsque vous êtes prêt à installer l’apprentissage personnalisé dans votre environnement client.  Le processus de mise en service prend jusqu’à 15 minutes. Vous recevrez une notification par courrier électronique (à l’adresse de courrier de notification que vous avez entrée dans la page d’approvisionnement) lorsque le site est prêt à être utilisé.

> [!IMPORTANT]
> L’administrateur client qui propose le site d’apprentissage personnalisé doit se rendre sur le site, puis ouvrir CustomLearningAdmin.aspx pour initialiser les propriétés d’administration de l’apprentissage personnalisé. Pour l’instant, l’administrateur client doit également affecter des propriétaires au site. 

## <a name="validate-provisioning-success"></a>Valider la réussite de l’approvisionnement

Une fois la mise en service terminée, l’administrateur client reçoit un courrier électronique du service d’approvisionnement PnP. L’administrateur peut copier le lien vers le site fourni dans le courrier électronique, puis suivre les instructions pour se rendre sur le site. L’administrateur client peut également accéder <l’URL DE VOTRE-SITE-COLLECTION>/SitePages/CustomLearningAdmin.aspx. Cela initialise l’élément de liste CustomConfig qui définit l’apprentissage personnalisé pour sa première utilisation. La personne qui ouvre cette page pour la première fois doit être un administrateur client, un administrateur de collection de sites ou un propriétaire du site. Vous devriez voir une page qui ressemble à ceci : 

## <a name="add-owners-to-site"></a>Ajouter des propriétaires au site
En tant qu’administrateur client, il est peu probable que vous soyez la personne qui personnalisant le site, vous devrez donc affecter des propriétaires au site. Les propriétaires ont des privilèges d’administration sur le site pour pouvoir modifier les pages du site et renommer le site. Ils ont également la possibilité de masquer et d’afficher le contenu remis via le volet Web d’apprentissage personnalisé. Ils ont également la possibilité de créer une playlist personnalisée et de les affecter à des sous-catégories personnalisées.  

1. Dans le menu **Paramètres** SharePoint, cliquez sur **Autorisations du site.**
2. Cliquez **sur Paramètres d’autorisation avancés.**
3. Cliquez **sur Formation personnalisée pour les propriétaires d’Office 365.**
4. Cliquez **sur Ajouter** des  >  **utilisateurs à ce groupe,** ajoutez les personnes que vous souhaitez être propriétaires, puis cliquez sur **Partager.**

8. Cliquez sur **l’option** Suivante dans le coin supérieur droit de la page pour suivre le site.  

### <a name="next-steps"></a>Étapes suivantes
- Explorez le [contenu par défaut](sitecontent.md) inclus dans le webpart.