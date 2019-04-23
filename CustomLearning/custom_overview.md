---
author: pkrebs
ms.author: pkrebs
title: Información general
ms.date: 02/18/2019
description: Información general sobre aprendizaje personalizado para Office 365 para administradores
ms.openlocfilehash: 6aee3a93a5109b37e43a7118bd98ca31e8b9ac1f
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055650"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="8c393-103">Personalización de la experiencia de aprendizaje</span><span class="sxs-lookup"><span data-stu-id="8c393-103">Customize the Learning Experience</span></span>

<span data-ttu-id="8c393-104">Introducción al aprendizaje personalizado para Office 365, una nueva solución de Microsoft diseñada para acelerar el uso y la adopción de Office 365 dentro de una organización.</span><span class="sxs-lookup"><span data-stu-id="8c393-104">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="8c393-105">Con aprendizaje personalizado, puede:</span><span class="sxs-lookup"><span data-stu-id="8c393-105">With Custom Learning, you can:</span></span>
- <span data-ttu-id="8c393-106">Personalización del contenido de aprendizaje y adopción de Office 365 para su entorno</span><span class="sxs-lookup"><span data-stu-id="8c393-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="8c393-107">Mostrar u ocultar contenido para reflejar los servicios o las características que se admiten en la organización</span><span class="sxs-lookup"><span data-stu-id="8c393-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="8c393-108">Mantener el contenido y los usuarios actualizados con una fuente actualizada de contenido de aprendizaje de Microsoft</span><span class="sxs-lookup"><span data-stu-id="8c393-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="8c393-109">Crear listas de reproducción personalizadas y categorías diseñadas específicamente para las necesidades del usuario</span><span class="sxs-lookup"><span data-stu-id="8c393-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="8c393-111">¿Cómo funciona el aprendizaje personalizado?</span><span class="sxs-lookup"><span data-stu-id="8c393-111">How does Custom Learning work?</span></span>

<span data-ttu-id="8c393-112">Aprendizaje personalizado para Office 365 (aprendizaje personalizado) consta de tres partes:</span><span class="sxs-lookup"><span data-stu-id="8c393-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="8c393-113">una fuente en directo de contenido de un catálogo de Microsoft online</span><span class="sxs-lookup"><span data-stu-id="8c393-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="8c393-114">un sitio de comunicación de SharePoint</span><span class="sxs-lookup"><span data-stu-id="8c393-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="8c393-115">un elemento Web de SharePoint</span><span class="sxs-lookup"><span data-stu-id="8c393-115">a SharePoint web part</span></span> 

![CG-howitworks. png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="8c393-117">Requisitos y permisos</span><span class="sxs-lookup"><span data-stu-id="8c393-117">Requirements and Permissions</span></span>

<span data-ttu-id="8c393-118">Antes de empezar con esta guía, asegúrese de que el administrador de inquilinos de SharePoint haya configurado el aprendizaje personalizado.</span><span class="sxs-lookup"><span data-stu-id="8c393-118">Before getting started with this guide, ensure that Custom Learning has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="8c393-119">Si no está seguro de si se configuró, póngase en contacto con el administrador de inquilinos de SharePoint para comprobar que se ha aprovisionado el aprendizaje personalizado.</span><span class="sxs-lookup"><span data-stu-id="8c393-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been provisioned.</span></span> <span data-ttu-id="8c393-120">Asegúrese también de obtener la dirección URL del sitio de SharePoint de aprendizaje personalizado.</span><span class="sxs-lookup"><span data-stu-id="8c393-120">Also be sure to get the URL of the Custom Learning SharePoint site.</span></span> <span data-ttu-id="8c393-121">Si es el administrador de inquilinos y no se ha aprovisionado el aprendizaje personalizado, vea provision [Custom Learning](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="8c393-121">If you are the Tenant Administrator and Custom Learning has not been provisioned, see [Provision Custom Learning](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-custom-learning"></a><span data-ttu-id="8c393-122">Permisos para aprovisionar aprendizaje personalizado</span><span class="sxs-lookup"><span data-stu-id="8c393-122">Permissions to provision Custom Learning</span></span>

- <span data-ttu-id="8c393-123">Administrador de inquilinos, también conocido como administrador global de Office 365</span><span class="sxs-lookup"><span data-stu-id="8c393-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="8c393-124">Administrador de la colección de sitios de SharePoint con permisos de propietario en el sitio</span><span class="sxs-lookup"><span data-stu-id="8c393-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="8c393-125">Permisos para usar características de administración de aprendizaje personalizadas</span><span class="sxs-lookup"><span data-stu-id="8c393-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="8c393-126">Administrador de colecciones de sitios</span><span class="sxs-lookup"><span data-stu-id="8c393-126">Site Collection Administrator</span></span>
- <span data-ttu-id="8c393-127">Propietario de SharePoint o permisos de miembro</span><span class="sxs-lookup"><span data-stu-id="8c393-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="8c393-128">Permisos para usar el sitio de aprendizaje personalizado como usuario</span><span class="sxs-lookup"><span data-stu-id="8c393-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="8c393-129">Office 365 permisos de usuario/permisos de visitante de sitio de SharePoint o superior</span><span class="sxs-lookup"><span data-stu-id="8c393-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="8c393-130">Introducción a la personalización</span><span class="sxs-lookup"><span data-stu-id="8c393-130">Get started with customization</span></span>
<span data-ttu-id="8c393-131">Una vez que haya asegurado de que dispone de los permisos necesarios para personalizar el sitio y el elemento Web, es el momento de empezar con el proceso de personalización.</span><span class="sxs-lookup"><span data-stu-id="8c393-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="8c393-132">Para empezar, consulte [ir al sitio de aprendizaje personalizado](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="8c393-132">To get started, see [Go to the Custom Learning Site](custom_goto.md).</span></span>