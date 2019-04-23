---
author: pkrebs
ms.author: pkrebs
title: Vinculación a recursos de aprendizaje personalizados
ms.date: 02/15/2019
description: Cómo vincular a recursos de aprendizaje personalizados
ms.openlocfilehash: cdde37f370663ca50241833a15e8411921b45a1b
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "32056173"
---
# <a name="link-to-custom-learning-content"></a><span data-ttu-id="77f84-103">Vincular a contenido de aprendizaje personalizado</span><span class="sxs-lookup"><span data-stu-id="77f84-103">Link to Custom Learning content</span></span>

<span data-ttu-id="77f84-104">Con aprendizaje personalizado, hay dos formas de vincular al contenido:</span><span class="sxs-lookup"><span data-stu-id="77f84-104">With Custom Learning, there are two ways to link to content:</span></span>

- <span data-ttu-id="77f84-105">Vínculo a la página que hospeda el elemento Web filtrado para el contenido que desea mostrar.</span><span class="sxs-lookup"><span data-stu-id="77f84-105">Link to the page that host the Web part filtered for the content you want to display.</span></span> 
- <span data-ttu-id="77f84-106">Vincular directamente a una instancia del elemento Web</span><span class="sxs-lookup"><span data-stu-id="77f84-106">Link directly to an instance of the Web part</span></span>

## <a name="link-to-a-page"></a><span data-ttu-id="77f84-107">Vínculo a una página</span><span class="sxs-lookup"><span data-stu-id="77f84-107">Link to a page</span></span>

<span data-ttu-id="77f84-108">Si ha creado nuevas páginas y experiencias de aprendizaje con el elemento Web de aprendizaje personalizado, puede crear un vínculo a la página con el elemento web configurado para mostrar el contenido que desea mostrar.</span><span class="sxs-lookup"><span data-stu-id="77f84-108">If you've created new pages and learning experiences with the Custom Learning Web part, you can link to the page with the Web part configured to show the content you want to display.</span></span> <span data-ttu-id="77f84-109">En la sección anterior, hemos explicado cómo mostrar listas de reproducción de Excel en una página.</span><span class="sxs-lookup"><span data-stu-id="77f84-109">In the previous section, we covered how to display Excel playlists on a page.</span></span> <span data-ttu-id="77f84-110">Ahora puede editar la Página principal para vincularla a la página.</span><span class="sxs-lookup"><span data-stu-id="77f84-110">You could now edit the Home page to link to the page.</span></span> 

1. <span data-ttu-id="77f84-111">En la Página principal, haga clic en **Editar**.</span><span class="sxs-lookup"><span data-stu-id="77f84-111">From the Home page, click **Edit**.</span></span>
2. <span data-ttu-id="77f84-112">Haga clic en **editar detalles** en uno de los mosaicos de la Página principal.</span><span class="sxs-lookup"><span data-stu-id="77f84-112">Click **Edit details** in one of the Home page tiles.</span></span> <span data-ttu-id="77f84-113">En este ejemplo, se editan las fichas de **listas de reproducción recomendadas** .</span><span class="sxs-lookup"><span data-stu-id="77f84-113">In this example, we edit the **Recommended playlists** tiles.</span></span>
3. <span data-ttu-id="77f84-114">En **vínculo**, haga clic en **cambiar**.</span><span class="sxs-lookup"><span data-stu-id="77f84-114">Under **Link**, click **Change**.</span></span>

![CG-linktopage. png](media/cg-linktopage.png)

4. <span data-ttu-id="77f84-116">Haga clic en **sitio**, después en **páginas del sitio**, haga clic en la página que desea vincular y, a continuación, haga clic en **abrir**.</span><span class="sxs-lookup"><span data-stu-id="77f84-116">Click **Site**, then **Site Pages**, click the page you want to link to, and then click **Open**.</span></span> <span data-ttu-id="77f84-117">En este ejemplo, nos vinculamos a la página **Create-Your-Own-Experience. aspx** tratada en la sección anterior.</span><span class="sxs-lookup"><span data-stu-id="77f84-117">In this example, we link to the **Create-your-own-experience.aspx** page covered in the previous section.</span></span>
5. <span data-ttu-id="77f84-118">Cierre el panel Propiedades del héroe, haga clic en **publicar**y, a continuación, pruebe el vínculo.</span><span class="sxs-lookup"><span data-stu-id="77f84-118">Close the Hero properties pane, click **Publish**, and then test the link.</span></span> 

## <a name="link-to-the-custom-learning-web-part"></a><span data-ttu-id="77f84-119">Vínculo al elemento Web de aprendizaje personalizado</span><span class="sxs-lookup"><span data-stu-id="77f84-119">Link to the Custom Learning web part</span></span>
<span data-ttu-id="77f84-120">El aprendizaje personalizado le proporciona, el administrador o un usuario final, la capacidad de vincular a una instancia del elemento web independiente de la página que contiene el elemento Web.</span><span class="sxs-lookup"><span data-stu-id="77f84-120">Custom Learning gives you, the administrator, or an end-user, the ability to link to an instance of the Web part independent of the page that contains the Web part.</span></span> <span data-ttu-id="77f84-121">Puede compartir el vínculo o el vínculo que se ha copiado desde otras páginas.</span><span class="sxs-lookup"><span data-stu-id="77f84-121">You can share the copied link or link to it from other pages.</span></span> <span data-ttu-id="77f84-122">Al hacer clic en el vínculo copiado, se muestra la instancia del elemento Web de aprendizaje personalizado en la página CustomLLearningViewer. aspx.</span><span class="sxs-lookup"><span data-stu-id="77f84-122">The copied link, when clicked, shows the Custom Learning web part instance in the CustomLLearningViewer.aspx page.</span></span> <span data-ttu-id="77f84-123">Veamos un ejemplo.</span><span class="sxs-lookup"><span data-stu-id="77f84-123">Let's look at an example.</span></span> 

1. <span data-ttu-id="77f84-124">En la Página principal, haga clic en **Office 365 Training**.</span><span class="sxs-lookup"><span data-stu-id="77f84-124">From the Home page, click **Office 365 training**.</span></span>
2. <span data-ttu-id="77f84-125">Haga clic en **Microsoft Teams**y, a continuación, en **Introducción a Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="77f84-125">Click **Microsoft Teams**, and then click **Intro to Microsoft Teams**.</span></span>
3. <span data-ttu-id="77f84-126">Haga clic en el icono **copiar** .</span><span class="sxs-lookup"><span data-stu-id="77f84-126">Click the **Copy** icon.</span></span>

![CG-linktowebpart. png](media/cg-linktowebpart.png)

4. <span data-ttu-id="77f84-128">Haga clic en Inicio en el menú aprendizaje personalizado.</span><span class="sxs-lookup"><span data-stu-id="77f84-128">Click Home from the Custom Learning menu.</span></span>
5. <span data-ttu-id="77f84-129">Pegue la dirección URL copiada en la barra de direcciones del explorador y presione Entrar.</span><span class="sxs-lookup"><span data-stu-id="77f84-129">Paste the copied URL in the address bar of the browser and press ENTER.</span></span> 

<span data-ttu-id="77f84-130">Como se muestra en la siguiente ilustración, el vínculo va a la página CustomLearningViewer. aspx y muestra el contenido en función de los parámetros del vínculo copiado.</span><span class="sxs-lookup"><span data-stu-id="77f84-130">As shown in the following illustration, the link goes to the CustomLearningViewer.aspx page and displays the content based on the parameters in the copied link.</span></span> 

![CG-linktowebpartviewer. png](media/cg-linktowebpartviewer.png)

