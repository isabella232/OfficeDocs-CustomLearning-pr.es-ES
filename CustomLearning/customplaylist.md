---
author: karuanag
ms.author: karuanag
title: Personalizar y compartir listas de reproducción
ms.date: 02/10/2019
description: Crear listas de reproducción personalizadas a partir de contenido existente o de nuevas páginas de SharePoint
ms.openlocfilehash: d330b6e401c9020eb68877bc8a132350811a2f31
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989731"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="23ec2-103">Personalizar y compartir listas de reproducción</span><span class="sxs-lookup"><span data-stu-id="23ec2-103">Customize and Share Playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="23ec2-104">Crear una lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="23ec2-104">Create a Playlist</span></span>

<span data-ttu-id="23ec2-p101">Una lista de reproducción es una conformidad de "activos". Un "activo" es una página de SharePoint o un elemento existente del contenido de aprendizaje de Microsoft. Cuando se crea una lista de reproducción, se seleccionan los activos que van juntos para crear una ruta de aprendizaje para el usuario.</span><span class="sxs-lookup"><span data-stu-id="23ec2-p101">A playlist is a compliation of "assets". An "asset" is a SharePoint page or existing item of Microsoft training content. When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="23ec2-p102">La ventaja de agregar páginas de SharePoint es que puede crear páginas de SharePoint con vídeos o vídeos de YouTube hospedados en la organización. También puede crear páginas con formularios u otro contenido de Office 365.</span><span class="sxs-lookup"><span data-stu-id="23ec2-p102">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization. You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="23ec2-110">Paso 1: crear una página de SharePoint para la lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="23ec2-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="23ec2-p103">En este ejemplo, primero crearemos una página de SharePoint para agregarla a la lista de reproducción. Crearemos una página con un elemento Web de vídeo de YouTube y un elemento Web de texto.  En estas instrucciones se da por sentado que usa el servicio de SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="23ec2-p103">In this example, we’ll first create a SharePoint page to add to the playlist. We’ll create a page with a YouTube video web part and Text web part.  These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="23ec2-114">Crear una nueva página</span><span class="sxs-lookup"><span data-stu-id="23ec2-114">Create a new page</span></span>
1.  <span data-ttu-id="23ec2-115">Seleccione el menú configuración > contenidos del sitio > páginas del sitio > nueva página del sitio de >.</span><span class="sxs-lookup"><span data-stu-id="23ec2-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="23ec2-116">En el área título, escriba usar el cuadro de comandos de Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="23ec2-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="23ec2-117">Seleccione Agregar una sección nueva y, a continuación, seleccione dos columnas.</span><span class="sxs-lookup"><span data-stu-id="23ec2-117">Select the Add a new section, and then select Two Columns.</span></span>

