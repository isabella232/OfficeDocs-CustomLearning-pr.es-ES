---
author: karuanag
ms.author: karuanag
title: Instalación del elemento Web de solución de aprendizaje personalizada
ms.date: 02/10/2019
description: Instrucciones de instalación para el elemento Web de solución de aprendizaje personalizada
ms.openlocfilehash: 53229e5b1b8175b06d888091963d1a9f2f0bd361
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989691"
---
# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="36ca1-103">Instalación del elemento Web de solución de aprendizaje personalizada</span><span class="sxs-lookup"><span data-stu-id="36ca1-103">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="36ca1-104">Requisitos previos para una instalación de todo el espacio empresarial</span><span class="sxs-lookup"><span data-stu-id="36ca1-104">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="36ca1-p101">Para instalar el elemento Web de aprendizaje personalizado para todo el espacio empresarial, tendrá que tener permisos administrativos de Office 365.  Si no dispone de estos permisos, puede trabajar con el administrador de Office 365 o instalar el elemento Web para una colección de sitios individual.</span><span class="sxs-lookup"><span data-stu-id="36ca1-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="36ca1-107">Usted o el administrador de Office 365 debe tener la instalación y configurar un [Catálogo de aplicaciones](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) para todo el inquilino o un catálogo de aplicaciones de [colección de sitios](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)para recibir el elemento Web.]</span><span class="sxs-lookup"><span data-stu-id="36ca1-107">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="36ca1-p102">Solo admitimos SharePoint Online. El elemento Web no es compatible con la instalación en ninguna versión de SharePoint local.</span><span class="sxs-lookup"><span data-stu-id="36ca1-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="36ca1-110">Agregar el elemento Web de aprendizaje personalizado al espacio empresarial</span><span class="sxs-lookup"><span data-stu-id="36ca1-110">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="36ca1-p103">Descargue el elemento Web de aprendizaje personalizado y guárdelo en su unidad local.  Este archivo se denomina "MS-Custom-Learning. sppkg".  No cambie el nombre o el sufijo del archivo.</span><span class="sxs-lookup"><span data-stu-id="36ca1-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="36ca1-114">Vaya al [portal de administración de Office 365](https://admin.microsoft.com/AdminPortal/Home#/homepage) para su espacio empresarial</span><span class="sxs-lookup"><span data-stu-id="36ca1-114">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="36ca1-p104">En el panel de navegación izquierdo, seleccione centros de administración, SharePoint. Se abrirá en una nueva pestaña., en el centro de administración de SharePoint, seleccione aplicaciones, catálogo de aplicaciones, aplicaciones para SharePoint</span><span class="sxs-lookup"><span data-stu-id="36ca1-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="36ca1-117">Seleccione cargar el elemento Web y elija el archivo "MS-Custom-Learning. sppkg" que ha descargado.</span><span class="sxs-lookup"><span data-stu-id="36ca1-117">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="36ca1-118">Para esta instalación de todo el espacio empresarial, marque la casilla que hay junto a "hacer que esta solución esté disponible en todos los de la organización".</span><span class="sxs-lookup"><span data-stu-id="36ca1-118">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  
 
> [!NOTE]
> <span data-ttu-id="36ca1-p105">Una vez instalado el elemento Web, lo encontrará en la galería de elementos Web en SharePoint Online.  **En la galería, el elemento Web se denomina "aprendizaje de Microsoft"**</span><span class="sxs-lookup"><span data-stu-id="36ca1-p105">Once the webpart is installed you will find it in your webpart gallery in SharePoint Online.  **In the gallery the webpart is named "Microsoft Learning"**</span></span>

![Implementar solución](media/trustapp_sm.png)


## <a name="add-the-microsoft-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="36ca1-122">Agregar el elemento Web de Microsoft Learning a una página de SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="36ca1-122">Add the Microsoft Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="36ca1-p106">Una vez instalado aprendizaje personalizado en el espacio empresarial, puede Agregar el elemento Web a una página de SharePoint. Cuando se hace que el aprendizaje de Office 365 y Windows 10 esté disponible en el sitio.</span><span class="sxs-lookup"><span data-stu-id="36ca1-p106">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do Office 365 and Windows 10 training is available to your site.</span></span>

1. <span data-ttu-id="36ca1-125">Agregue el elemento Web de aprendizaje personalizado en un diseño de columna de ancho completo:</span><span class="sxs-lookup"><span data-stu-id="36ca1-125">Add the Custom Learning webpart in a full width column layout:</span></span>

![Diseño de página de SharePoint](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="36ca1-p107">En la página de SharePoint, seleccione Agregar sección y, a continuación, seleccione columna de ancho completo.  Verá el siguiente mensaje:</span><span class="sxs-lookup"><span data-stu-id="36ca1-p107">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="36ca1-p108">Seleccione Microsoft Learning.  Ahora debería ver lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="36ca1-p108">Select Microsoft Learning.  You should now see the following:</span></span> 

![Elemento Web de aprendizaje personalizado](media/clo365addwebpart.png)

 <span data-ttu-id="36ca1-133">Ahora puede hacer clic en los mosaicos para explorar el contenido predeterminado incluido en la solución.</span><span class="sxs-lookup"><span data-stu-id="36ca1-133">You can now click on the tiles to explore the default content included in the solution.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="36ca1-134">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="36ca1-134">Next Steps</span></span>
- <span data-ttu-id="36ca1-135">Explore el [contenido predeterminado](webpartcontent.md) incluido en el elemento Web.</span><span class="sxs-lookup"><span data-stu-id="36ca1-135">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="36ca1-136">[Personalice](customization.md) la experiencia de aprendizaje para su organización.</span><span class="sxs-lookup"><span data-stu-id="36ca1-136">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="36ca1-137">[Impulsar la adopción](driveadoption.md) de la solución de formación.</span><span class="sxs-lookup"><span data-stu-id="36ca1-137">[Drive adoption](driveadoption.md) of your training solution.</span></span>

