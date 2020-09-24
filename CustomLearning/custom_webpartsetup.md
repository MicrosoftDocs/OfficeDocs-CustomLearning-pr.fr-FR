---
author: pkrebs
ms.author: pkrebs
title: Mettre en service le site d’apprentissage personnalisé
ms.date: 02/10/2019
description: Mettre en service le site de formation personnalisée pour Office 365 via le moteur de mise en service SharePoint
ms.service: sharepoint online
ms.openlocfilehash: feebef7f351aab4cd1efe7f87596dad98dba7536
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233756"
---
# <a name="provision-custom-learning"></a>Mettre en service une formation personnalisée

Avec le service de mise en service SharePoint Online, un administrateur client Office 365 peut démarrer le processus de mise en service avec quelques clics simples. Le service de mise en service est la méthode recommandée pour mettre en service l’apprentissage personnalisé. Il est rapide, facile et ne prend que quelques minutes pour démarrer le processus. Avant de commencer à utiliser le service de mise en service, assurez-vous que vous avez rempli les conditions préalables pour la mise en service.

## <a name="prerequisites"></a>Conditions préalables
 
Pour configurer correctement l’apprentissage personnalisé avec le [service de mise en service SharePoint Online](https://provisioning.sharepointpnp.com)du service de mise en service, la personne qui effectue la mise en service doit répondre aux conditions préalables suivantes : 
 
- La personne chargée de mettre en service l’apprentissage personnalisé doit être un client Administratorof le client où l’apprentissage personnalisé sera mis en service.  
- Un catalogue d’applications client doit être disponible dans l’option apps du centre d’administration SharePoint. Si votre organisation ne dispose pas d’un catalogue d’applications client SharePoint, reportez-vous à la [documentation SharePoint Online](https://docs.microsoft.com/sharepoint/use-app-catalog) pour en créer une.  
- La personne chargée de mettre en service l’apprentissage personnalisé doit être un propriétaire de collection de sites du catalogue d’applications client. Si la personne chargée de la mise en service de l’apprentissage personnalisé n’est pas un propriétaire de collection de sites du catalogue d’applications, [suivez ces instructions](addappadmin.md) et continuez. 

### <a name="to-provision-custom-learning"></a>Pour configurer l’apprentissage personnalisé

1. Accédez à http://provisioning.sharepointpnp.com et **Connectez-vous** à partir du coin supérieur droit de la page d’accueil.  Connectez-vous avec les informations d’identification du client ciblé dans lequel vous prévoyez d’installer le modèle de site.

![pnphome.png](media/inst_signin.png)

2. Effacez le **consentement au nom de votre organisation** et sélectionnez **accepter**.

![dans](media/inst_perms.png)

3. Sélectionnez **Custom Learning for Office 365** dans la Galerie de solutions.

![dans](media/inst_select.png)

4. Dans la page d’accueil de la solution, sélectionnez **Ajouter à votre client** .

![inst_select.png](media/inst_add.png)

5. Renseignez les champs de la page informations de configuration en fonction de votre installation. Au minimum entrez l’adresse de messagerie à laquelle vous souhaitez obtenir des notifications sur le processus de mise en service et l’URL de destination de votre site à mettre en service.  
> [!NOTE]
> Faites en sorte que l’URL de destination de votre site soit conviviale pour vos employés, par exemple « /sites/MyTraining » ou « /teams/LearnOffice365 ».

![inst_options.png](media/inst_options.png)

6. Sélectionnez **configuration** lorsque vous êtes prêt à installer l’apprentissage personnalisé dans votre environnement de client.  Le processus de mise en service prend jusqu’à 15 minutes. Vous recevrez une notification par courrier électronique (à l’adresse de courrier de notification que vous avez entrée dans la page d’approvisionnement) lorsque le site est prêt à être utilisé.

> [!IMPORTANT]
> L’administrateur client qui met en service le site d’apprentissage personnalisé doit accéder au site, puis ouvrir CustomLearningAdmin. aspx pour initialiser les propriétés personnalisées de l’administrateur pédagogique. Pour l’instant, l’administrateur client doit également affecter des propriétaires au site. 

## <a name="validate-provisioning-success"></a>Valider la réussite de la mise en service

Lorsque la mise en service est terminée, l’administrateur de client reçoit un courrier électronique du service de mise en service PnP. L’administrateur peut copier le lien vers le site fourni dans le courrier électronique, puis suivre les instructions pour accéder au site. L’administrateur client peut également accéder à <votre-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx. Cela initialise l’élément de liste CustomConfig qui configure la formation personnalisée pour sa première utilisation. La personne qui ouvre cette page pour la première fois doit être administrateur client, administrateur de collection de sites ou propriétaire du site. Vous devriez voir une page semblable à celle-ci : 

## <a name="add-owners-to-site"></a>Ajouter des propriétaires au site
En tant qu’administrateur client, il est peu probable que vous soyez la personne qui personnalise le site ; vous devez donc attribuer des propriétaires au site. Les propriétaires disposent de privilèges d’administrateur sur le site afin qu’ils puissent modifier les pages du site et repersonnaliser le site. Ils ont également la possibilité de masquer et d’afficher le contenu fourni par le biais du composant WebPart formation personnalisée. Ils ont également la possibilité de créer une playlist personnalisée et de les affecter à des sous-catégories personnalisées.  

1. Dans le menu **paramètres** SharePoint, cliquez sur **autorisations de site**.
2. Cliquez sur **paramètres d’autorisation avancés**.
3. Cliquez sur **formation personnalisée pour les propriétaires Office 365**.
4. Cliquez sur **nouveau**  >  **Ajouter des utilisateurs à ce groupe**, ajoutez les personnes voulues, puis cliquez sur **partager**.

8. Cliquez sur l’option **suivante** dans le coin supérieur droit de la page pour suivre le site.  

### <a name="next-steps"></a>Étapes suivantes
- Explorez le [contenu par défaut](sitecontent.md) inclus dans le composant WebPart.
