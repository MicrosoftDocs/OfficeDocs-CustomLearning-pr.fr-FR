---
author: pkrebs
ms.author: pkrebs
title: Personnaliser les parcours d’apprentissage
ms.date: 02/18/2019
description: Personnaliser les parcours d’apprentissage
ms.service: sharepoint online
ms.openlocfilehash: 56027e48917cbdeeb2187f87497f3281fff3c23a
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48234226"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="4a86c-103">Personnaliser les parcours d’apprentissage</span><span class="sxs-lookup"><span data-stu-id="4a86c-103">Customize learning pathways</span></span>

<span data-ttu-id="4a86c-104">Les voies d’apprentissage de Microsoft 365 vous permettent de personnaliser le contenu de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="4a86c-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="4a86c-105">Par exemple, vous pouvez :</span><span class="sxs-lookup"><span data-stu-id="4a86c-105">For example, you can:</span></span>  
- <span data-ttu-id="4a86c-106">Modifier le site SharePoint des chemins d’apprentissage : modifiez le nom du site, le logo et les autres.</span><span class="sxs-lookup"><span data-stu-id="4a86c-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="4a86c-107">Modifiez la page poser des questions et obtenir de l’aide pour créer votre propre centre d’aide.</span><span class="sxs-lookup"><span data-stu-id="4a86c-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="4a86c-108">Masquer ou afficher le contenu pour refléter les services ou fonctionnalités pris en charge dans votre organisation</span><span class="sxs-lookup"><span data-stu-id="4a86c-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="4a86c-109">Créer des listes de lecture et des sous-catégories personnalisées conçues spécifiquement pour répondre aux besoins de vos utilisateurs</span><span class="sxs-lookup"><span data-stu-id="4a86c-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="4a86c-110">Créez des pages d’arrivée dont le contenu est filtré pour prendre en charge les résultats de l’entreprise, tels que l’adoption de Microsoft Teams, Outlook Mobile ou collaborer avec Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4a86c-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![cg-introducing.png](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="4a86c-112">Configuration requise et autorisations</span><span class="sxs-lookup"><span data-stu-id="4a86c-112">Requirements and Permissions</span></span>

<span data-ttu-id="4a86c-113">Avant de commencer à utiliser le guide personnaliser les voies d’apprentissage, vérifiez que les voies de formation ont été configurées par votre administrateur client SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4a86c-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="4a86c-114">Si vous ne savez pas si elle a été configurée, contactez votre administrateur client SharePoint pour vérifier que les voies de formation ont été configurées.</span><span class="sxs-lookup"><span data-stu-id="4a86c-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="4a86c-115">Veillez également à obtenir l’URL du site SharePoint des voies d’apprentissage.</span><span class="sxs-lookup"><span data-stu-id="4a86c-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="4a86c-116">Si vous êtes l’administrateur client et que les voies de formation n’ont pas été configurées, consultez la rubrique mise en [service des chemins d’apprentissage](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="4a86c-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="4a86c-117">Autorisations pour mettre en service des chemins d’apprentissage</span><span class="sxs-lookup"><span data-stu-id="4a86c-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="4a86c-118">Administrateur client, également appelé administrateur général Office 365</span><span class="sxs-lookup"><span data-stu-id="4a86c-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="4a86c-119">L’administrateur de collection de sites SharePoint avec des autorisations de Propriétaire sur le site</span><span class="sxs-lookup"><span data-stu-id="4a86c-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="4a86c-120">Autorisations d’utilisation des fonctionnalités d’administration des voies d’apprentissage</span><span class="sxs-lookup"><span data-stu-id="4a86c-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="4a86c-121">Administrateur de collection de sites</span><span class="sxs-lookup"><span data-stu-id="4a86c-121">Site Collection Administrator</span></span>
- <span data-ttu-id="4a86c-122">Autorisations de propriétaire ou de membre SharePoint</span><span class="sxs-lookup"><span data-stu-id="4a86c-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="4a86c-123">Autorisations d’utilisation du site de voies d’apprentissage en tant qu’utilisateur</span><span class="sxs-lookup"><span data-stu-id="4a86c-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="4a86c-124">Autorisations pour les utilisateurs d’Office 365/autorisations pour les visiteurs de site SharePoint ou supérieures</span><span class="sxs-lookup"><span data-stu-id="4a86c-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="4a86c-125">Prise en main de la personnalisation</span><span class="sxs-lookup"><span data-stu-id="4a86c-125">Get started with customization</span></span>
<span data-ttu-id="4a86c-126">Une fois que vous avez vérifié que vous disposez des autorisations nécessaires pour personnaliser le site et le composant WebPart, il est temps de commencer avec le processus de personnalisation.</span><span class="sxs-lookup"><span data-stu-id="4a86c-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="4a86c-127">Pour commencer, consultez [la rubrique accéder au site des voies d’apprentissage](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="4a86c-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>