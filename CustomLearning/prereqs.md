---
author: karuanag
ms.author: karuanag
title: Conditions préalables à l'installation
ms.date: 02/11/2019
description: Décisions et informations prérequises pour l'installation et la configuration de l'apprentissage personnalisé
ms.openlocfilehash: 1a57e8fbecfbce4608c8dcb618f4fdc007467789
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989715"
---
# <a name="getting-started"></a><span data-ttu-id="502f9-103">Mise en route</span><span class="sxs-lookup"><span data-stu-id="502f9-103">Getting Started</span></span>

<span data-ttu-id="502f9-p101">Custom Learning for Office 365 vous permettra de fournir des solutions de formation à la demande pour votre organisation.  Ici, nous aborderons les conditions préalables et les décisions que vous devrez prendre pour un déploiement réussi.</span><span class="sxs-lookup"><span data-stu-id="502f9-p101">Custom Learning for Office 365 will allow you to provide on-demand training solutions for your organization.  Here we will discuss the pre-requisites and decisions you will need to make for a successful deployment.</span></span>

<span data-ttu-id="502f9-p102">Les instructions suivantes décrivent comment configurer l'apprentissage personnalisé pour Office 365 (CLO365), notamment l'installation du modèle de site de communication CLO365 et le composant WebPart formation personnalisée dans votre environnement client. Ces instructions couvrent l'installation de CLO365 via le service SharePoint Online Provisioning ( https://provisioning.sharepointpnp.com en anglais) si vous souhaitez installer uniquement le composant WebPart formation personnalisée à utiliser sur un site de communication SharePoint Online existant, reportez-vous à la rubrique instructions pour l' [installation du composant WebPart personnalisé](installwebpart.md).</span><span class="sxs-lookup"><span data-stu-id="502f9-p102">The following instructions outline how to provision Custom Learning for Office 365 (CLO365), including the installation of the CLO365 communication site template and the Custom Learning web part, into your tenant environment. These instructions cover the installation of CLO365 via the SharePoint Online Provisioning Service at https://provisioning.sharepointpnp.com    If you are interested in installing just the Custom Learning web part for use on an existing SharePoint Online communication site, please refer to the instructions for [installing the custom webpart](installwebpart.md).</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="502f9-108">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="502f9-108">Prerequisites</span></span>
 
<span data-ttu-id="502f9-109">Pour installer correctement CLO365 via le [service de mise en service SharePoint Online](https://provisioning.sharepointpnp.com) , vous devez remplir les conditions préalables suivantes:</span><span class="sxs-lookup"><span data-stu-id="502f9-109">To successfully install CLO365 via the [SharePoint Online Provisioning Service](https://provisioning.sharepointpnp.com) you must meet the following pre-requisites:</span></span> 
 
- <span data-ttu-id="502f9-110">La personne qui mettra en service CLO365 doit être l'administrateur client du client cible pour l'installation.</span><span class="sxs-lookup"><span data-stu-id="502f9-110">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>  
- <span data-ttu-id="502f9-p103">Un client «catalogue d'applications» doit être disponible dans l'option «applications» du centre d'administration SharePoint. Si vous n'avez pas de catalogue d'applications, reportez-vous à la [documentation SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) pour mettre en service cette fonctionnalité.</span><span class="sxs-lookup"><span data-stu-id="502f9-p103">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center. If you do not have an app catalog currently refer to the [SharePoint Online documentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) to provision this feature.</span></span>  
- <span data-ttu-id="502f9-p104">La personne qui mettra en service CLO365 doit être propriétaire de la collection de sites du catalogue d'applications dans le client cible pour l'installation. Si le programme d'installation de CLO365 n'est pas un propriétaire de collection de sites du catalogue d'applications, [suivez ces instructions](addappadmin.md) et continuez.</span><span class="sxs-lookup"><span data-stu-id="502f9-p104">The individual that will be provisioning CLO365 must be a site collection owner of the app catalog in the target tenant for install. If the CLO365 installer is not a site collection owner of the app catalog [complete these instructions](addappadmin.md) and continue.</span></span>  

### <a name="next-steps---service-decisionsservicedecisionsmd"></a><span data-ttu-id="502f9-115">Étapes suivantes- [décisions de service](servicedecisions.md)</span><span class="sxs-lookup"><span data-stu-id="502f9-115">Next Steps - [Service Decisions](servicedecisions.md)</span></span>
