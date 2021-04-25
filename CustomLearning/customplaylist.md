---
author: karuanag
ms.author: karuanag
manager: alexb
title: Personalizar y compartir listas de reproducción
ms.date: 02/10/2019
description: Crear listas de reproducción personalizadas a partir de contenido existente o nuevas páginas de SharePoint
ms.service: sharepoint-online
audience: itpro
ms.topic: article
ms.openlocfilehash: 31a0e5524181d26f4d62ae7206636c9e553b6f8f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000216"
---
# <a name="customize-and-share-playlists"></a>Personalizar y compartir listas de reproducción

## <a name="create-a-playlist"></a>Crear una lista de reproducción

Una lista de reproducción es una complición de "activos". Un "activo" es una página de SharePoint o un elemento existente del contenido de aprendizaje de Microsoft. Cuando creas una lista de reproducción, seleccionas activos que van juntos para crear una ruta de aprendizaje para el usuario.  

La ventaja de agregar páginas de SharePoint es que puede crear páginas de SharePoint con vídeos o vídeos de YouTube hospedados en su organización. También puede crear páginas con formularios u otro contenido de Office 365.  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a>Paso 1: Crear una página de SharePoint para la lista de reproducción
En este ejemplo, primero crearemos una página de SharePoint para agregarla a la lista de reproducción. Crearemos una página con un elemento web de vídeo de YouTube y un elemento web de texto.  Estas instrucciones suponen que está usando el servicio de SharePoint Online. 

#### <a name="create-a-new-page"></a>Crear una nueva página
1.  Seleccione el menú Configuración > contenido del sitio > página > Página de > sitio nueva.
2.  En el área de título, escriba Usar el cuadro de comandos de Teams
3.  Seleccione la sección Agregar un nuevo y, a continuación, dos columnas.

![agregar dos columnas](media/clo365addtwocolumn.png)

4.  En el cuadro izquierdo, seleccione Agregar un nuevo elemento web y, a continuación, seleccione Insertar. 
5.  En un explorador web, vaya a esta dirección URL https://youtu.be/wYrRCRphrp0 y obtenga el código de inserción del vídeo. 
6.  En el elemento web de SharePoint, seleccione Agregar código incrustado y, a continuación, péguelo en el cuadro Insertar. 
7.  En el cuadro derecho, seleccione Agregar un nuevo elemento web y, a continuación, seleccione Texto. 
8.  En un explorador web, vaya a esta dirección URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b y copie la opción Pruébalo. Instrucciones de la página y péguelas en el elemento web de texto. La página debe tener el siguiente aspecto. 
![Página Insertar](media/clo365teamscommandbox.png)
9.  Haga **clic en** Publicar y, a continuación, copie la dirección URL de la página y péguela en el Bloc de notas

#### <a name="step-2-create-the-playlist"></a>Paso 2: Crear la lista de reproducción

1. Vaya a la **página Administración de aprendizaje personalizada** en la experiencia del sitio.
![Pantalla en la que selecciona Administración de aprendizaje personalizada.](media/custom_admin.png)
1. Asegúrese de **que Categoría** está seleccionada 
1. Haz clic en la categoría en la que quieres que aparezca la nueva lista de reproducción
1. Junto al nombre de categoría, haga clic en el símbolo más Ventana con la opción ![ Categoría y el signo Más resaltado.](media/custom_addplay.png)

1. Rellene los valores como se muestra en el ejemplo siguiente y seleccione **Crear**. 
![Página en la que escribes los detalles de la lista de reproducción.](media/custom_details.png)
- **Título:** nombre para mostrar de la lista de reproducción
- **Descripción:** información sobre lo que se va a aprender
- **Categoría:** preseleccionada en función de la selección inicial
- **Subcategoría:** preseleccionada en función de la selección intial
- **Tecnología:** seleccione según corresponda
- **Nivel:** principiante, intermidado o avanzado
- **Audiencia:** esto le permite dirigir el contenido en función de una lista predefinida de roles proporcionados por Microsoft.

6. Haga clic **en Guardar detalle**

> [!TIP]
> Puedes personalizar la imagen de icono de la lista de reproducción.  Haga clic en el icono de imagen e inserte una dirección URL de una imagen cargada anteriormente.  Asegúrese de que la imagen se encuentra dentro de la colección de sitios aprendizaje personalizado o en otra ubicación en la que todos los usuarios tendrán acceso al archivo.  
![Elija una ventana de imagen.](media/custom_image.png)

#### <a name="step-3-add-assets-to-the-playlist"></a>Paso 3: Agregar activos a la lista de reproducción
En este paso, agregará activos existentes de Microsoft y la página de SharePoint que creó a la lista de reproducción. 

1. Una vez guardados los detalles de la lista de reproducción, puedes usar la búsqueda de activos existentes.
1. **Escribe cualquier término de búsqueda** para ver una lista de activos predefinidos que están disponibles en otras listas de reproducción. **Haz clic en el nombre** de un activo para incluirlo en la nueva lista de reproducción.<br/>
![Página Activos de lista de reproducción](media/custom_slist.png)

También puede agregar la página de SharePoint que creó anteriormente o crear una desde cero en la experiencia.

1. Haga clic en la **opción Nuevo activo** en el cuadro de diálogo Activos de lista de reproducción.
1. Dé a su activo un **título**. Una vez especificado, se mostrarán opciones adicionales.
![Formulario en el que escribes el título y detalles adicionales.](media/custom_newpage.png)
1. Ahora puede crear una nueva página de activos en SharePoint Online o escribir la dirección URL de una página existente para agregarla a la lista de reproducción personalizada. 
1. **Los** campos Category , **Sub Category** y **Technology** se rellenarán previamente en función de las selecciones anteriores para esta lista de reproducción.
1. Realice las selecciones adecuadas para Nivel y Audiencia para este activo individual.  
1. Haga **clic en Guardar activo** para agregarlo a la lista de reproducción personalizada
1. Repita estos pasos, ya sea buscando o agregando páginas individuales, hasta que se complete la lista de reproducción. 
1. Haga **clic en Cerrar lista de reproducción** para guardar

La lista de reproducción con este contenido ahora estará disponible en cualquier lugar que haya instalado o incrustado el elemento web aprendizaje personalizado. 

> [!NOTE]
> Si cometes un error una vez cerrada la lista de reproducción, puedes eliminarla de la categoría haciendo clic en la X situada junto al nombre de la lista de reproducción.  

#### <a name="things-to-think-about"></a>Cosas en las que pensar

Las listas de reproducción personalizadas se pueden usar para ayudar a los usuarios finales en una variedad de tareas.  ¿Tiene un formulario de solicitud de tiempo libre?  ¿Un formulario para solicitar equipamiento de hardware?  Los activos de aprendizaje existentes se pueden programar en la experiencia.  

## <a name="share-playlists"></a>Compartir listas de reproducción

1. Navegue a cualquier lista de reproducción dentro de la experiencia del sitio o del elemento web
1. En la esquina superior izquierda verá tres iconos
1. Haga clic en el icono que representa un vínculo
1. Copia la dirección URL en la pantalla de lista ![ de reproducción donde hagas clic en Copiar junto a la dirección URL.](media/share.png)
Esta dirección URL ahora se puede insertar en la navegación del sitio o usarse en otras comunicaciones para llevar a los empleados directamente a esa lista de reproducción. 

### <a name="next-steps---drive-adoption"></a>Pasos siguientes: [impulsar la adopción](driveadoption.md)
