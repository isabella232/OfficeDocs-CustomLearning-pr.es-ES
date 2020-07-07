---
author: pkrebs
ms.author: pkrebs
title: Opción de instalación para rutas de aprendizaje
ms.date: 07/16/2020
description: Opción de instalación para rutas de aprendizaje
ms.openlocfilehash: 1434a06fbe5f374de7b2f2e4fa471a8eda5ac871
ms.sourcegitcommit: ba0cddd12dd8687ec4b97c26174fdda09de83b05
ms.contentlocale: es-ES
ms.lasthandoff: 07/06/2020
ms.locfileid: "45043222"
---
# <a name="setup-options-for-multilingual-learning-pathways"></a>Opciones de instalación para rutas de aprendizaje multilingües
Con el lanzamiento de características multilingües para los sitios de comunicaciones de SharePoint Online, los caminos de aprendizaje ahora ofrecen compatibilidad para varios idiomas. Puede configurar rutas de aprendizaje en diferentes tipos de formas para satisfacer las necesidades de su organización. Para ayudarle a decidir cuál es la mejor ruta de acceso para su organización, hemos descrito las opciones de instalación. 

## <a name="new-install-scenarios"></a>Nuevos escenarios de instalación
Los "nuevos escenarios de instalación" explican las opciones para instalar una nueva instancia de las rutas de aprendizaje mediante el servicio de libro de apariencia de Microsoft 365. 

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>Escenario 1: no se han instalado caminos de aprendizaje y se necesita la compatibilidad multilingüe de rutas de aprendizaje 
Si no ha instalado rutas de aprendizaje y necesita varios idiomas, puede usar el servicio de libro de apariencia de Microsoft 365 para instalar una nueva solución de caminos de aprendizaje con soporte para nueve idiomas. El inglés será el idioma predeterminado y no se podrá cambiar. 
- Para aprovisionar una nueva solución de caminos de aprendizaje con el inglés como idioma predeterminado del sitio, vea [provision a New Learning Pathways Solution](custom_provision.md).

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>Escenario 2: hemos instalado caminos de aprendizaje pero no los usan actualmente o no han realizado ninguna personalización en el sitio o las listas de reproducción 
Si ha instalado caminos de aprendizaje pero no los usa de forma activa o no ha realizado ninguna personalización en el sitio o las listas de reproducción, puede usar el servicio de libro de apariencia de Microsoft 365 para instalar una nueva solución con soporte para nueve idiomas. El inglés será el idioma predeterminado y no se podrá cambiar. 
- Para aprovisionar una nueva solución de caminos de aprendizaje con el inglés como idioma predeterminado del sitio, vea [provision a New Learning Pathways Solution](custom_provision.md).

### <a name="scenario-3-we-havent-installed-learning-pathways-and-dont-need-multilingual-support"></a>Escenario 3: no hemos instalado caminos de aprendizaje y no es necesario que admita multilingüe 
Si no ha instalado las rutas de aprendizaje y no necesita compatibilidad multilingüe, puede instalarla desde el servicio de libro de apariencia de Microsoft 365. El idioma predeterminado será el inglés. Después de la instalación, debe desactivar la compatibilidad multilingüe. 
- Para aprovisionar una nueva solución de caminos de aprendizaje sin compatibilidad multilingüe, vea [provision a New Learning Pathways Solution](custom_provision.md).

## <a name="update-learning-pathways-with-a-web-part-upload-scenarios"></a>Actualización de las rutas de aprendizaje (con una carga de elementos Web)
Si tiene instalada una versión existente de las rutas de aprendizaje, puede cargar el elemento Web de rutas de aprendizaje en el catálogo de aplicaciones de SharePoint para habilitar la compatibilidad multilingüe. 

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-dont-need-multilingual-support"></a>Escenario 1: Necesitamos actualizar una versión existente de las rutas de aprendizaje, pero no es necesario que admita multilingüe
Puede actualizar las rutas de aprendizaje de la versión 4,0 sin la compatibilidad multilingüe. Con la actualización, obtiene un par de características nuevas, incluido un selector de imagen para listas de reproducción personalizadas y subcategorías. 

