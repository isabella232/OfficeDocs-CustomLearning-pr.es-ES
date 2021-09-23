---
author: karuanag
ms.author: karuanag
manager: alexb
title: Personalizar y compartir listas de reproducción
ms.date: 02/10/2019
description: Crear listas de reproducción personalizadas a partir de contenido existente o páginas SharePoint nuevas
ms.service: sharepoint-online
audience: itpro
ms.topic: article
ms.openlocfilehash: 31310a6737543a3006f810ffc6b9522d6c9583da
ms.sourcegitcommit: a93cae8ea6e3c1141d7266d04131b69f2c2498cb
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/23/2021
ms.locfileid: "59485341"
---
# <a name="customize-and-share-playlists"></a>Personalizar y compartir listas de reproducción

## <a name="create-a-playlist"></a>Crear una lista de reproducción

Una lista de reproducción es una compilación de "activos". Un "activo" es una página SharePoint o un elemento existente del contenido de aprendizaje de Microsoft. Cuando creas una lista de reproducción, seleccionas activos que van juntos para crear una ruta de aprendizaje para el usuario.  

La ventaja de agregar SharePoint páginas es que puedes crear páginas SharePoint con vídeos o vídeos de YouTube hospedados en tu organización. También puede crear páginas con formularios u otro Office 365 contenido.  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a>Paso 1: Crear una página SharePoint para la lista de reproducción
En este ejemplo, primero crearemos una página SharePoint agregar a la lista de reproducción. Crearemos una página con un elemento web de vídeo de YouTube y un elemento web de texto.  Estas instrucciones suponen que usa el servicio SharePoint online. 

#### <a name="create-a-new-page"></a>Crear una nueva página
1.  Seleccione el Configuración menú > Contenido del sitio > página > Página > sitio.
2.  En el área de título, escriba Usar el Teams cuadro de comando
3.  Seleccione la sección Agregar un nuevo y, a continuación, dos columnas.

    ![agregar dos columnas](media/clo365addtwocolumn.png)

4.  En el cuadro izquierdo, seleccione Agregar un nuevo elemento web y, a continuación, seleccione Insertar. 
5.  En un explorador web, vaya a esta dirección URL https://youtu.be/wYrRCRphrp0 y obtenga el código de inserción del vídeo. 
6.  En el SharePoint web, seleccione Agregar código incrustado y, a continuación, péguelo en el cuadro Insertar. 
7.  En el cuadro derecho, seleccione Agregar un nuevo elemento web y, a continuación, seleccione Texto. 
8.  En un explorador web, vaya a esta dirección URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b y copie la opción Pruébalo. Instrucciones de la página y péguelas en el elemento web de texto. La página debe tener el siguiente aspecto. 
   ![Página Insertar](media/clo365teamscommandbox.png)
9.  Haga **clic en** Publicar y, a continuación, copie la dirección URL de la página y péguela en Bloc de notas

#### <a name="step-2-create-the-playlist"></a>Paso 2: Crear la lista de reproducción

1. Vaya a la **página Administración Learning personalizada** en la experiencia del sitio.
   ![Administrador personalizado](media/custom_admin.png)
1. Asegúrese de **que Categoría** está seleccionada 
1. Haz clic en la categoría en la que quieres que aparezca la nueva lista de reproducción
1. Junto al nombre de categoría, haz clic en el símbolo más ![ Agregar lista de reproducción personalizada](media/custom_addplay.png)

1. Rellene los valores como se muestra en el ejemplo siguiente y seleccione **Crear**. 
  ![Detalles de listas de reproducción personalizadas](media/custom_details.png)
- **Título:** nombre para mostrar de la lista de reproducción
- **Descripción:** información sobre lo que se va a aprender
- **Categoría:** preseleccionada en función de la selección inicial
- **Subcategoría:** preseleccionada en función de la selección inicial
- **Tecnología:** seleccione según corresponda
- **Nivel:** principiante, intermedio o avanzado
- **Audiencia:** esto le permite dirigir el contenido en función de una lista predefinida de roles proporcionados por Microsoft.

6. Haga clic **en Guardar detalle**

> [!TIP]
> Puedes personalizar la imagen de icono de la lista de reproducción.  Haga clic en el icono de imagen e inserte una dirección URL de una imagen cargada anteriormente.  Asegúrese de que la imagen se encuentra dentro de la colección de sitios Learning personalizada o en otra ubicación en la que todos los usuarios tendrán acceso al archivo.  
![Imagen personalizada](media/custom_image.png)

#### <a name="step-3-add-assets-to-the-playlist"></a>Paso 3: Agregar activos a la lista de reproducción
En este paso, agregarás activos existentes de Microsoft y la SharePoint que creaste a la lista de reproducción. 

1. Una vez guardados los detalles de la lista de reproducción, puedes usar la búsqueda de activos existentes.
1. **Escribe cualquier término de búsqueda** para ver una lista de activos predefinidos que están disponibles en otras listas de reproducción. **Haz clic en el nombre** de un activo para incluirlo en la nueva lista de reproducción.

    ![Lista de reproducción de búsqueda personalizada](media/custom_slist.png)

También puede agregar la página SharePoint que creó anteriormente o crear una desde cero en la experiencia.

1. Haga clic en la **opción Nuevo activo** en el cuadro de diálogo Activos de lista de reproducción
1. Dé a su activo un **título**. Una vez especificado, las opciones adicionales ![ mostrarán nueva página personalizada](media/custom_newpage.png)
1. Ahora puedes crear una nueva página de activos en SharePoint Online o escribir la dirección URL de una página existente para agregarla a la lista de reproducción personalizada. 
1. **Los** campos Category , **Sub Category** y **Technology** se rellenarán previamente en función de las selecciones anteriores para esta lista de reproducción.
1. Realice las selecciones adecuadas para Nivel y Audiencia para este activo individual.  
1. Haga **clic en Guardar activo** para agregarlo a la lista de reproducción personalizada
1. Repita estos pasos, ya sea buscando o agregando páginas individuales, hasta que se complete la lista de reproducción. 
1. Haga **clic en Cerrar lista de reproducción** para guardar

La lista de reproducción con este contenido ahora estará disponible en cualquier lugar en el que haya instalado o incrustado el elemento web Learning personalizado. 

> [!NOTE]
> Si cometes un error una vez cerrada la lista de reproducción, puedes eliminarla de la categoría haciendo clic en la X situada junto al nombre de la lista de reproducción.  

#### <a name="things-to-think-about"></a>Cosas en las que pensar

Las listas de reproducción personalizadas se pueden usar para ayudar a los usuarios finales en una variedad de tareas.  ¿Tiene un formulario de solicitud de tiempo libre?  ¿Un formulario para solicitar equipamiento de hardware?  Los activos de aprendizaje existentes se pueden programar en la experiencia.  

## <a name="share-playlists"></a>Compartir listas de reproducción

1. Navegue a cualquier lista de reproducción dentro del elemento web o la experiencia del sitio
1. En la esquina superior izquierda verá tres iconos
1. Haga clic en el icono que representa un vínculo
1. Copiar la dirección URL en la lista de reproducción

   ![Compartir lista de reproducción Esta dirección URL ahora se puede insertar en la navegación del sitio o usarse en otras comunicaciones para llevar a los empleados ](media/share.png) directamente a esa lista de reproducción. 

### <a name="next-steps---drive-adoption"></a>Pasos siguientes: [impulsar la adopción](driveadoption.md)
