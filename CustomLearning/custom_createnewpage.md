---
author: pkrebs
ms.author: pkrebs
title: Crear páginas de SharePoint para listas de reproducción
ms.date: 02/10/2019
description: Crear páginas de SharePoint para listas de reproducción
ms.service: sharepoint-online
ms.openlocfilehash: 40c249fbd5b0fdaefd555f23bf20ac23240ea954
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999096"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="1bc68-103">Crear páginas de SharePoint para listas de reproducción personalizadas</span><span class="sxs-lookup"><span data-stu-id="1bc68-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="1bc68-104">Una de las características únicas de las rutas de aprendizaje es la capacidad de crear listas de reproducción que se ensamblan a partir de activos de Microsoft y de activos de SharePoint que cree.</span><span class="sxs-lookup"><span data-stu-id="1bc68-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="1bc68-105">En este ejemplo, crearemos una página de SharePoint antes de crear una lista de reproducción.</span><span class="sxs-lookup"><span data-stu-id="1bc68-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="1bc68-106">La capacidad de crear listas de reproducción a partir de páginas de SharePoint ofrece una variedad de oportunidades para crear páginas con los elementos web disponibles de Microsoft o su organización.</span><span class="sxs-lookup"><span data-stu-id="1bc68-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="1bc68-107">Por ejemplo, una lista de reproducción puede incluir una página de SharePoint con vídeos incrustados de YouTube, un formulario creado a partir de Office 365 Forms o un informe de Power BI incrustado.</span><span class="sxs-lookup"><span data-stu-id="1bc68-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="1bc68-108">En este ejemplo, le mostraremos cómo crear una página con el elemento web Embed y el elemento web Text.</span><span class="sxs-lookup"><span data-stu-id="1bc68-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="1bc68-109">Crear una página de SharePoint para una lista de reproducción personalizada</span><span class="sxs-lookup"><span data-stu-id="1bc68-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="1bc68-110">Haga clic en el **icono** de Engranaje de SharePoint y, a continuación, haga clic en Agregar **una página**.</span><span class="sxs-lookup"><span data-stu-id="1bc68-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="1bc68-111">Haga **clic en Agregar una nueva sección (+)** en el lado izquierdo de la página y, a continuación, haga clic en Dos **columnas** para el diseño de sección.</span><span class="sxs-lookup"><span data-stu-id="1bc68-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="1bc68-112">En la columna izquierda, haga clic en + y, a continuación, haga clic en el elemento web **Insertar.**</span><span class="sxs-lookup"><span data-stu-id="1bc68-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="1bc68-113">En la columna derecha, haga clic en +y, a continuación, haga clic en el **elemento** web Texto.</span><span class="sxs-lookup"><span data-stu-id="1bc68-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="1bc68-114">La página debe tener este aspecto.</span><span class="sxs-lookup"><span data-stu-id="1bc68-114">Your page should look like this.</span></span>

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="1bc68-116">Agregar un vídeo y texto de YouTube</span><span class="sxs-lookup"><span data-stu-id="1bc68-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="1bc68-117">En el explorador, ve a YouTube.</span><span class="sxs-lookup"><span data-stu-id="1bc68-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="1bc68-118">En este ejemplo, busque "Qué es Office 365: las mejores aplicaciones de productividad de Microsoft".</span><span class="sxs-lookup"><span data-stu-id="1bc68-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="1bc68-119">Haz clic en el vídeo para reproducirlo, luego pausalo y, a continuación, haz clic con el botón secundario en él.</span><span class="sxs-lookup"><span data-stu-id="1bc68-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="1bc68-120">Haga **clic en Copiar código de** inserción y, a continuación, vuelva a la página de SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1bc68-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="1bc68-121">Haga **clic en Agregar código de** inserción en el elemento web **Insertar** y, a continuación, agregue el código desde el vídeo de YouTube.</span><span class="sxs-lookup"><span data-stu-id="1bc68-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="1bc68-122">Vuelva a la página de YouTube y copie el **texto Descripción** del vídeo.</span><span class="sxs-lookup"><span data-stu-id="1bc68-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="1bc68-123">Vuelva a la página de SharePoint, seleccione el **elemento** web Texto y, a continuación, copie el texto del vídeo de YouTube.</span><span class="sxs-lookup"><span data-stu-id="1bc68-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="1bc68-124">Seleccione el **icono Editar elemento web** en el área Título de la página de SharePoint y, a continuación, asigne a la página el nombre "Introducción a la lista de reproducción personalizada".</span><span class="sxs-lookup"><span data-stu-id="1bc68-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="1bc68-125">En **Diseño**, seleccione **Sin formato** y, a continuación, cierre el panel de propiedades de la **región** de título.</span><span class="sxs-lookup"><span data-stu-id="1bc68-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="1bc68-126">La página ahora debería tener un aspecto parecido al siguiente.</span><span class="sxs-lookup"><span data-stu-id="1bc68-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="1bc68-128">Publicar la página</span><span class="sxs-lookup"><span data-stu-id="1bc68-128">Publish the page</span></span>

- <span data-ttu-id="1bc68-129">Seleccione el **botón** Publicar.</span><span class="sxs-lookup"><span data-stu-id="1bc68-129">Select the **Publish** button.</span></span> <span data-ttu-id="1bc68-130">Ahora ya está listo para agregar esta página de SharePoint a la lista de reproducción personalizada.</span><span class="sxs-lookup"><span data-stu-id="1bc68-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 