---
author: pkrebs
ms.author: pkrebs
title: Actualizar las formas de aprendizaje de Microsoft 365
ms.date: 07/06/2020
description: Actualizar las formas de aprendizaje de Microsoft 365
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 324bf41df1a6eec8d4646f3affdd48bedbbe3252
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000346"
---
# <a name="update-learning-pathways"></a>Actualización de formas de aprendizaje
Si tiene un sitio de Learning Pathways existente, puede actualizarlo para soporte multilingüe. Para actualizar las rutas de aprendizaje a la versión multilingüe 4.0, cargue el paquete de elementos web, customlearning.sppkg, en el Catálogo de aplicaciones del espacio empresarial de SharePoint. Al actualizar las rutas de aprendizaje:  

- Se mantienen todas las listas de reproducción y activos personalizados creados anteriormente
- Se mantiene la configuración para ocultar o mostrar contenido
- La plantilla de SharePoint caminos de aprendizaje no cambia
- Las páginas del sitio de caminos de aprendizaje no se traducen. Este trabajo debe realizarse manualmente

## <a name="read-the-learning-pathways-multilingual-overview"></a>Leer información general multilingüe sobre las rutas de aprendizaje
Para obtener información sobre cómo funciona el soporte multilingüe para las rutas de aprendizaje, lea la introducción multilingüe [caminos de aprendizaje.](custom_overview.md) 

## <a name="prerequisites-to-update"></a>Requisitos previos para actualizar
Antes de actualizar las rutas de aprendizaje, debe cumplirse el siguiente requisito previo:
- La persona que actualiza las rutas de aprendizaje debe ser el propietario de una colección de sitios del catálogo de aplicaciones del inquilino. Si la persona que aprovisiona las rutas de aprendizaje no es el propietario de una colección de sitios del Catálogo de aplicaciones, [complete estas instrucciones](addappadmin.md) y continúe. 

## <a name="set-language-settings"></a>Establecer la configuración de idioma 
Antes de actualizar las rutas de aprendizaje, establezca la configuración del idioma del sitio. Para habilitar la compatibilidad multilingüe para el sitio de rutas de aprendizaje, puede establecer habilitar páginas y noticias para que se traduzcan a varios **idiomas** en **On** y, a continuación, agregar los idiomas que desea admitir para el sitio.
1.  En el sitio Caminos de aprendizaje, seleccione **Configuración** en la parte superior derecha y, a continuación, seleccione **Información del sitio**.
2.  En la parte inferior del panel de información del sitio, seleccione **Ver toda la configuración del sitio**.
3.  En **Administración del sitio**, seleccione Configuración de **idioma**.
4.  En **Habilitar que las páginas y las noticias se traduzcan a varios idiomas,** establece el modificador de alternancia. 
- Para un sitio multiligual, deslice el botón de alternancia a **On** y, a continuación, vaya a la sección Agregar idiomas. 
- Para un sitio solo en inglés, deslice el botón de alternancia a **Desactivado**.

### <a name="add-languages"></a>Agregar idiomas
Las rutas de aprendizaje admiten nueve idiomas, solo debes agregar los idiomas que necesites. En los ejemplos usados en esta documentación, se agregará italiano. 
- En **Agregar o quitar idiomas de sitio,** empiece a escribir un nombre de idioma en Seleccionar o **escribir** un idioma, o elija un idioma en la lista desplegable. Puede repetir este paso para agregar varios idiomas. Puede agregar o quitar idiomas de su sitio en cualquier momento si vuelve a esta página.
 
### <a name="assign-translators"></a>Asignar traductores
Al definir la configuración de idioma para las rutas de aprendizaje, puede asignar traductores. Los traductores deben tener configurado un perfil de idioma extranjero. Para obtener más información acerca de los perfiles de idioma extranjero, vea [Crear sitios de comunicación multilingües, páginas y noticias.](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)  
- Para un idioma compatible, haga clic **en Seleccionar o escribir un traductor** y, a continuación, seleccione un traductor. 

## <a name="update-the-learning-pathways-web-part-package"></a>Actualizar el paquete de elementos web caminos de aprendizaje
En este paso, cargará el elemento web caminos de aprendizaje 4.0 en el Catálogo de aplicaciones de SharePoint y, a continuación, navegará a la página Administración de caminos de aprendizaje para iniciar el proceso de actualización.

### <a name="upload-the-web-part-package"></a>Cargar el paquete de elementos web
1.  Vaya al repositorio de aprendizaje personalizado de [GitHub,](https://github.com/pnp/custom-learning-office-365/tree/master/webpart)seleccione **customlearning.sppkg** y, a continuación, descárelo en una unidad local del equipo.
2.  Si aún no ha iniciado sesión, inicie sesión en su espacio empresarial con una cuenta de administrador de espacios empresariales o de administrador de la colección de sitios. 
3.  Haga **clic en Administrador** Mostrar  >  **todas** las características de  >  **SharePoint**  >  **Más**. 
4.  En **Aplicaciones,** haga clic **en Abrir**. 
5.  Haga **clic en Catálogo de aplicaciones** Distribuir aplicaciones para  >  **SharePoint**. 
6.  Haga clic **en Cargar**  >  **Elegir archivos**. 
7.  Seleccione el **archivo customlearning.sppkg** que descargó y haga clic **en Aceptar**  >  **implementar**. 

### <a name="complete-the-update"></a>Completar la actualización
1.  En el sitio Caminos de aprendizaje, seleccione Administración de caminos **de aprendizaje** en el **menú** Inicio. 
2.  Verá un mensaje que le preguntará si desea actualizar. 
![El mensaje le pide que inicie la actualización.](media/custom_update_adminprompt_ml.png)
3.  Haga clic en **Iniciar**. 
4. Una vez completada la actualización, haga clic **en Cerrar**. 

### <a name="next-steps"></a>Siguientes pasos
- Explore el [contenido predeterminado proporcionado](custom_exploresite.md) en el sitio y el elemento web.
- Para obtener más información acerca de la traducción de páginas de sitio, vea [Translate site pages](custom_translate_page_ml.md). 

