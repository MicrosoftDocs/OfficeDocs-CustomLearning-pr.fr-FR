---
author: pkrebs
ms.author: pkrebs
title: Vue d’ensemble
ms.date: 02/15/2019
description: Vue d'ensemble de la formation personnalisée pour Office 365 pour les administrateurs
ms.openlocfilehash: c4b9679ae5a7158306bfd53e345f8e892ab206bc
ms.sourcegitcommit: afb5502604d271f49f6d1133db9dfc499f710eec
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30064984"
---
# <a name="overview-of-custom-learning"></a><span data-ttu-id="540bb-103">Vue d'ensemble de l'apprentissage personnalisé</span><span class="sxs-lookup"><span data-stu-id="540bb-103">Overview of Custom Learning</span></span>
<span data-ttu-id="540bb-p101">INTRODUCTION personnalisée pour Office 365, une nouvelle solution Microsoft conçue pour accélérer l'utilisation et l'adoption d'Office 365 au sein d'une organisation. Grâce à l'apprentissage personnalisé, vous pouvez:</span><span class="sxs-lookup"><span data-stu-id="540bb-p101">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization. With Custom Learning, you can:</span></span>

- <span data-ttu-id="540bb-p102">Personnalisez l'apprentissage personnalisé pour Office 365 dans votre environnement. Modifier les pages de site avec votre marque et logo, des événements de formation et des informations de support technique. Masquer et afficher du contenu pour des services ou des fonctionnalités qui ne sont pas pris en charge dans votre organisation.</span><span class="sxs-lookup"><span data-stu-id="540bb-p102">Tailor Custom Learning for Office 365 to your environment. Modify site pages with your brand and logo, training events, and support info. Hide and show content for services or features that are not supported in your organization.</span></span> 
- <span data-ttu-id="540bb-109">Laissez Microsoft maintenir votre contenu et vos utilisateurs à jour: la formation personnalisée fournit un flux dynamique de contenu d'apprentissage que Microsoft conserve à jour.</span><span class="sxs-lookup"><span data-stu-id="540bb-109">Let Microsoft keep your content and users up-to-date – Custom Learning provides a dynamic feed of learning content that Microsoft keeps up-to-date.</span></span> 
- <span data-ttu-id="540bb-110">Créez des catégories et des playlists personnalisées reflétant les stratégies, les procédures et les cultures de votre organisation, ce qui permet aux utilisateurs de créer des compétences avec du contenu d'apprentissage adapté spécifiquement à leurs besoins.</span><span class="sxs-lookup"><span data-stu-id="540bb-110">Build categories and custom playlists reflecting your organization’s policies, procedures, and culture, enabling users to build skills with learning content crafted specifically to their needs.</span></span>

![cg_introducing. png](media/cg_introducing.png)

## <a name="how-does-custom-learning-word"></a><span data-ttu-id="540bb-112">Comment se comporte-t-il?</span><span class="sxs-lookup"><span data-stu-id="540bb-112">How does Custom Learning word?</span></span>
<span data-ttu-id="540bb-113">Custom Learning for Office 365 (formation personnalisée pour Short) se compose de trois parties:</span><span class="sxs-lookup"><span data-stu-id="540bb-113">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
- <span data-ttu-id="540bb-114">un site de communication SharePoint</span><span class="sxs-lookup"><span data-stu-id="540bb-114">a SharePoint communication site</span></span>
- <span data-ttu-id="540bb-115">un composant WebPart SharePoint</span><span class="sxs-lookup"><span data-stu-id="540bb-115">a SharePoint web part</span></span>
- <span data-ttu-id="540bb-116">flux de contenu en direct d'un catalogue Microsoft Online</span><span class="sxs-lookup"><span data-stu-id="540bb-116">a live feed of content from a Microsoft online catalog</span></span>

