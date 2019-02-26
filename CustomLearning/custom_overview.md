---
author: pkrebs
ms.author: pkrebs
title: Vue d’ensemble
ms.date: 02/18/2019
description: Vue d'ensemble de la formation personnalisée pour Office 365 pour les administrateurs
ms.openlocfilehash: 98187038b66252523c74d88dd9bfd0f217591bc5
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/25/2019
ms.locfileid: "30087533"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="d5360-103">Personnaliser l'expérience d'apprentissage</span><span class="sxs-lookup"><span data-stu-id="d5360-103">Customize the Learning Experience</span></span>

<span data-ttu-id="d5360-p101">INTRODUCTION personnalisée pour Office 365, une nouvelle solution Microsoft conçue pour accélérer l'utilisation et l'adoption d'Office 365 au sein d'une organisation. Grâce à l'apprentissage personnalisé, vous pouvez:</span><span class="sxs-lookup"><span data-stu-id="d5360-p101">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization. With Custom Learning, you can:</span></span>
- <span data-ttu-id="d5360-106">Personnalisation du contenu d'apprentissage et d'adoption Office 365 pour votre environnement</span><span class="sxs-lookup"><span data-stu-id="d5360-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="d5360-107">Masquer ou afficher le contenu pour refléter les services ou fonctionnalités pris en charge dans votre organisation</span><span class="sxs-lookup"><span data-stu-id="d5360-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="d5360-108">Mise à jour de votre contenu et de vos utilisateurs avec un flux de mise à jour du contenu de formation de Microsoft</span><span class="sxs-lookup"><span data-stu-id="d5360-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="d5360-109">Créer des listes de lecture et des catégories personnalisées conçues spécifiquement pour répondre aux besoins de vos utilisateurs</span><span class="sxs-lookup"><span data-stu-id="d5360-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="d5360-111">Comment fonctionne l'apprentissage personnalisé?</span><span class="sxs-lookup"><span data-stu-id="d5360-111">How does Custom Learning work?</span></span>

<span data-ttu-id="d5360-112">Custom Learning for Office 365 (formation personnalisée pour Short) se compose de trois parties:</span><span class="sxs-lookup"><span data-stu-id="d5360-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="d5360-113">flux de contenu en direct d'un catalogue Microsoft Online</span><span class="sxs-lookup"><span data-stu-id="d5360-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="d5360-114">un site de communication SharePoint</span><span class="sxs-lookup"><span data-stu-id="d5360-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="d5360-115">un composant WebPart SharePoint</span><span class="sxs-lookup"><span data-stu-id="d5360-115">a SharePoint web part</span></span> 

![CG-howitworks. png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="d5360-117">Configuration requise et autorisations</span><span class="sxs-lookup"><span data-stu-id="d5360-117">Requirements and Permissions</span></span>

<span data-ttu-id="d5360-p102">Avant de commencer à utiliser ce guide, vérifiez que l'apprentissage personnalisé a été configuré par votre administrateur client SharePoint. Si vous ne savez pas si elle a été configurée, contactez votre administrateur client SharePoint pour vérifier que l'apprentissage personnalisé a été installé. Assurez-vous également d'obtenir l'URL du site SharePoint de formation personnalisé. Si vous êtes l'administrateur client et que l'apprentissage personnalisé n'a pas été installé, consultez le Guide d'installation personnalisée pour Office 365.</span><span class="sxs-lookup"><span data-stu-id="d5360-p102">Before getting started with this guide, ensure that Custom Learning has been set up by your  SharePoint tenant administrator. If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been installed. Also be sure to get the URL of the Custom Learning SharePoint site. If you are the Tenant Administrator and Custom Learning has not been installed, see the Custom Learning for Office 365 Installation Guide.</span></span> 

### <a name="permissions-to-install-custom-learning"></a><span data-ttu-id="d5360-122">Autorisations pour installer l'apprentissage personnalisé</span><span class="sxs-lookup"><span data-stu-id="d5360-122">Permissions to install Custom Learning</span></span>

- <span data-ttu-id="d5360-123">Administrateur général Office 365</span><span class="sxs-lookup"><span data-stu-id="d5360-123">Office 365 Global Administrator</span></span>
- <span data-ttu-id="d5360-124">Administrateur SharePoint</span><span class="sxs-lookup"><span data-stu-id="d5360-124">SharePoint Administrator</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="d5360-125">Autorisations d'utilisation des fonctionnalités d'administration de formation personnalisées</span><span class="sxs-lookup"><span data-stu-id="d5360-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="d5360-126">Autorisations du propriétaire de site SharePoint ou de l'administrateur SharePoint Office 365</span><span class="sxs-lookup"><span data-stu-id="d5360-126">Office 365 SharePoint Administrator/SharePoint Site Owner Permissions</span></span>
- <span data-ttu-id="d5360-127">Administrateur de la collection de sites SharePoint/autorisations du propriétaire du site SharePoint</span><span class="sxs-lookup"><span data-stu-id="d5360-127">SharePoint Site Collection Administrator/SharePoint Site Owner Permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="d5360-128">Autorisations d'utilisation du site d'apprentissage personnalisé en tant qu'utilisateur</span><span class="sxs-lookup"><span data-stu-id="d5360-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="d5360-129">Autorisations utilisateur Office 365/autorisations des visiteurs du site SharePoint ou supérieur</span><span class="sxs-lookup"><span data-stu-id="d5360-129">Office 365 user permissions/SharePoint Site Visitor Permissions or higher</span></span>