![agregar dos columnas](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="23ec2-119">En el cuadro de la izquierda, seleccione Agregar un nuevo elemento Web y, a continuación, seleccione incrustar.</span><span class="sxs-lookup"><span data-stu-id="23ec2-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="23ec2-120">En un explorador Web, vaya a esta dirección https://youtu.be/wYrRCRphrp0 URL y obtenga el código para insertar para el vídeo.</span><span class="sxs-lookup"><span data-stu-id="23ec2-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="23ec2-121">En el elemento Web de SharePoint, seleccione Agregar código para insertar y, a continuación, péguelo en el cuadro insertar.</span><span class="sxs-lookup"><span data-stu-id="23ec2-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="23ec2-122">En el cuadro derecho, seleccione Agregar un nuevo elemento Web y, a continuación, seleccione texto.</span><span class="sxs-lookup"><span data-stu-id="23ec2-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="23ec2-p104">En un explorador Web, vaya a esta dirección URL https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b : y copie el bloque de! Instrucciones de la página y pegarlas en el elemento Web de texto. La página debe tener un aspecto similar al siguiente.</span><span class="sxs-lookup"><span data-stu-id="23ec2-p104">In a Web browser, go to this URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it! Instructions from the page and paste them into the Text Web part. Your page should look like the following.</span></span> 

![Insertar página](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="23ec2-127">Haga clic en **publicar**y, a continuación, copie la dirección URL de la página y péguela en el Bloc de notas</span><span class="sxs-lookup"><span data-stu-id="23ec2-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="23ec2-128">Paso 2: crear la lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="23ec2-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="23ec2-p105">Navegue a la página de **Administración de aprendizaje personalizada** en la experiencia del sitio. ![custom_admin. png](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="23ec2-p105">Navigate to the **Custom Learning Administration** page in your site experience. ![custom_admin.png](media/custom_admin.png)</span></span>
1. <span data-ttu-id="23ec2-131">Asegurarse de que la **categoría** está seleccionada</span><span class="sxs-lookup"><span data-stu-id="23ec2-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="23ec2-132">Haga clic en la categoría en la que desea que aparezca la nueva lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="23ec2-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="23ec2-133">Junto al nombre de la categoría, haga clic en el ![símbolo más custom_addplay. png](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="23ec2-133">Next to the category name, click on the plus symbol ![custom_addplay.png](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="23ec2-p106">ReLlene los valores como se muestra en el ejemplo siguiente y seleccione **crear**. ![custom_details. png](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="23ec2-p106">Fill in the values as shown in the example below and select **Create**. ![custom_details.png](media/custom_details.png)</span></span>
- <span data-ttu-id="23ec2-136">**Título** : nombre para mostrar de la lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="23ec2-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="23ec2-137">**Descripción** : información sobre lo que se aprenderá</span><span class="sxs-lookup"><span data-stu-id="23ec2-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="23ec2-138">**Categoría** : preseleccionado en función de la selección inicial</span><span class="sxs-lookup"><span data-stu-id="23ec2-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="23ec2-139">**Subcategoría** : preseleccionado en función de la selección inicial</span><span class="sxs-lookup"><span data-stu-id="23ec2-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="23ec2-140">**Tecnología** : seleccionar según corresponda</span><span class="sxs-lookup"><span data-stu-id="23ec2-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="23ec2-141">**Nivel** : principiante, Intermidate o avanzado</span><span class="sxs-lookup"><span data-stu-id="23ec2-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="23ec2-142">**Audiencia** : Esto permite destinar contenido en función de una lista predefinida de roles proporcionados por Microsoft.</span><span class="sxs-lookup"><span data-stu-id="23ec2-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="23ec2-143">Haga clic en **Guardar detalle**</span><span class="sxs-lookup"><span data-stu-id="23ec2-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="23ec2-p107">Puede personalizar la imagen del icono de la lista de reproducción.  Haga clic en el icono de imagen e inserte una dirección URL de una imagen previamente cargada.  Asegúrese de que la imagen se encuentra dentro de la colección de sitios de aprendizaje personalizada o en otra ubicación en la que todos los usuarios tendrán acceso al archivo.</span><span class="sxs-lookup"><span data-stu-id="23ec2-p107">You can customize the icon image for your playlist.  Click the image icon and insert an URL of a previously uploaded image.  Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="23ec2-147">![custom_image. png](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="23ec2-147">![custom_image.png](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="23ec2-148">Paso 3: agregar activos a la lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="23ec2-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="23ec2-149">En este paso, agregará los activos existentes de Microsoft y la página de SharePoint que ha creado a la lista de reproducción.</span><span class="sxs-lookup"><span data-stu-id="23ec2-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="23ec2-150">Una vez que haya guardado los detalles de la lista de reproducción, puede usar la búsqueda de activos existentes.</span><span class="sxs-lookup"><span data-stu-id="23ec2-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="23ec2-p108">**Escriba un término de búsqueda** para ver una lista de activos predefinidos que están disponibles desde otras listas de reproducción. **Haga clic en el nombre** de un activo para incluirlo en la nueva lista de reproducción. ![custom_slist. png](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="23ec2-p108">**Enter in any search term** to see a list of predefined assets that are available from other playlists. **Click on the name** of an asset to include it in your new playlist. ![custom_slist.png](media/custom_slist.png)</span></span>

<span data-ttu-id="23ec2-154">También puede Agregar la página de SharePoint que creó anteriormente o crear una a partir de cero en la experiencia.</span><span class="sxs-lookup"><span data-stu-id="23ec2-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="23ec2-155">Haga clic en la opción **nuevo activo** en el cuadro de diálogo activos de la lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="23ec2-155">Click on the **New Asset** option in the Playlist Assets dialog</span></span>
1. <span data-ttu-id="23ec2-p109">Asigne un **título**al activo. Una vez escritas, las opciones ![adicionales mostrarán custom_newpage. png](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="23ec2-p109">Give your asset a **Title**. Once entered, additional options will display ![custom_newpage.png](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="23ec2-158">Ahora puede crear una nueva página de activos en SharePoint Online o especificar en la dirección URL de una página existente para agregarla a la lista de reproducción personalizada.</span><span class="sxs-lookup"><span data-stu-id="23ec2-158">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="23ec2-159">\*\*\*\* Los campos Category, **Sub Category** y **Technology** se rellenarán previamente en función de las selecciones anteriores de esta lista de reproducción.</span><span class="sxs-lookup"><span data-stu-id="23ec2-159">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="23ec2-160">Realice las selecciones adecuadas para nivel y audiencia para este activo individual.</span><span class="sxs-lookup"><span data-stu-id="23ec2-160">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="23ec2-161">Haga clic en **Guardar activo** para agregarlo a la lista de reproducción personalizada</span><span class="sxs-lookup"><span data-stu-id="23ec2-161">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="23ec2-162">Repita estos pasos, ya sea buscando o agregando páginas individuales, hasta que la lista de reproducción haya finalizado.</span><span class="sxs-lookup"><span data-stu-id="23ec2-162">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="23ec2-163">Haga clic en **cerrar lista de reproducción** para guardar</span><span class="sxs-lookup"><span data-stu-id="23ec2-163">Click **Close Playlist** to save</span></span>

<span data-ttu-id="23ec2-164">La lista de reproducción con este contenido estará ahora disponible en cualquier lugar en el que haya instalado o incrustado el elemento Web de aprendizaje personalizado.</span><span class="sxs-lookup"><span data-stu-id="23ec2-164">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="23ec2-165">Si comete un error después de cerrar la lista de reproducción, puede eliminarla de la categoría haciendo clic en la X junto al nombre de la lista de reproducción.</span><span class="sxs-lookup"><span data-stu-id="23ec2-165">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="23ec2-166">Cosas que debe considerar</span><span class="sxs-lookup"><span data-stu-id="23ec2-166">Things to Think About</span></span>

<span data-ttu-id="23ec2-p110">Las listas de reproducción personalizadas se pueden usar para ayudar a los usuarios finales en diversas tareas.  ¿Tiene un formulario de solicitud de tiempo de espera?  Un formulario para solicitar equipamiento de hardware?  Los activos de formación existentes se pueden programar en la experiencia.</span><span class="sxs-lookup"><span data-stu-id="23ec2-p110">Custom playlists can be used to assist your end users in a variety of tasks.  Do you have a time off request form?  A form to request hardware equipment?  Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="23ec2-171">Compartir listas de reproducción</span><span class="sxs-lookup"><span data-stu-id="23ec2-171">Share Playlists</span></span>

1. <span data-ttu-id="23ec2-172">Navegar a cualquier lista de reproducción de la experiencia del elemento Web o del sitio</span><span class="sxs-lookup"><span data-stu-id="23ec2-172">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="23ec2-173">En la esquina superior izquierda verá tres iconos</span><span class="sxs-lookup"><span data-stu-id="23ec2-173">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="23ec2-174">Haga clic en el icono que representa un vínculo</span><span class="sxs-lookup"><span data-stu-id="23ec2-174">Click on the icon representing a link</span></span>
1. <span data-ttu-id="23ec2-175">Copiar la dirección URL a la lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="23ec2-175">Copy the URL to the playlist</span></span>

<span data-ttu-id="23ec2-176">![Share. png](media/share.png) ahora, esta dirección URL puede insertarse en la navegación del sitio o usarse en otras comunicaciones para llevar a sus empleados directamente a esa lista de reproducción.</span><span class="sxs-lookup"><span data-stu-id="23ec2-176">![share.png](media/share.png) This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoptiondriveadoptionmd"></a><span data-ttu-id="23ec2-177">Pasos siguientes: [impulsar la adopción](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="23ec2-177">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
