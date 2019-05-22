---
author: pkrebs
ms.author: pkrebs
title: Approvisionner le site des chemins d’apprentissage Microsoft 365
ms.date: 02/10/2019
description: Approvisionner le site des voies d’apprentissage Microsoft 365 via le service de mise en service SharePoint
ms.openlocfilehash: e48052a395a8669ef684110a1c93409f5859a1d2
ms.sourcegitcommit: 0077704d7edcc26eda76900115716fc5b7b1c518
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/21/2019
ms.locfileid: "34334741"
---
# <a name="provision-microsoft-365-learning-pathways"></a>Mettre en service des chemins d’apprentissage Microsoft 365

Avec le service de mise en service SharePoint Online, un administrateur client Office 365 peut démarrer le processus de mise en service avec quelques clics simples. Le service de mise en service est la méthode recommandée pour mettre en service les voies de formation. Il est rapide, facile et ne prend que quelques minutes pour démarrer le processus. Avant de commencer à utiliser le service de mise en service, assurez-vous que vous avez rempli les conditions préalables pour la mise en service.

> [!IMPORTANT]
> À 5/21/2019, les voies d’apprentissage Microsoft 365 sont le nouveau nom de la solution anciennement appelée formation personnalisée pour Office 365. Si vous avez déjà mis en service une formation personnalisée pour Office 365 dans votre organisation et que vous souhaitez mettre à jour la solution, suivez les instructions «mise à jour de la solution» dans le [fichier Lisez-moi des chemins d’apprentissage Microsoft 365](https://github.com/pnp/custom-learning-office-365). Si vous configurez les voies d’apprentissage de Microsoft 365 pour la première fois, reportez-vous à la rubrique [provision microsoft 365 Learning voies instructions]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision) dans la documentation Microsoft 365 Learning voies.  

## <a name="prerequisites"></a>Conditions préalables
 
Pour configurer les voies d’apprentissage de Microsoft 365 avec le service de mise en service, la personne qui effectue la mise en service doit répondre aux conditions préalables suivantes: 
 
- Les voies d’apprentissage de mise en service de la personne doivent être un administrateur client du client où les voies d’apprentissage seront mises en service.  
- Un catalogue d’applications client doit être disponible dans l’option apps du centre d’administration SharePoint. Si votre organisation ne dispose pas d’un catalogue d’applications client SharePoint, reportez-vous à la [documentation SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) pour en créer une.  
- La mise en service des chemins d’apprentissage doit être un propriétaire de collection de sites du catalogue d’applications client. Si la personne chargée de la mise en service des chemins d’apprentissage n’est pas un propriétaire de collection de sites du catalogue d’applications, [suivez ces instructions](addappadmin.md) et continuez. 

### <a name="to-provision-learning-pathways"></a>Pour mettre en service des chemins d’apprentissage

1. Accédez à http://provisioning.sharepointpnp.com et **Connectez-vous** à partir du coin supérieur droit de la page d’accueil.  Connectez-vous avec les informations d’identification du client ciblé dans lequel vous prévoyez d’installer le modèle de site.

![pnphome. png](media/inst_signin.png)

2. Effacez le **consentement au nom de votre organisation** et sélectionnez **accepter**.

![dans](media/inst_perms.png)

Le service de mise en service requiert ces autorisations pour créer le catalogue d’applications client, installer l’application dans le catalogue d’applications client et approvisionner le modèle de site. Il n’y a pas d’impact global sur votre client et ces autorisations sont utilisées de manière explicite pour l’installation de la solution. Vous devez accepter ces autorisations pour poursuivre l’installation.

3. Faites défiler la page vers le bas, sélectionnez l’onglet **solutions** , puis sélectionnez **voies d’apprentissage pour Office 365**. 

![dans](media/inst_select.png)

4. Sélectionnez **Ajouter à votre client**

![inst_select. png](media/inst_add.png)

5. Renseignez les champs de la page informations de mise en service en fonction de votre installation. Au minimum entrez l’adresse de messagerie à laquelle vous souhaitez obtenir des notifications sur le processus de mise en service et l’URL de destination de votre site à mettre en service.  
> [!NOTE]
> Faites en sorte que l’URL de destination de votre site soit conviviale pour vos employés, par exemple «/sites/MyTraining» ou «/teams/LearnMicrosoft365».

![inst_options. png](media/inst_options.png)

6. Sélectionnez **configuration** lorsque vous êtes prêt à installer les voies de formation dans votre environnement de client.  Le processus de mise en service prendra jusqu’à 15 minutes. Vous serez averti par e-mail (à l’adresse e-mail de notification que vous avez entrée sur la page de mise en service) lorsque le site est prêt pour l’accès. 

> [!IMPORTANT]
> L’administrateur client qui met en service le site des voies d’apprentissage doit accéder au site, puis ouvrir **CustomLearningAdmin. aspx** pour initialiser les propriétés d’administration des voies d’apprentissage. Pour l’instant, l’administrateur client doit également affecter des propriétaires au site. 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Valider la réussite de la mise en service et initialiser la liste CustomConfig

Lorsque la mise en service est terminée, l’administrateur client qui a mis en service le site reçoit un courrier électronique du service de mise en service PnP. Le courrier électronique contient un lien vers le site. À ce stade, l’administrateur client doit accéder au site en utilisant le lien fourni dans le message électronique et configurer le site pour la première utilisation:

- Accédez à `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`. L’ouverture de **CustomLearningAdmin. aspx** Initialise l’élément de liste **CustomConfig** qui configure les voies de formation pour la première utilisation. Vous devriez voir une page semblable à celle-ci:

![CG-adminapppage. png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Ajouter des propriétaires au site
En tant qu’administrateur client, il est peu probable que vous soyez la personne qui personnalise le site; vous devrez donc affecter quelques propriétaires au site. Les propriétaires disposent de privilèges d’administrateur sur le site afin qu’ils puissent modifier les pages du site et repersonnaliser le site. Ils ont également la possibilité de masquer et d’afficher le contenu fourni via le composant WebPart voies d’apprentissage. En outre, ils auront la possibilité de créer une playlist personnalisée et de les affecter à des sous-catégories personnalisées.  

1. Dans le menu **paramètres** SharePoint, cliquez sur **autorisations de site**.
2. Cliquez sur **paramètres d’autorisation avancés**.
3. Cliquez sur **propriétaires de voies d’apprentissage Microsoft 365**.
4. Cliquez sur **nouveau** > **Ajouter des utilisateurs à ce groupe**, puis ajoutez les personnes que vous souhaitez être propriétaires. 
5. Ajoutez un lien pour [Explorer le site](custom_exploresite.md) dans le message de partage, puis cliquez sur **partager**.

### <a name="next-steps"></a>Étapes suivantes
- Explorez le [contenu par défaut](custom_exploresite.md) fourni dans le site et le composant WebPart.
