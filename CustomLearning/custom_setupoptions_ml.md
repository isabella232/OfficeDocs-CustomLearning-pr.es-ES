---
author: pkrebs
ms.author: pkrebs
title: Opciones de configuración para rutas de aprendizaje multilingües
ms.date: 07/6/2020
description: Opciones de configuración para rutas de aprendizaje multilingües
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 1384885adc1d7119658bf968e18e8859c784ef37
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999316"
---
# <a name="setup-options-for-multilingual-learning-pathways"></a>Opciones de configuración para rutas de aprendizaje multilingües
Con el lanzamiento de características multilingües para sitios de comunicaciones de SharePoint Online, las rutas de aprendizaje ahora ofrecen compatibilidad con varios idiomas. Puede configurar rutas de aprendizaje de diferentes tipos de formas para satisfacer las necesidades de su organización. Para ayudarle a decidir la mejor ruta de acceso para su organización, hemos descrito las opciones de configuración. 

## <a name="new-install-scenarios"></a>Nuevos escenarios de instalación
Los "nuevos escenarios de instalación" explican las opciones para instalar una nueva instancia de las rutas de aprendizaje mediante el servicio de aprovisionamiento de SharePoint, ahora disponible en el libro de apariencias de SharePoint.

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>Escenario 1: No hemos instalado caminos de aprendizaje y necesitamos soporte multilingüe para las rutas de aprendizaje 
Si no ha instalado caminos de aprendizaje y necesita varios idiomas, puede usar el Servicio de aprovisionamiento de SharePoint para instalar una nueva solución de caminos de aprendizaje con compatibilidad con nueve idiomas. El inglés será el idioma predeterminado y no se puede cambiar. 
- Para aprovisionar una nueva solución de caminos de aprendizaje con inglés como idioma predeterminado para el sitio, vea [Provision a new learning pathways solution](custom_provision_ml.md).

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>Escenario 2: Instalamos rutas de aprendizaje, pero no la estamos usando actualmente o no hemos realizado ninguna personalización en el sitio o listas de reproducción 
Si instaló rutas de aprendizaje pero no la está usando activamente o no ha realizado personalizaciones en el sitio o listas de reproducción, puede usar el Servicio de aprovisionamiento de SharePoint para instalar una nueva solución con compatibilidad con nueve idiomas. El inglés será el idioma predeterminado y no se puede cambiar. 
- Para aprovisionar una nueva solución de caminos de aprendizaje con inglés como idioma predeterminado para el sitio, vea [Provision a new learning pathways solution](custom_provision_ml.md).

### <a name="scenario-3-we-havent-installed-learning-pathways-and-dont-need-multilingual-support"></a>Escenario 3: No hemos instalado caminos de aprendizaje y no necesitamos soporte multilingüe 
Si no ha instalado caminos de aprendizaje y no necesita soporte multilingüe, puede instalarlo desde el servicio de aprovisionamiento de SharePoint. El inglés será el idioma predeterminado. Después de la instalación, debe desactivar la compatibilidad multilingüe. 
- Para aprovisionar una nueva solución de caminos de aprendizaje sin compatibilidad multilingüe, vea [Provision a new learning pathways solution](custom_provision_ml.md).

## <a name="update-learning-pathways-with-a-web-part-upload-scenarios"></a>Actualizar escenarios de rutas de aprendizaje (con una carga de elementos web)
Si tiene instalada una versión existente de las rutas de aprendizaje, puede cargar el elemento web caminos de aprendizaje en el Catálogo de aplicaciones de SharePoint para habilitar la compatibilidad multilingüe. 

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-dont-need-multilingual-support"></a>Escenario 1: Necesitamos actualizar una versión existente de las rutas de aprendizaje, pero no necesitamos soporte multilingüe
Puede actualizar las rutas de aprendizaje versión 4.0 sin compatibilidad multilingüe. Con la actualización, obtienes un par de características nuevas, incluido un selector de imágenes para listas de reproducción personalizadas y subcategorías. 

