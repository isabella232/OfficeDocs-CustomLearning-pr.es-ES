---
author: pkrebs
ms.author: pkrebs
title: Actualización de las rutas de aprendizaje para la compatibilidad multilingüe
ms.date: 05/20/2019
description: Actualización de las rutas de aprendizaje para la compatibilidad multilingüe
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: 37a9b77ee45b8ae1ae4973f171c32de11fb530e1
ms.sourcegitcommit: 1f080ed4cf3687f922907304db3fd7a06aa9d501
ms.translationtype: Auto
ms.contentlocale: es-ES
ms.lasthandoff: 07/02/2020
ms.locfileid: "45031706"
---
# <a name="update-learning-pathways-for-multilingual-support"></a>Actualización de las rutas de aprendizaje para la compatibilidad multilingüe
Si tiene un sitio de caminos de aprendizaje existente, puede actualizarlo para la compatibilidad multilingüe. Para actualizar las rutas de aprendizaje a la versión multilingüe de 4,0, cargue el paquete de elementos Web, customlearning. sppkg, en el catálogo de aplicaciones del espacio empresarial de SharePoint. Al actualizar rutas de aprendizaje:  

- Se mantienen todos los activos y listas de reproducción personalizados creados anteriormente
- Se mantiene la configuración para ocultar o mostrar contenido
- La plantilla de SharePoint de rutas de aprendizaje permanece sin cambios
- Las páginas del sitio de las rutas de aprendizaje no se traducen. Este trabajo debe realizarse manualmente

## <a name="read-the-learning-pathways-multilingual-overview"></a>Leer la introducción multilingüe de las rutas de aprendizaje
Para obtener información sobre cómo funciona la compatibilidad multilingüe para las rutas de aprendizaje, lea la [Introducción multilingüe](custom_overview_ml.md)de las rutas de aprendizaje. 

## <a name="prerequisites-to-update"></a>Requisitos previos para la actualización
Antes de actualizar las rutas de aprendizaje, es necesario cumplir los siguientes requisitos previos:
- La persona que actualice las rutas de aprendizaje debe ser un propietario de la colección de sitios del catálogo de aplicaciones del espacio empresarial. Si la persona que aprovisiona las rutas de aprendizaje no es un propietario de la colección de sitios del catálogo de aplicaciones, [complete estas instrucciones](addappadmin.md) y continúe. 

## <a name="set-language-settings"></a>Establecer la configuración de idioma 
Antes de actualizar las rutas de aprendizaje, establezca la configuración de idioma del sitio. Para habilitar la compatibilidad multilingüe con el sitio de caminos de aprendizaje, puede configurar las **páginas y noticias de habilitar para que se traduzcan en varios idiomas** y, a **continuación, agregar**los idiomas que desea que sean compatibles con el sitio.
1.  Desde el sitio de caminos de aprendizaje, seleccione **configuración** de la parte superior derecha y, a continuación, seleccione **información del sitio**.
2.  En la parte inferior del panel de información del sitio, seleccione **ver toda la configuración del sitio**.
3.  En **Administración del sitio**, seleccione **configuración de idioma**.
4.  En **Habilitar páginas y noticias para que se traduzcan a varios idiomas**, establezca el modificador para alternar. 
- Para un sitio de multiligual, deslice el botón de alternancia a **activado**y, a continuación, vaya a la sección agregar idiomas. 
- Para un sitio de solo inglés, deslice el botón de alternancia a **desactivado**.

### <a name="add-languages"></a>Agregar idiomas
Las rutas de aprendizaje admiten nueve idiomas, solo debe agregar los idiomas que necesite. En los ejemplos que se usan en esta documentación, se agregará italiano. 
- En **Agregar o quitar idiomas del sitio**, escriba el nombre de un idioma en **seleccionar o escriba un idioma**o seleccione un idioma de la lista desplegable. Puede repetir este paso para agregar varios idiomas. Puede Agregar o quitar idiomas de su sitio en cualquier momento volviendo a esta página.
 
### <a name="assign-translators"></a>Asignar traductores
Al definir la configuración de idioma para las rutas de aprendizaje, puede asignar traductores. Los traductores deben tener configurado un perfil de idioma extranjero. Para obtener más información acerca de los perfiles de idiomas externos, consulte [crear sitios de comunicación multilingües, páginas y noticias](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).  
- Para un idioma compatible, haga clic en **seleccionar o escriba un traductor** y, a continuación, seleccione un traductor. 

## <a name="update-the-learning-pathways-web-part-package"></a>Actualizar el paquete de elementos Web de rutas de aprendizaje
En este paso, carga el elemento Web caminos de aprendizaje 4,0 en el catálogo de aplicaciones de SharePoint y, a continuación, navega a la página de administración de caminos de aprendizaje para iniciar el proceso de actualización.

### <a name="upload-the-web-part-package"></a>Cargar el paquete de elementos Web
1.  Vaya a la ubicación de recursos compartidos multilingües en Teams y descargue **customlearning. sppkg** a una unidad local de su PC. 
2.  Si aún no ha iniciado sesión, inicie sesión en su inquilino con una cuenta de administrador de inquilinos o de administración de la colección de sitios. 
3.  Haga clic en **Administración**,  >  **Mostrar todas**  >  **SharePoint**  >  **las características más**de SharePoint. 
4.  En **aplicaciones**, haga clic en **abrir**. 
5.  Haga clic en **Catálogo**  >  **de aplicaciones distribuir aplicaciones para SharePoint**. 
6.  Haga clic en **cargar**  >  **archivos de selección**. 
7.  Seleccione el archivo **customlearning. sppkg** que ha descargado y haga clic en **Aceptar**  >  **implementar**. 

### <a name="complete-the-update"></a>Completar la actualización
1.  Desde el sitio de caminos de aprendizaje, seleccione **aprendizaje de rutas de aprendizaje** en el menú de **Inicio** . 
2.  Verá un mensaje en el que se le preguntará si desea actualizar. 
![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)
3.  Haga clic en **Iniciar**. 
4. Una vez finalizada la actualización, haga clic en **cerrar**. 

### <a name="next-steps"></a>Siguientes pasos
- Explore el [contenido predeterminado](custom_exploresite.md) proporcionado en el sitio y el elemento Web.
- Para obtener más información acerca de la conversión de páginas del sitio, consulte [translate site pages](custom_translate_page_ml.md). 

