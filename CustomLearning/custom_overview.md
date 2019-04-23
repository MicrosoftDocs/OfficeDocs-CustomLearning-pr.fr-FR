---
author: pkrebs
ms.author: pkrebs
title: Vue d’ensemble
ms.date: 02/18/2019
description: Vue d'ensemble de la formation personnalisée pour Office 365 pour les administrateurs
ms.openlocfilehash: 6aee3a93a5109b37e43a7118bd98ca31e8b9ac1f
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055632"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="cdb76-103">Personnaliser l'expérience d'apprentissage</span><span class="sxs-lookup"><span data-stu-id="cdb76-103">Customize the Learning Experience</span></span>

<span data-ttu-id="cdb76-104">INTRODUCTION personnalisée pour Office 365, une nouvelle solution Microsoft conçue pour accélérer l'utilisation et l'adoption d'Office 365 au sein d'une organisation.</span><span class="sxs-lookup"><span data-stu-id="cdb76-104">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="cdb76-105">Grâce à l'apprentissage personnalisé, vous pouvez:</span><span class="sxs-lookup"><span data-stu-id="cdb76-105">With Custom Learning, you can:</span></span>
- <span data-ttu-id="cdb76-106">Personnalisation du contenu d'apprentissage et d'adoption Office 365 pour votre environnement</span><span class="sxs-lookup"><span data-stu-id="cdb76-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="cdb76-107">Masquer ou afficher le contenu pour refléter les services ou fonctionnalités pris en charge dans votre organisation</span><span class="sxs-lookup"><span data-stu-id="cdb76-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="cdb76-108">Mise à jour de votre contenu et de vos utilisateurs avec un flux de mise à jour du contenu de formation de Microsoft</span><span class="sxs-lookup"><span data-stu-id="cdb76-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="cdb76-109">Créer des listes de lecture et des catégories personnalisées conçues spécifiquement pour répondre aux besoins de vos utilisateurs</span><span class="sxs-lookup"><span data-stu-id="cdb76-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="cdb76-111">Comment fonctionne l'apprentissage personnalisé?</span><span class="sxs-lookup"><span data-stu-id="cdb76-111">How does Custom Learning work?</span></span>

<span data-ttu-id="cdb76-112">Custom Learning for Office 365 (formation personnalisée pour Short) se compose de trois parties:</span><span class="sxs-lookup"><span data-stu-id="cdb76-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="cdb76-113">flux de contenu en direct d'un catalogue Microsoft Online</span><span class="sxs-lookup"><span data-stu-id="cdb76-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="cdb76-114">un site de communication SharePoint</span><span class="sxs-lookup"><span data-stu-id="cdb76-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="cdb76-115">un composant WebPart SharePoint</span><span class="sxs-lookup"><span data-stu-id="cdb76-115">a SharePoint web part</span></span> 

![CG-howitworks. png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="cdb76-117">Configuration requise et autorisations</span><span class="sxs-lookup"><span data-stu-id="cdb76-117">Requirements and Permissions</span></span>

<span data-ttu-id="cdb76-118">Avant de commencer à utiliser ce guide, vérifiez que l'apprentissage personnalisé a été configuré par votre administrateur client SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cdb76-118">Before getting started with this guide, ensure that Custom Learning has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="cdb76-119">Si vous ne savez pas si elle a été configurée, contactez votre administrateur client SharePoint pour vérifier que l'apprentissage personnalisé a été mis en service.</span><span class="sxs-lookup"><span data-stu-id="cdb76-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been provisioned.</span></span> <span data-ttu-id="cdb76-120">Assurez-vous également d'obtenir l'URL du site SharePoint de formation personnalisé.</span><span class="sxs-lookup"><span data-stu-id="cdb76-120">Also be sure to get the URL of the Custom Learning SharePoint site.</span></span> <span data-ttu-id="cdb76-121">Si vous êtes l'administrateur client et que l'apprentissage personnalisé n'a pas été mis en service, consultez la rubrique [provision Custom Learning](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="cdb76-121">If you are the Tenant Administrator and Custom Learning has not been provisioned, see [Provision Custom Learning](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-custom-learning"></a><span data-ttu-id="cdb76-122">Autorisations pour mettre en service l'apprentissage personnalisé</span><span class="sxs-lookup"><span data-stu-id="cdb76-122">Permissions to provision Custom Learning</span></span>

- <span data-ttu-id="cdb76-123">Administrateur client, également appelé administrateur général Office 365</span><span class="sxs-lookup"><span data-stu-id="cdb76-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="cdb76-124">Administrateur de collection de sites SharePoint avec des autorisations de propriétaire sur le site</span><span class="sxs-lookup"><span data-stu-id="cdb76-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="cdb76-125">Autorisations d'utilisation des fonctionnalités d'administration de formation personnalisées</span><span class="sxs-lookup"><span data-stu-id="cdb76-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="cdb76-126">Administrateur de collection de sites</span><span class="sxs-lookup"><span data-stu-id="cdb76-126">Site Collection Administrator</span></span>
- <span data-ttu-id="cdb76-127">Autorisations de propriétaire ou de membre SharePoint</span><span class="sxs-lookup"><span data-stu-id="cdb76-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="cdb76-128">Autorisations d'utilisation du site d'apprentissage personnalisé en tant qu'utilisateur</span><span class="sxs-lookup"><span data-stu-id="cdb76-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="cdb76-129">Autorisations utilisateur Office 365/autorisations des visiteurs du site SharePoint ou supérieur</span><span class="sxs-lookup"><span data-stu-id="cdb76-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="cdb76-130">Prise en main de la personnalisation</span><span class="sxs-lookup"><span data-stu-id="cdb76-130">Get started with customization</span></span>
<span data-ttu-id="cdb76-131">Une fois que vous avez vérifié que vous disposez des autorisations nécessaires pour personnaliser le site et le composant WebPart, il est temps de commencer avec le processus de personnalisation.</span><span class="sxs-lookup"><span data-stu-id="cdb76-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="cdb76-132">Pour commencer, consultez [la rubrique accéder au site d'apprentissage personnalisé](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="cdb76-132">To get started, see [Go to the Custom Learning Site](custom_goto.md).</span></span>