![cg_howitworks. png](media/cg_howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="540bb-118">Configuration requise et autorisations</span><span class="sxs-lookup"><span data-stu-id="540bb-118">Requirements and Permissions</span></span>
<span data-ttu-id="540bb-p103">La formation personnalisée pour Office 365 doit être installée par l'administrateur client de votre organisation-personne disposant de l'autorisation d'administrateur client. Avant de commencer à utiliser ces procédures de personnalisation présentées dans ce guide, assurez-vous que l'apprentissage personnalisé a été configuré par un administrateur client SharePoint. Si vous n'êtes pas sûr, contactez votre administrateur client SharePoint pour vérifier que l'apprentissage personnalisé a été installé. Assurez-vous également d'obtenir l'URL du site SharePoint de formation personnalisé. Si vous êtes l'administrateur client et que l'apprentissage personnalisé n'a pas été installé, consultez le Guide d'installation personnalisée pour Office 365.</span><span class="sxs-lookup"><span data-stu-id="540bb-p103">Custom Learning for Office 365 must be installed by your organization’s tenant administrator - someone who has Tenant Administrator permission. Before getting started with this customization procedures covered in this guide, ensure that Custom Learning has been set up by a SharePoint tenant administrator. If you’re not sure, contact your SharePoint tenant administrator to verify that Custom Learning has been installed. Also be sure to get the URL of the Custom Learning SharePoint site. If you are the Tenant Administrator and Custom Learning has not been installed, see the Custom Learning for Office 365 Installation Guide.</span></span> 

### <a name="permissions-required-for-custom-learning"></a><span data-ttu-id="540bb-124">Autorisations requises pour l'apprentissage personnalisé</span><span class="sxs-lookup"><span data-stu-id="540bb-124">Permissions required for Custom Learning</span></span> 
<span data-ttu-id="540bb-125">Voici une répartition des autorisations requises pour l'installation, la personnalisation et l'utilisation d'une formation personnalisée.</span><span class="sxs-lookup"><span data-stu-id="540bb-125">Here’s a breakdown of the permissions required for installing, customizing, and using Custom Learning.</span></span> 

<span data-ttu-id="540bb-126">**Autorisations pour installer l'apprentissage personnalisé**</span><span class="sxs-lookup"><span data-stu-id="540bb-126">**Permissions to install Custom Learning**</span></span>
- <span data-ttu-id="540bb-127">Administrateur général Office 365</span><span class="sxs-lookup"><span data-stu-id="540bb-127">Office 365 Global Administrator</span></span>
- <span data-ttu-id="540bb-128">Administrateur SharePoint</span><span class="sxs-lookup"><span data-stu-id="540bb-128">SharePoint Administrator</span></span>

<span data-ttu-id="540bb-129">**Autorisations d'utilisation des fonctionnalités d'administration de formation personnalisées**</span><span class="sxs-lookup"><span data-stu-id="540bb-129">**Permissions to use Custom Learning Administration features**</span></span>
- <span data-ttu-id="540bb-130">Autorisations du propriétaire de site SharePoint ou de l'administrateur SharePoint Office 365</span><span class="sxs-lookup"><span data-stu-id="540bb-130">Office 365 SharePoint Administrator/SharePoint Site Owner Permissions</span></span>
- <span data-ttu-id="540bb-131">Administrateur de la collection de sites SharePoint/autorisations du propriétaire du site SharePoint</span><span class="sxs-lookup"><span data-stu-id="540bb-131">SharePoint Site Collection Administrator/SharePoint Site Owner Permissions</span></span>

<span data-ttu-id="540bb-132">**Pour utiliser le site de formation personnalisé en tant qu'utilisateur**</span><span class="sxs-lookup"><span data-stu-id="540bb-132">**To use the Custom Learning site as a user**</span></span>
- <span data-ttu-id="540bb-133">Autorisations utilisateur Office 365/autorisations des visiteurs du site SharePoint ou supérieur</span><span class="sxs-lookup"><span data-stu-id="540bb-133">Office 365 user permissions/SharePoint Site Visitor Permissions or higher</span></span>
- <span data-ttu-id="540bb-134">Si vous n'êtes pas certain d'avoir obtenu les autorisations nécessaires, contactez votre administrateur client SharePoint.</span><span class="sxs-lookup"><span data-stu-id="540bb-134">If you’re not sure if you’ve been granted the necessary permissions, contact your SharePoint Tenant Administrator.</span></span>

### <a name="next-steps"></a><span data-ttu-id="540bb-135">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="540bb-135">Next Steps</span></span>

- [<span data-ttu-id="540bb-136">Personnaliser et partager des sélections</span><span class="sxs-lookup"><span data-stu-id="540bb-136">Customize and Share Playlists</span></span>](customplaylist.md)
- [<span data-ttu-id="540bb-137">Adoption des lecteurs</span><span class="sxs-lookup"><span data-stu-id="540bb-137">Drive Adoption</span></span>](driveadoption.md) 