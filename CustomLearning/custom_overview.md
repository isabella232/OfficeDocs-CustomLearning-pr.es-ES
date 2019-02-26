---
author: pkrebs
ms.author: pkrebs
title: Información general
ms.date: 02/18/2019
description: Información general sobre aprendizaje personalizado para Office 365 para administradores
ms.openlocfilehash: 98187038b66252523c74d88dd9bfd0f217591bc5
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/25/2019
ms.locfileid: "30087539"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="819d6-103">Personalización de la experiencia de aprendizaje</span><span class="sxs-lookup"><span data-stu-id="819d6-103">Customize the Learning Experience</span></span>

<span data-ttu-id="819d6-p101">Introducción al aprendizaje personalizado para Office 365, una nueva solución de Microsoft diseñada para acelerar el uso y la adopción de Office 365 dentro de una organización. Con aprendizaje personalizado, puede:</span><span class="sxs-lookup"><span data-stu-id="819d6-p101">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization. With Custom Learning, you can:</span></span>
- <span data-ttu-id="819d6-106">Personalización del contenido de aprendizaje y adopción de Office 365 para su entorno</span><span class="sxs-lookup"><span data-stu-id="819d6-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="819d6-107">Mostrar u ocultar contenido para reflejar los servicios o las características que se admiten en la organización</span><span class="sxs-lookup"><span data-stu-id="819d6-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="819d6-108">Mantener el contenido y los usuarios actualizados con una fuente actualizada de contenido de aprendizaje de Microsoft</span><span class="sxs-lookup"><span data-stu-id="819d6-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="819d6-109">Crear listas de reproducción personalizadas y categorías diseñadas específicamente para las necesidades del usuario</span><span class="sxs-lookup"><span data-stu-id="819d6-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="819d6-111">¿Cómo funciona el aprendizaje personalizado?</span><span class="sxs-lookup"><span data-stu-id="819d6-111">How does Custom Learning work?</span></span>

<span data-ttu-id="819d6-112">Aprendizaje personalizado para Office 365 (aprendizaje personalizado) consta de tres partes:</span><span class="sxs-lookup"><span data-stu-id="819d6-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="819d6-113">una fuente en directo de contenido de un catálogo de Microsoft online</span><span class="sxs-lookup"><span data-stu-id="819d6-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="819d6-114">un sitio de comunicación de SharePoint</span><span class="sxs-lookup"><span data-stu-id="819d6-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="819d6-115">un elemento Web de SharePoint</span><span class="sxs-lookup"><span data-stu-id="819d6-115">a SharePoint web part</span></span> 

![CG-howitworks. png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="819d6-117">Requisitos y permisos</span><span class="sxs-lookup"><span data-stu-id="819d6-117">Requirements and Permissions</span></span>

<span data-ttu-id="819d6-p102">Antes de empezar con esta guía, asegúrese de que el administrador de inquilinos de SharePoint haya configurado el aprendizaje personalizado. Si no está seguro de si se configuró, póngase en contacto con el administrador de inquilinos de SharePoint para comprobar que el aprendizaje personalizado se ha instalado. Asegúrese también de obtener la dirección URL del sitio de SharePoint de aprendizaje personalizado. Si usted es el administrador de inquilinos y no se ha instalado aprendizaje personalizado, consulte la guía de instalación de aprendizaje personalizado de Office 365.</span><span class="sxs-lookup"><span data-stu-id="819d6-p102">Before getting started with this guide, ensure that Custom Learning has been set up by your  SharePoint tenant administrator. If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been installed. Also be sure to get the URL of the Custom Learning SharePoint site. If you are the Tenant Administrator and Custom Learning has not been installed, see the Custom Learning for Office 365 Installation Guide.</span></span> 

### <a name="permissions-to-install-custom-learning"></a><span data-ttu-id="819d6-122">Permisos para instalar aprendizaje personalizado</span><span class="sxs-lookup"><span data-stu-id="819d6-122">Permissions to install Custom Learning</span></span>

- <span data-ttu-id="819d6-123">Administrador global de Office 365</span><span class="sxs-lookup"><span data-stu-id="819d6-123">Office 365 Global Administrator</span></span>
- <span data-ttu-id="819d6-124">Administrador de SharePoint</span><span class="sxs-lookup"><span data-stu-id="819d6-124">SharePoint Administrator</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="819d6-125">Permisos para usar características de administración de aprendizaje personalizadas</span><span class="sxs-lookup"><span data-stu-id="819d6-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="819d6-126">Office 365 administrador de SharePoint/permisos de propietario del sitio de SharePoint</span><span class="sxs-lookup"><span data-stu-id="819d6-126">Office 365 SharePoint Administrator/SharePoint Site Owner Permissions</span></span>
- <span data-ttu-id="819d6-127">Permisos de propietario del sitio de SharePoint y administrador de la colección de sitios de SharePoint</span><span class="sxs-lookup"><span data-stu-id="819d6-127">SharePoint Site Collection Administrator/SharePoint Site Owner Permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="819d6-128">Permisos para usar el sitio de aprendizaje personalizado como usuario</span><span class="sxs-lookup"><span data-stu-id="819d6-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="819d6-129">Office 365 permisos de usuario/permisos de visitante de sitio de SharePoint o superior</span><span class="sxs-lookup"><span data-stu-id="819d6-129">Office 365 user permissions/SharePoint Site Visitor Permissions or higher</span></span>


