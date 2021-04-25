---
author: pkrebs
ms.author: pkrebs
title: Personnaliser les parcours d’apprentissage
ms.date: 02/18/2019
manager: bpardi
audience: admin
ms.topic: article
description: Personnaliser les parcours d’apprentissage
ms.service: sharepoint-online
ms.openlocfilehash: a5087096ec3bd7c1194aab9dd089276fc196a736
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999500"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="caf03-103">Personnaliser les parcours d’apprentissage</span><span class="sxs-lookup"><span data-stu-id="caf03-103">Customize learning pathways</span></span>

<span data-ttu-id="caf03-104">Les parcours d'apprentissage de Microsoft 365 offrent de nombreuses façons de personnaliser le contenu pour votre organisation.</span><span class="sxs-lookup"><span data-stu-id="caf03-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="caf03-105">Par exemple, vous pouvez :</span><span class="sxs-lookup"><span data-stu-id="caf03-105">For example, you can:</span></span>  
- <span data-ttu-id="caf03-106">Modifiez le site SharePoint du parcours d'apprentissage : modifiez le nom du site, son logo et ses chemins d'accès.</span><span class="sxs-lookup"><span data-stu-id="caf03-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="caf03-107">Modifiez la page Poser des questions et obtenir de l'aide pour créer votre propre Centre d'aide.</span><span class="sxs-lookup"><span data-stu-id="caf03-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="caf03-108">Masquer ou afficher le contenu pour refléter les services ou fonctionnalités pris en charge dans votre organisation</span><span class="sxs-lookup"><span data-stu-id="caf03-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="caf03-109">Créer des playlists et sous-catégories personnalisées conçues spécifiquement pour les besoins de votre utilisateur</span><span class="sxs-lookup"><span data-stu-id="caf03-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="caf03-110">Créez des pages d'accueil avec du contenu filtré pour prendre en charge les résultats de l'entreprise, comme l'adoption de Microsoft Teams, Outlook Mobile ou l'utilisation plus collaborative de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="caf03-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![Collection de photos du parcours d'apprentissage général de Microsoft.](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="caf03-112">Conditions requises et autorisations</span><span class="sxs-lookup"><span data-stu-id="caf03-112">Requirements and Permissions</span></span>

<span data-ttu-id="caf03-113">Avant de commencer à prendre en compte les instructions de personnalisation du parcours d'apprentissage, assurez-vous que le parcours d'apprentissage a été mis en place par votre administrateur client SharePoint.</span><span class="sxs-lookup"><span data-stu-id="caf03-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="caf03-114">Si vous ne savez pas si elle a été définie, contactez votre administrateur client SharePoint pour vérifier que le parcours d'apprentissage a été mis en service.</span><span class="sxs-lookup"><span data-stu-id="caf03-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="caf03-115">Assurez-vous également d'obtenir l'URL du site SharePoint du parcours d'apprentissage.</span><span class="sxs-lookup"><span data-stu-id="caf03-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="caf03-116">Si vous êtes l'administrateur client et que le parcours d'apprentissage n'a pas été mis en service, consultez La mise en service [du parcours d'apprentissage.](custom_provision.md)</span><span class="sxs-lookup"><span data-stu-id="caf03-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="caf03-117">Autorisations de mise en service du parcours d'apprentissage</span><span class="sxs-lookup"><span data-stu-id="caf03-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="caf03-118">Administrateur client, également connu sous le nom d'administrateur général Office 365</span><span class="sxs-lookup"><span data-stu-id="caf03-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="caf03-119">L’administrateur de collection de sites SharePoint avec des autorisations de Propriétaire sur le site</span><span class="sxs-lookup"><span data-stu-id="caf03-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="caf03-120">Autorisations d'utilisation des fonctionnalités d'administration des parcours d'apprentissage</span><span class="sxs-lookup"><span data-stu-id="caf03-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="caf03-121">Administrateur de collection de sites</span><span class="sxs-lookup"><span data-stu-id="caf03-121">Site Collection Administrator</span></span>
- <span data-ttu-id="caf03-122">Autorisations du propriétaire ou du membre SharePoint</span><span class="sxs-lookup"><span data-stu-id="caf03-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="caf03-123">Autorisations d'utiliser le site du parcours d'apprentissage en tant qu'utilisateur</span><span class="sxs-lookup"><span data-stu-id="caf03-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="caf03-124">Autorisations pour les utilisateurs d’Office 365/autorisations pour les visiteurs de site SharePoint ou supérieures</span><span class="sxs-lookup"><span data-stu-id="caf03-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="caf03-125">Prise en main de la personnalisation</span><span class="sxs-lookup"><span data-stu-id="caf03-125">Get started with customization</span></span>
<span data-ttu-id="caf03-126">Une fois que vous avez garanti que vous avez les autorisations nécessaires pour personnaliser le site et le site Web, il est temps de commencer le processus de personnalisation.</span><span class="sxs-lookup"><span data-stu-id="caf03-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="caf03-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="caf03-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>