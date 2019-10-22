---
author: pkrebs
ms.author: pkrebs
title: Información general
ms.date: 02/18/2019
description: Introducción a los caminos de aprendizaje de Microsoft 365
ms.openlocfilehash: 74fac090177ad8009155e21a977b05ee2b742b3b
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/21/2019
ms.locfileid: "34247863"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="86e24-103">Personalización de la experiencia de aprendizaje</span><span class="sxs-lookup"><span data-stu-id="86e24-103">Customize the learning experience</span></span>

<span data-ttu-id="86e24-104">Introducción a los caminos de aprendizaje de Microsoft 365, una nueva solución de Microsoft diseñada para acelerar el uso y la adopción de Office 365 dentro de una organización.</span><span class="sxs-lookup"><span data-stu-id="86e24-104">Introducing Microsoft 365 learning pathways, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="86e24-105">Con Learning pathwyas, puede:</span><span class="sxs-lookup"><span data-stu-id="86e24-105">With learning pathwyas, you can:</span></span>
- <span data-ttu-id="86e24-106">Personalización del contenido de aprendizaje y adopción de Microsoft 365 para su entorno</span><span class="sxs-lookup"><span data-stu-id="86e24-106">Tailor Microsoft 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="86e24-107">Mostrar u ocultar contenido para reflejar los servicios o las características que se admiten en la organización</span><span class="sxs-lookup"><span data-stu-id="86e24-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="86e24-108">Mantener el contenido y los usuarios actualizados con una fuente actualizada de contenido de aprendizaje de Microsoft</span><span class="sxs-lookup"><span data-stu-id="86e24-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="86e24-109">Crear listas de reproducción personalizadas y categorías diseñadas específicamente para las necesidades del usuario</span><span class="sxs-lookup"><span data-stu-id="86e24-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="how-does-learning-pathways-work"></a><span data-ttu-id="86e24-111">¿Cómo funcionan las rutas de aprendizaje?</span><span class="sxs-lookup"><span data-stu-id="86e24-111">How does learning pathways work?</span></span>

<span data-ttu-id="86e24-112">las rutas de aprendizaje para Office 365 (caminos de aprendizaje para abreviar) constan de tres partes:</span><span class="sxs-lookup"><span data-stu-id="86e24-112">learning pathways for Office 365 (learning pathways for short) consists of three parts:</span></span> 
1. <span data-ttu-id="86e24-113">una fuente en directo de contenido de un catálogo de Microsoft online</span><span class="sxs-lookup"><span data-stu-id="86e24-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="86e24-114">un sitio de comunicación de SharePoint</span><span class="sxs-lookup"><span data-stu-id="86e24-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="86e24-115">un elemento Web de SharePoint</span><span class="sxs-lookup"><span data-stu-id="86e24-115">a SharePoint web part</span></span> 

![CG-howitworks. png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="86e24-117">Requisitos y permisos</span><span class="sxs-lookup"><span data-stu-id="86e24-117">Requirements and Permissions</span></span>

<span data-ttu-id="86e24-118">Antes de empezar con esta guía, asegúrese de que el administrador de inquilinos de SharePoint haya configurado las rutas de aprendizaje.</span><span class="sxs-lookup"><span data-stu-id="86e24-118">Before getting started with this guide, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="86e24-119">Si no está seguro de si se configuró, póngase en contacto con el administrador de inquilinos de SharePoint para comprobar que las rutas de aprendizaje se han aprovisionado.</span><span class="sxs-lookup"><span data-stu-id="86e24-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="86e24-120">Asegúrese también de obtener la dirección URL del sitio de SharePoint de rutas de aprendizaje.</span><span class="sxs-lookup"><span data-stu-id="86e24-120">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="86e24-121">Si usted es el administrador de inquilinos y no se han aprovisionado los caminos de aprendizaje, consulte [provision Learning Pathways](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="86e24-121">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="86e24-122">Permisos para aprovisionar rutas de aprendizaje</span><span class="sxs-lookup"><span data-stu-id="86e24-122">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="86e24-123">Administrador de inquilinos, también conocido como administrador global de Office 365</span><span class="sxs-lookup"><span data-stu-id="86e24-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="86e24-124">Administrador de la colección de sitios de SharePoint con permisos de propietario en el sitio</span><span class="sxs-lookup"><span data-stu-id="86e24-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="86e24-125">Permisos para usar las características de administración de rutas de aprendizaje</span><span class="sxs-lookup"><span data-stu-id="86e24-125">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="86e24-126">Administrador de colecciones de sitios</span><span class="sxs-lookup"><span data-stu-id="86e24-126">Site Collection Administrator</span></span>
- <span data-ttu-id="86e24-127">Propietario de SharePoint o permisos de miembro</span><span class="sxs-lookup"><span data-stu-id="86e24-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="86e24-128">Permisos para usar el sitio de rutas de aprendizaje como usuario</span><span class="sxs-lookup"><span data-stu-id="86e24-128">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="86e24-129">Office 365 permisos de usuario/permisos de visitante de sitio de SharePoint o superior</span><span class="sxs-lookup"><span data-stu-id="86e24-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="86e24-130">Introducción a la personalización</span><span class="sxs-lookup"><span data-stu-id="86e24-130">Get started with customization</span></span>
<span data-ttu-id="86e24-131">Una vez que haya asegurado de que dispone de los permisos necesarios para personalizar el sitio y el elemento Web, es el momento de empezar con el proceso de personalización.</span><span class="sxs-lookup"><span data-stu-id="86e24-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="86e24-132">Para empezar, consulte [Go to the Learning Pathways site](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="86e24-132">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>