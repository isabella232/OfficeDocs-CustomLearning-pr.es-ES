---
author: pkrebs
ms.author: pkrebs
title: Crear páginas de SharePoint para listas de reproducción
ms.date: 02/10/2019
description: Crear páginas de SharePoint para listas de reproducción
ms.service: sharepoint online
ms.openlocfilehash: 99425b9be685a8090394ecb446a7c82dee24fe5d
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/23/2020
ms.locfileid: "48234512"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="d1849-103">Crear páginas de SharePoint para listas de reproducción personalizadas</span><span class="sxs-lookup"><span data-stu-id="d1849-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="d1849-104">Una de las características únicas de las rutas de aprendizaje es la capacidad de crear listas de reproducción que se ensamblan a partir de activos de Microsoft y de los activos de SharePoint que se crean.</span><span class="sxs-lookup"><span data-stu-id="d1849-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="d1849-105">En este ejemplo, crearemos una página de SharePoint antes de crear una lista de reproducción.</span><span class="sxs-lookup"><span data-stu-id="d1849-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="d1849-106">La capacidad de crear listas de reproducción desde páginas de SharePoint ofrece varias oportunidades para crear páginas con los elementos Web disponibles en Microsoft o en su organización.</span><span class="sxs-lookup"><span data-stu-id="d1849-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="d1849-107">Por ejemplo, una lista de reproducción puede incluir una página de SharePoint con vídeos incrustados de YouTube, o un formulario creado a partir de formularios de Office 365, o un informe de Power BI incrustado.</span><span class="sxs-lookup"><span data-stu-id="d1849-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="d1849-108">En este ejemplo, le mostraremos cómo crear una página con el elemento Web insertar y el elemento Web texto.</span><span class="sxs-lookup"><span data-stu-id="d1849-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="d1849-109">Crear una página de SharePoint para una lista de reproducción personalizada</span><span class="sxs-lookup"><span data-stu-id="d1849-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="d1849-110">Haga clic en el icono de **engranaje** de SharePoint y, a continuación, haga clic en **Agregar una página**.</span><span class="sxs-lookup"><span data-stu-id="d1849-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="d1849-111">Haga clic en **Agregar una nueva sección (+)** en el lado izquierdo de la página y, a continuación, haga clic en **dos columnas** para el diseño de la sección.</span><span class="sxs-lookup"><span data-stu-id="d1849-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="d1849-112">En la columna izquierda, haga clic en + y, a continuación, haga clic en el elemento Web **incrustar** .</span><span class="sxs-lookup"><span data-stu-id="d1849-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="d1849-113">En la columna derecha, haga clic en + y, a continuación, haga clic en el elemento Web de **texto** .</span><span class="sxs-lookup"><span data-stu-id="d1849-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="d1849-114">La página debe tener un aspecto similar a este.</span><span class="sxs-lookup"><span data-stu-id="d1849-114">Your page should look like this.</span></span>

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="d1849-116">Agregar un vídeo y texto desde YouTube</span><span class="sxs-lookup"><span data-stu-id="d1849-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="d1849-117">En el explorador, vaya a YouTube.</span><span class="sxs-lookup"><span data-stu-id="d1849-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="d1849-118">Para este ejemplo, busque "¿Qué es Office 365 – mejor aplicación de productividad de Microsoft".</span><span class="sxs-lookup"><span data-stu-id="d1849-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="d1849-119">Haga clic en el vídeo para reproducirlo, luego PAUSE y haga clic con el botón derecho en él.</span><span class="sxs-lookup"><span data-stu-id="d1849-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="d1849-120">Haga clic en **Copiar código para insertar**y, a continuación, vuelva a la página de SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d1849-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="d1849-121">Haga clic en **Agregar código para insertar** en el elemento Web **Insertar** y, a continuación, agregue el código del vídeo de YouTube.</span><span class="sxs-lookup"><span data-stu-id="d1849-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="d1849-122">Vuelva a la página de YouTube y copie el texto de la **Descripción** del vídeo.</span><span class="sxs-lookup"><span data-stu-id="d1849-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="d1849-123">Vuelva a la página de SharePoint, seleccione el elemento Web de **texto** y, a continuación, copie el texto del vídeo de YouTube.</span><span class="sxs-lookup"><span data-stu-id="d1849-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="d1849-124">Seleccione el icono **Editar elemento Web** en el área de título de la página de SharePoint y, a continuación, asigne a la página el nombre "Introducción a la lista de reproducción personalizada".</span><span class="sxs-lookup"><span data-stu-id="d1849-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="d1849-125">En **diseño**, seleccione **normal**y, a continuación, cierre panel Propiedades del **área de título** .</span><span class="sxs-lookup"><span data-stu-id="d1849-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="d1849-126">La página debería tener ahora un aspecto similar al siguiente.</span><span class="sxs-lookup"><span data-stu-id="d1849-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="d1849-128">Publicar la página</span><span class="sxs-lookup"><span data-stu-id="d1849-128">Publish the page</span></span>

- <span data-ttu-id="d1849-129">Seleccione el botón **publicar** .</span><span class="sxs-lookup"><span data-stu-id="d1849-129">Select the **Publish** button.</span></span> <span data-ttu-id="d1849-130">Ahora está listo para agregar esta página de SharePoint a la lista de reproducción personalizada.</span><span class="sxs-lookup"><span data-stu-id="d1849-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 