- Para actualizar una solución de vías de aprendizaje existente sin compatibilidad multilingüe, consulte [Update Learning Pathways for Multilingual Support](custom_update.md). El proceso de actualización de la compatibilidad multilingüe no es el mismo que el de la compatibilidad multilingüe, sino con menos pasos. 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>Escenario 2: es necesario actualizar a la compatibilidad multilingüe y el idioma predeterminado de la colección de sitios es nuestro idioma predeterminado
Las rutas de aprendizaje de la versión 4. O serán compatibles con páginas multilingües de la colección de sitios. Además de la compatibilidad multilingüe, obtiene un par de características nuevas, incluido un selector de imagen para listas de reproducción personalizadas y subcategorías. 
- Para actualizar un sitio existente de rutas de aprendizaje soporte multilingüe, consulte [Update Learning Pathways for Multilingual Support](custom_update.md). 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>Actualización de rutas de aprendizaje para soporte multilingüe con instalación manual 
A continuación, se describen los escenarios para actualizar una instancia existente de la solución de rutas de aprendizaje a la versión multilingüe de la versión 4,0 mediante la instalación manual del elemento Web de rutas de aprendizaje. 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>Escenario 1: es necesario la compatibilidad multilingüe y el idioma predeterminado de la colección de sitios no es nuestro idioma predeterminado: sin contenido personalizado 
Las rutas de aprendizaje de la versión 4,0 serán compatibles con este escenario. Sin embargo, en este escenario se presupone que no tiene contenido ni listas de reproducción personalizados en el sitio existente. Para este escenario, puede crear un nuevo sitio de comunicación de SharePoint Online con su idioma predeterminado, cargar el elemento Web y, a continuación, configurar manualmente las rutas de aprendizaje con un script de PowerShell. 
- Para configurar rutas de aprendizaje para la compatibilidad multilingüe con su idioma predeterminado, consulte [instalación manual de rutas de aprendizaje para soporte multilingüe](custom_manualsetup.md).

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>Escenario 2: es necesario la compatibilidad multilingüe y el idioma predeterminado de la colección de sitios no es nuestro idioma predeterminado, además de contenido personalizado 
Para este escenario, puede crear un nuevo sitio de comunicación de SharePoint Online con su idioma predeterminado, cargar el elemento Web y, a continuación, configurar manualmente las rutas de aprendizaje con un script de PowerShell. 

Después de restablecer el sitio de caminos de aprendizaje siguiendo los pasos anteriores, tendrá que mover el contenido de la lista de **CustomPlaylists** y la lista de **CustomAssets** . Si lo desea, también puede mover las páginas personalizadas reales que componen los activos personalizados si residen en el sitio de caminos de aprendizaje existente y su intención es eliminarla. La tarea puede ser difícil porque para todos los elementos de la lista **CustomPlaylists** , el identificador del elemento de lista de la lista **CustomAssets** está escondido en el campo JSONData de cada elemento de lista de lista de reproducción. Por lo tanto, simplemente mover el contenido de la lista de **CustomPlaylists** de un sitio a otro no será suficiente. Además, la lista **CustomAssets** contiene la dirección URL absoluta de la página del activo personalizado en el campo JSONData del elemento de lista. Si los activos no se mueven y no se cambia el nombre del sitio (lo que cambia la dirección URL absoluta a la página del activo), entonces **CustomAssets** puede permanecer. Pero tendrá que corregir manualmente las entradas. Teniendo en cuenta la complejidad de este tipo de migración, sugerimos que considere la posibilidad de enumerar uno de nuestros asociados de caminos de aprendizaje para ayudarle a realizar esta transición.
- Para configurar rutas de aprendizaje para la compatibilidad multilingüe con su idioma predeterminado, consulte [instalación manual de rutas de aprendizaje para soporte multilingüe](custom_manualsetup.md).