- Para actualizar una solución de caminos de aprendizaje existente sin compatibilidad multilingüe, vea [Update learning pathways for multilingual support](custom_update_ml.md). El proceso de actualización sin compatibilidad multilingüe es el mismo que con la compatibilidad multilingüe, pero con menos pasos. 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>Escenario 2: Debemos actualizar a soporte multilingüe y el idioma predeterminado de la colección de sitios es nuestro idioma predeterminado
Caminos de aprendizaje versión 4.O admitirá páginas multilingües en la colección de sitios. Además de la compatibilidad multilingüe, obtienes un par de nuevas características, incluido un selector de imágenes para listas de reproducción personalizadas y subcategorías. 
- Para actualizar una compatibilidad multilingüe de sitios de rutas de aprendizaje existentes, vea [Actualizar rutas de aprendizaje para soporte multilingüe.](custom_update_ml.md) 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>Actualizar las rutas de aprendizaje para la compatibilidad multilingüe con la instalación manual 
A continuación se describen los escenarios para actualizar una instancia existente de la solución de caminos de aprendizaje a la versión 4.0 multilingüe mediante la instalación manual del elemento web caminos de aprendizaje. 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>Escenario 1: Necesitamos soporte multilingüe y el idioma predeterminado de la colección de sitios no es nuestro idioma predeterminado: no hay contenido personalizado 
Las rutas de aprendizaje versión 4.0 admiten este escenario. Sin embargo, este escenario supone que no tienes contenido personalizado ni listas de reproducción en el sitio existente. Para este escenario, puede crear un nuevo sitio de comunicación de SharePoint Online con el idioma predeterminado, cargar el elemento web y, a continuación, configurar manualmente las rutas de aprendizaje con un script de PowerShell. 
- Para configurar las rutas de aprendizaje para la compatibilidad multilingüe con el idioma predeterminado, consulte Instalación manual de caminos de aprendizaje [para soporte multilingüe.](custom_manualsetup_ml.md)

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>Escenario 2: Necesitamos soporte multilingüe y el idioma predeterminado de la colección de sitios no es nuestro idioma predeterminado, además de que tenemos contenido personalizado 
Para este escenario, puede crear un nuevo sitio de comunicación de SharePoint Online con el idioma predeterminado, cargar el elemento web y, a continuación, configurar manualmente las rutas de aprendizaje con un script de PowerShell. 

Después de restablecer el sitio de rutas de aprendizaje siguiendo los pasos anteriores, deberá mover el contenido de la lista **CustomPlaylists** y la lista **CustomAssets.** También puede, opcionalmente, mover las páginas personalizadas reales que forma parte de los activos personalizados si viven en el sitio de rutas de aprendizaje existentes y su intención es eliminarlo. La tarea puede ser difícil porque para todos los elementos de la lista **CustomPlaylists,** el identificador del elemento de lista de la **lista CustomAssets** está en el campo JSONData de cada elemento de lista de listas de reproducción. Por lo tanto, simplemente mover el contenido de la **lista CustomPlaylists** de un sitio al otro no será suficiente. Además, la **lista CustomAssets** contiene la dirección URL absoluta de la página del activo personalizado en el campo JSONData del elemento de lista. Si los activos no se mueven y no se cambia el nombre del sitio (cambiando así la dirección URL absoluta a la página del activo), **customAssets** puede permanecer. Pero tendrá que corregir manualmente las entradas. Dada la complejidad de este tipo de migración, le recomendamos que considere la posibilidad de alistar uno de nuestros asociados de caminos de aprendizaje para ayudarle a realizar esta transición.
- Para configurar las rutas de aprendizaje para la compatibilidad multilingüe con el idioma predeterminado, consulte Instalación manual de caminos de aprendizaje [para soporte multilingüe.](custom_manualsetup_ml.md)

