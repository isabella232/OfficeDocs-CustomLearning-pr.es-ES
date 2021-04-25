---
author: pkrebs
ms.author: pkrebs
title: Personalizar las formas de aprendizaje
ms.date: 02/18/2019
manager: bpardi
audience: admin
ms.topic: article
description: Personalizar las formas de aprendizaje
ms.service: sharepoint-online
ms.openlocfilehash: a5087096ec3bd7c1194aab9dd089276fc196a736
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999506"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="aae0a-103">Personalizar las formas de aprendizaje</span><span class="sxs-lookup"><span data-stu-id="aae0a-103">Customize learning pathways</span></span>

<span data-ttu-id="aae0a-104">Las rutas de aprendizaje de Microsoft 365 proporcionan una variedad de formas de personalizar el contenido de su organización.</span><span class="sxs-lookup"><span data-stu-id="aae0a-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="aae0a-105">Por ejemplo, puede:</span><span class="sxs-lookup"><span data-stu-id="aae0a-105">For example, you can:</span></span>  
- <span data-ttu-id="aae0a-106">Modificar las rutas de aprendizaje del sitio de SharePoint: cambie el nombre del sitio, el logotipo y ellos.</span><span class="sxs-lookup"><span data-stu-id="aae0a-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="aae0a-107">Modifique la página Hacer preguntas y obtener ayuda para crear su propio Centro de ayuda.</span><span class="sxs-lookup"><span data-stu-id="aae0a-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="aae0a-108">Ocultar o mostrar contenido para reflejar los servicios o características compatibles con la organización</span><span class="sxs-lookup"><span data-stu-id="aae0a-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="aae0a-109">Crear listas de reproducción personalizadas y subcategorías diseñadas específicamente para las necesidades del usuario</span><span class="sxs-lookup"><span data-stu-id="aae0a-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="aae0a-110">Cree páginas de aterrizaje con contenido filtrado para admitir resultados empresariales, como impulsar la adopción de Microsoft Teams, Outlook mobile o trabajar de forma más colaborativa con Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="aae0a-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![Colección de fotos de caminos de aprendizaje generales de Microsoft.](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="aae0a-112">Requisitos y permisos</span><span class="sxs-lookup"><span data-stu-id="aae0a-112">Requirements and Permissions</span></span>

<span data-ttu-id="aae0a-113">Antes de empezar con la guía Personalizar caminos de aprendizaje, asegúrese de que el administrador de inquilinos de SharePoint haya configurado las rutas de aprendizaje.</span><span class="sxs-lookup"><span data-stu-id="aae0a-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="aae0a-114">Si no está seguro de si se ha configurado, póngase en contacto con el administrador de inquilinos de SharePoint para comprobar que se han aprovisionado las rutas de aprendizaje.</span><span class="sxs-lookup"><span data-stu-id="aae0a-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="aae0a-115">Asegúrese también de obtener la dirección URL del sitio de SharePoint de las rutas de aprendizaje.</span><span class="sxs-lookup"><span data-stu-id="aae0a-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="aae0a-116">Si es el administrador de inquilinos y no se han aprovisionado las rutas de aprendizaje, vea Aprovisionar caminos [de aprendizaje.](custom_provision.md)</span><span class="sxs-lookup"><span data-stu-id="aae0a-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="aae0a-117">Permisos para aprovisionar caminos de aprendizaje</span><span class="sxs-lookup"><span data-stu-id="aae0a-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="aae0a-118">Administrador de inquilinos, también conocido como administrador global de Office 365</span><span class="sxs-lookup"><span data-stu-id="aae0a-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="aae0a-119">Administrador de la colección de sitios de SharePoint con permisos de propietario en el sitio</span><span class="sxs-lookup"><span data-stu-id="aae0a-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="aae0a-120">Permisos para usar las características de administración de caminos de aprendizaje</span><span class="sxs-lookup"><span data-stu-id="aae0a-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="aae0a-121">Administrador de colecciones de sitios</span><span class="sxs-lookup"><span data-stu-id="aae0a-121">Site Collection Administrator</span></span>
- <span data-ttu-id="aae0a-122">Permisos de propietario o miembro de SharePoint</span><span class="sxs-lookup"><span data-stu-id="aae0a-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="aae0a-123">Permisos para usar el sitio de rutas de aprendizaje como usuario</span><span class="sxs-lookup"><span data-stu-id="aae0a-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="aae0a-124">Permisos de usuario de Microsoft Office 365 y permisos de visitante de sitio de SharePoint o superior</span><span class="sxs-lookup"><span data-stu-id="aae0a-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="aae0a-125">Introducción a la personalización</span><span class="sxs-lookup"><span data-stu-id="aae0a-125">Get started with customization</span></span>
<span data-ttu-id="aae0a-126">Una vez que haya asegurado que tiene los permisos necesarios para personalizar el sitio y el elemento web, es el momento de empezar con el proceso de personalización.</span><span class="sxs-lookup"><span data-stu-id="aae0a-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="aae0a-127">Para empezar, vea [Go to the learning pathways site](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="aae0a-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>