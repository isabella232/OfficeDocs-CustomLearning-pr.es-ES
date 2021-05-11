---
author: pkrebs
ms.author: pkrebs
title: Crear SharePoint para listas de reproducción
ms.date: 02/10/2019
description: Crear SharePoint para listas de reproducción
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: ce4a204b3072469840b6f3fa8f93d9e78833b181
ms.sourcegitcommit: 956ab22dd8ce23ee1779f1a01d34b434243c3cb1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/11/2021
ms.locfileid: "52310664"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="40f56-103">Crear SharePoint para listas de reproducción personalizadas</span><span class="sxs-lookup"><span data-stu-id="40f56-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="40f56-104">Una de las características únicas de las rutas de aprendizaje es la capacidad de crear listas de reproducción que se ensamblan a partir de activos de Microsoft y SharePoint activos que cree.</span><span class="sxs-lookup"><span data-stu-id="40f56-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="40f56-105">En este ejemplo, crearemos una página de SharePoint antes de crear una lista de reproducción.</span><span class="sxs-lookup"><span data-stu-id="40f56-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="40f56-106">La capacidad de crear listas de reproducción SharePoint páginas ofrece una variedad de oportunidades para crear páginas con los elementos web disponibles de Microsoft o su organización.</span><span class="sxs-lookup"><span data-stu-id="40f56-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="40f56-107">Por ejemplo, una lista de reproducción puede incluir una página SharePoint con vídeos incrustados de YouTube, un formulario creado a partir de Office 365 Forms o un informe de Power BI integrado.</span><span class="sxs-lookup"><span data-stu-id="40f56-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="40f56-108">En este ejemplo, le mostraremos cómo crear una página con el elemento web Embed y el elemento web Text.</span><span class="sxs-lookup"><span data-stu-id="40f56-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="40f56-109">Crear una SharePoint para una lista de reproducción personalizada</span><span class="sxs-lookup"><span data-stu-id="40f56-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="40f56-110">Haga clic en el SharePoint **Engranaje** y, a continuación, haga clic **en Agregar una página**.</span><span class="sxs-lookup"><span data-stu-id="40f56-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="40f56-111">Haga **clic en Agregar una nueva sección (+)** en el lado izquierdo de la página y, a continuación, haga clic en Dos **columnas** para el diseño de sección.</span><span class="sxs-lookup"><span data-stu-id="40f56-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="40f56-112">En la columna izquierda, haga clic en + y, a continuación, haga clic en el elemento web **Insertar.**</span><span class="sxs-lookup"><span data-stu-id="40f56-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="40f56-113">En la columna derecha, haga clic en +y, a continuación, haga clic en el **elemento** web Texto.</span><span class="sxs-lookup"><span data-stu-id="40f56-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="40f56-114">La página debe tener este aspecto.</span><span class="sxs-lookup"><span data-stu-id="40f56-114">Your page should look like this.</span></span>

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="40f56-116">Agregar un vídeo y texto de YouTube</span><span class="sxs-lookup"><span data-stu-id="40f56-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="40f56-117">En el explorador, ve a YouTube.</span><span class="sxs-lookup"><span data-stu-id="40f56-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="40f56-118">Para este ejemplo, busque "What is Office 365– Microsoft's best productivity apps".</span><span class="sxs-lookup"><span data-stu-id="40f56-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="40f56-119">Haz clic en el vídeo para reproducirlo, luego pausalo y, a continuación, haz clic con el botón secundario en él.</span><span class="sxs-lookup"><span data-stu-id="40f56-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="40f56-120">Haga **clic en Copiar código de** inserción y, a continuación, vuelva a la SharePoint página.</span><span class="sxs-lookup"><span data-stu-id="40f56-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="40f56-121">Haga **clic en Agregar código de** inserción en el elemento web **Insertar** y, a continuación, agregue el código desde el vídeo de YouTube.</span><span class="sxs-lookup"><span data-stu-id="40f56-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="40f56-122">Vuelva a la página de YouTube y copie el **texto Descripción** del vídeo.</span><span class="sxs-lookup"><span data-stu-id="40f56-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="40f56-123">Vuelva a la SharePoint, seleccione el **elemento** web Texto y, a continuación, copie el texto del vídeo de YouTube.</span><span class="sxs-lookup"><span data-stu-id="40f56-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="40f56-124">Seleccione el **icono Editar elemento web** en el área Título de la página SharePoint y, a continuación, asigne a la página el nombre "Introducción a la lista de reproducción personalizada".</span><span class="sxs-lookup"><span data-stu-id="40f56-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="40f56-125">En **Diseño**, seleccione **Sin formato** y, a continuación, cierre el panel de propiedades de la **región** de título.</span><span class="sxs-lookup"><span data-stu-id="40f56-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="40f56-126">La página ahora debería tener un aspecto parecido al siguiente.</span><span class="sxs-lookup"><span data-stu-id="40f56-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="40f56-128">Publicar la página</span><span class="sxs-lookup"><span data-stu-id="40f56-128">Publish the page</span></span>

- <span data-ttu-id="40f56-129">Seleccione el **botón** Publicar.</span><span class="sxs-lookup"><span data-stu-id="40f56-129">Select the **Publish** button.</span></span> <span data-ttu-id="40f56-130">Ahora estás listo para agregar esta página SharePoint a la lista de reproducción personalizada.</span><span class="sxs-lookup"><span data-stu-id="40f56-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 