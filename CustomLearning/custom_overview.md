---
author: pkrebs
ms.author: pkrebs
title: Vue d’ensemble
ms.date: 02/18/2019
description: Vue d’ensemble des chemins d’apprentissage Microsoft 365
ms.openlocfilehash: 74fac090177ad8009155e21a977b05ee2b742b3b
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/21/2019
ms.locfileid: "34247845"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="0f1fe-103">Personnaliser l’expérience d’apprentissage</span><span class="sxs-lookup"><span data-stu-id="0f1fe-103">Customize the learning experience</span></span>

<span data-ttu-id="0f1fe-104">Présentation des voies d’apprentissage Microsoft 365, une nouvelle solution Microsoft conçue pour accélérer l’utilisation et l’adoption d’Office 365 au sein d’une organisation.</span><span class="sxs-lookup"><span data-stu-id="0f1fe-104">Introducing Microsoft 365 learning pathways, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="0f1fe-105">Avec Learning pathwyas, vous pouvez :</span><span class="sxs-lookup"><span data-stu-id="0f1fe-105">With learning pathwyas, you can:</span></span>
- <span data-ttu-id="0f1fe-106">Personnalisation du contenu d’apprentissage et d’adoption Microsoft 365 pour votre environnement</span><span class="sxs-lookup"><span data-stu-id="0f1fe-106">Tailor Microsoft 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="0f1fe-107">Masquer ou afficher le contenu pour refléter les services ou fonctionnalités pris en charge dans votre organisation</span><span class="sxs-lookup"><span data-stu-id="0f1fe-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="0f1fe-108">Mise à jour de votre contenu et de vos utilisateurs avec un flux de mise à jour du contenu de formation de Microsoft</span><span class="sxs-lookup"><span data-stu-id="0f1fe-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="0f1fe-109">Créer des listes de lecture et des catégories personnalisées conçues spécifiquement pour répondre aux besoins de vos utilisateurs</span><span class="sxs-lookup"><span data-stu-id="0f1fe-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="how-does-learning-pathways-work"></a><span data-ttu-id="0f1fe-111">Comment fonctionnent les voies d’apprentissage ?</span><span class="sxs-lookup"><span data-stu-id="0f1fe-111">How does learning pathways work?</span></span>

<span data-ttu-id="0f1fe-112">les voies de formation pour Office 365 (voies d’apprentissage pour les courts) se composent de trois parties :</span><span class="sxs-lookup"><span data-stu-id="0f1fe-112">learning pathways for Office 365 (learning pathways for short) consists of three parts:</span></span> 
1. <span data-ttu-id="0f1fe-113">flux de contenu en direct d’un catalogue Microsoft Online</span><span class="sxs-lookup"><span data-stu-id="0f1fe-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="0f1fe-114">un site de communication SharePoint</span><span class="sxs-lookup"><span data-stu-id="0f1fe-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="0f1fe-115">un composant WebPart SharePoint</span><span class="sxs-lookup"><span data-stu-id="0f1fe-115">a SharePoint web part</span></span> 

![CG-howitworks. png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="0f1fe-117">Configuration requise et autorisations</span><span class="sxs-lookup"><span data-stu-id="0f1fe-117">Requirements and Permissions</span></span>

<span data-ttu-id="0f1fe-118">Avant de commencer à utiliser ce guide, assurez-vous que les voies de formation ont été configurées par votre administrateur client SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0f1fe-118">Before getting started with this guide, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="0f1fe-119">Si vous ne savez pas si elle a été configurée, contactez votre administrateur client SharePoint pour vérifier que les voies de formation ont été configurées.</span><span class="sxs-lookup"><span data-stu-id="0f1fe-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="0f1fe-120">Veillez également à obtenir l’URL du site SharePoint des voies d’apprentissage.</span><span class="sxs-lookup"><span data-stu-id="0f1fe-120">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="0f1fe-121">Si vous êtes l’administrateur client et que les voies de formation n’ont pas été configurées, consultez la rubrique mise en [service des chemins d’apprentissage](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="0f1fe-121">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="0f1fe-122">Autorisations pour mettre en service des chemins d’apprentissage</span><span class="sxs-lookup"><span data-stu-id="0f1fe-122">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="0f1fe-123">Administrateur client, également appelé administrateur général Office 365</span><span class="sxs-lookup"><span data-stu-id="0f1fe-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="0f1fe-124">Administrateur de collection de sites SharePoint avec des autorisations de propriétaire sur le site</span><span class="sxs-lookup"><span data-stu-id="0f1fe-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="0f1fe-125">Autorisations d’utilisation des fonctionnalités d’administration des voies d’apprentissage</span><span class="sxs-lookup"><span data-stu-id="0f1fe-125">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="0f1fe-126">Administrateur de collection de sites</span><span class="sxs-lookup"><span data-stu-id="0f1fe-126">Site Collection Administrator</span></span>
- <span data-ttu-id="0f1fe-127">Autorisations de propriétaire ou de membre SharePoint</span><span class="sxs-lookup"><span data-stu-id="0f1fe-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="0f1fe-128">Autorisations d’utilisation du site de voies d’apprentissage en tant qu’utilisateur</span><span class="sxs-lookup"><span data-stu-id="0f1fe-128">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="0f1fe-129">Autorisations utilisateur Office 365/autorisations des visiteurs du site SharePoint ou supérieur</span><span class="sxs-lookup"><span data-stu-id="0f1fe-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="0f1fe-130">Prise en main de la personnalisation</span><span class="sxs-lookup"><span data-stu-id="0f1fe-130">Get started with customization</span></span>
<span data-ttu-id="0f1fe-131">Une fois que vous avez vérifié que vous disposez des autorisations nécessaires pour personnaliser le site et le composant WebPart, il est temps de commencer avec le processus de personnalisation.</span><span class="sxs-lookup"><span data-stu-id="0f1fe-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="0f1fe-132">Pour commencer, consultez [la rubrique accéder au site des voies d’apprentissage](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="0f1fe-132">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>