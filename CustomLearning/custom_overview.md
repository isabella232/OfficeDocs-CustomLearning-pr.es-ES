---
author: pkrebs
ms.author: pkrebs
title: Personalización de caminos de aprendizaje
ms.date: 02/18/2019
description: Personalización de caminos de aprendizaje
ms.openlocfilehash: 15d782455204cf043937bec03041a85abc9e4ee3
ms.sourcegitcommit: 3b8896c81ad2adbcfdbda658482847af5fccb264
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/30/2019
ms.locfileid: "37886643"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="001b0-103">Personalización de caminos de aprendizaje</span><span class="sxs-lookup"><span data-stu-id="001b0-103">Customize learning pathways</span></span>

<span data-ttu-id="001b0-104">Los caminos de aprendizaje de Microsoft 365 proporcionan una variedad de maneras en las que puede personalizar el contenido de su organización.</span><span class="sxs-lookup"><span data-stu-id="001b0-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="001b0-105">Por ejemplo, puede:</span><span class="sxs-lookup"><span data-stu-id="001b0-105">For example, you can:</span></span>  
- <span data-ttu-id="001b0-106">Modifique el sitio de SharePoint de rutas de aprendizaje: cambie el nombre del sitio, el logotipo y los mismos.</span><span class="sxs-lookup"><span data-stu-id="001b0-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="001b0-107">Modifique la página formular preguntas y obtener ayuda para crear su propio centro de ayuda.</span><span class="sxs-lookup"><span data-stu-id="001b0-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="001b0-108">Mostrar u ocultar contenido para reflejar los servicios o las características que se admiten en la organización</span><span class="sxs-lookup"><span data-stu-id="001b0-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="001b0-109">Crear listas de reproducción personalizadas y subcategorías diseñadas específicamente para las necesidades del usuario</span><span class="sxs-lookup"><span data-stu-id="001b0-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="001b0-110">Cree páginas de aterrizaje con contenido filtrado para apoyar resultados empresariales, como impulsar la adopción de Microsoft Teams, Outlook Mobile o trabajar de forma más colaborativa con Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="001b0-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="001b0-112">Requisitos y permisos</span><span class="sxs-lookup"><span data-stu-id="001b0-112">Requirements and Permissions</span></span>

<span data-ttu-id="001b0-113">Antes de empezar con la guía de personalización de las rutas de aprendizaje, asegúrese de que el administrador de inquilinos de SharePoint haya configurado las rutas de aprendizaje.</span><span class="sxs-lookup"><span data-stu-id="001b0-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="001b0-114">Si no está seguro de si se configuró, póngase en contacto con el administrador de inquilinos de SharePoint para comprobar que las rutas de aprendizaje se han aprovisionado.</span><span class="sxs-lookup"><span data-stu-id="001b0-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="001b0-115">Asegúrese también de obtener la dirección URL del sitio de SharePoint de rutas de aprendizaje.</span><span class="sxs-lookup"><span data-stu-id="001b0-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="001b0-116">Si usted es el administrador de inquilinos y no se han aprovisionado los caminos de aprendizaje, consulte [provision Learning Pathways](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="001b0-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="001b0-117">Permisos para aprovisionar rutas de aprendizaje</span><span class="sxs-lookup"><span data-stu-id="001b0-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="001b0-118">Administrador de inquilinos, también conocido como administrador global de Office 365</span><span class="sxs-lookup"><span data-stu-id="001b0-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="001b0-119">Administrador de la colección de sitios de SharePoint con permisos de propietario en el sitio</span><span class="sxs-lookup"><span data-stu-id="001b0-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="001b0-120">Permisos para usar las características de administración de rutas de aprendizaje</span><span class="sxs-lookup"><span data-stu-id="001b0-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="001b0-121">Administrador de colecciones de sitios</span><span class="sxs-lookup"><span data-stu-id="001b0-121">Site Collection Administrator</span></span>
- <span data-ttu-id="001b0-122">Propietario de SharePoint o permisos de miembro</span><span class="sxs-lookup"><span data-stu-id="001b0-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="001b0-123">Permisos para usar el sitio de rutas de aprendizaje como usuario</span><span class="sxs-lookup"><span data-stu-id="001b0-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="001b0-124">Office 365 permisos de usuario/permisos de visitante de sitio de SharePoint o superior</span><span class="sxs-lookup"><span data-stu-id="001b0-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="001b0-125">Introducción a la personalización</span><span class="sxs-lookup"><span data-stu-id="001b0-125">Get started with customization</span></span>
<span data-ttu-id="001b0-126">Una vez que haya asegurado de que dispone de los permisos necesarios para personalizar el sitio y el elemento Web, es el momento de empezar con el proceso de personalización.</span><span class="sxs-lookup"><span data-stu-id="001b0-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="001b0-127">Para empezar, consulte [Go to the Learning Pathways site](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="001b0-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>