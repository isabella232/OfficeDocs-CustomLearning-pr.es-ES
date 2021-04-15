---
title: Preguntas más frecuentes sobre las rutas de aprendizaje de Microsoft 365
author: karuanag
ms.author: karuanag
ms.date: 02/10/2019
ms.topic: article
manager: alexb
audience: itpro
description: Información de preguntas más frecuentes para las rutas de aprendizaje de Microsoft 365.
ms.service: sharepoint-online
ms.openlocfilehash: f791d6421740c3458be525a7e306b10edab58259
ms.sourcegitcommit: 96ad347dc08694ce2af5a5d42bf1f753d1c30a65
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/13/2021
ms.locfileid: "51749408"
---
# <a name="frequently-asked-questions"></a>Preguntas frecuentes

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>Recientemente vi una entrada de blog en la que se cambia el nombre de Aprendizaje personalizado para Office 365 a Rutas de aprendizaje de Microsoft 365. ¿Hay otros cambios que se agregan a la solución como parte del esfuerzo de cambio de nombre? ¿Debo actualizar la solución en mi organización?

La versión de caminos de aprendizaje de Microsoft 365 es un esfuerzo de cambio de marca dedicado a cambiar el nombre de la solución para alinearse con la personal de marca de Microsoft 365. Si actualmente tiene aprendizaje personalizado para Office 365 que se ejecuta correctamente en su organización, no es necesario actualizar la solución en este momento.  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>¿Cuáles son los requisitos para instalar las rutas de aprendizaje de Microsoft 365 en mi entorno de inquilino?

- Tener habilitados SharePoint Online y los sitios de comunicación.
- La persona que aprovisionará CLO365 debe ser el administrador de inquilinos del inquilino de destino para su instalación.
- Un inquilino "Catálogo de aplicaciones" debe estar disponible dentro de la opción "Aplicaciones" del Centro de administración de SharePoint.
- Si se crea un nuevo Catálogo de aplicaciones, se requiere un tiempo de espera de 30 minutos o más para que el Catálogo de aplicaciones se aprovisione por completo. Al intentar aprovisionar rutas de aprendizaje de Microsoft 365 directamente después de crear el catálogo de aplicaciones de inquilino, se producirá un error de aprovisionamiento de la solución de caminos de aprendizaje. 
- La persona que aprovisionará CLO365 debe ser administrador de la colección de sitios del catálogo de aplicaciones en el inquilino de destino para su instalación.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Por qué Microsoft pide permisos de inquilino al instalar rutas de aprendizaje de Microsoft 365 

- El servicio de aprovisionamiento de SharePoint Online usa los permisos para aprovisionar el sitio de SharePoint Caminos de aprendizaje, crear las páginas del sitio e instalar la aplicación caminos de aprendizaje de Microsoft 365 en su inquilino. Ese es el único motivo por el que solicitamos los permisos. Sin los permisos solicitados, el Servicio de aprovisionamiento de SharePoint no puede ejecutar los comandos que instalan automáticamente la plantilla de sitio de caminos de aprendizaje y el elemento web. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>¿Cuáles son las implicaciones de que las rutas de aprendizaje de Microsoft 365 estén en una versión preliminar beta? 

Las rutas de aprendizaje de Microsoft 365 se encuentran actualmente en Beta Preview. Tenga en cuenta lo siguiente al evaluar, planear e implementar las rutas de aprendizaje de Microsoft 365:

- Al igual que con cualquier solución Beta, nuestro equipo de administración de servicios se reserva el derecho de realizar cambios en el servicio y sus componentes. Como está resolviendo errores y problemas de experiencia de usuario activamente, es probable que deba actualizar WebPart.
- Para actualizar el elemento web, deberá descargarlo desde nuestro repositorio de GitHub y cargarlo en el catálogo de aplicaciones de inquilino. Consulte la sección "Actualización de la solución" del archivo [Léame](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) de rutas de aprendizaje de Microsoft 365. 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>¿En qué idiomas están disponibles las rutas de aprendizaje de Microsoft 365?

Actualmente, las rutas de aprendizaje de Microsoft 365 solo están disponibles en inglés. El aprovisionamiento automático de un extremo a otro solo funciona con inquilinos en inglés. Tenemos previsto implementar la compatibilidad multilingüe para los siguientes idiomas en el segundo trimestre de 2020. 

- Chino (simplificado) 
- Francés  
- Alemán 
- Italiano (Italia) 
- Japonés (Japón)  
- Portugués (Brasil) 
- Ruso (ruso)  
- Español 

> La compatibilidad con el idioma neerlandés no se incluirá en la próxima versión de compatibilidad con varios idiomas para las rutas de aprendizaje. Seguiremos evaluando nuevas opciones de idioma en el futuro.

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>¿Cuánto tiempo se necesita para instalar el sitio en nuestro entorno de inquilino?

En función de nuestras pruebas de la instalación, debe tardar menos de 15 minutos. No se incluye el tiempo necesario para personalizar el sitio y adaptarlo a sus necesidades.

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>¿Las rutas de aprendizaje de Microsoft 365 son una solución de código abierto y cuáles son las implicaciones?

Las rutas de aprendizaje de Microsoft 365 son una solución de software de código abierto (OSS) y, como tal, conlleva un conjunto de ventajas y consideraciones para el sistema operativo:

#### <a name="benefits"></a>Ventajas 
- Las rutas de aprendizaje de **Microsoft 365 son una solución gratuita:** Los clientes pueden instalar la solución en su inquilino, personalizarla y ponerla a disposición de los usuarios finales
- **El sistema operativo permite un desarrollo y colaboración rápidos:**  Todas las soluciones de código abierto están disponibles para una amplia comunidad de colaboradores.  Microsoft está comprometido con este método para impulsar la innovación.  Para garantizar que ofrecemos una experiencia que beneficia al conjunto más amplio de nuestros clientes, nuestro equipo principal de administración de servicios se reservará el derecho de determinar qué contribuciones se combinan en nuestra compilación oficial.  
- **El sistema operativo habilita la colaboración con partners:** Microsoft está trabajando con varios partners de aprendizaje para apoyar sus esfuerzos para futuras extensiones y contribuciones a las rutas de aprendizaje de Microsoft 365. Proporcionaremos más información a medida que estos planes estén finalizados. 
    
#### <a name="implications"></a>Implicaciones
- **OSS no es un producto comercialmente disponible:** Los productos comerciales incluyen actualización y revisión y se incluyen en contratos de soporte técnico basados en tarifas. Aunque Actualmente Microsoft ofrece documentación, actualización y revisión para las rutas de aprendizaje de Microsoft 365, se basa en nuestro compromiso de mejorar este escenario empresarial en particular. Nuestros planes son seguir invirtiendo en caminos de aprendizaje, tener en cuenta que nuestro equipo de administración de servicios puede cambiar estrategias en el futuro. Los cambios futuros en las rutas de aprendizaje de Microsoft 365 se comunicarán antes de que entren en vigor. 
- Como sistema operativo, las rutas de aprendizaje de **Microsoft 365** se admiten a través de una lista de problemas en línea en GitHub: las rutas de aprendizaje de Microsoft 365 no están cubiertas por ningún contrato de soporte técnico de Microsoft existente. Los problemas enviados son triaged por microsoft 365 caminos de aprendizaje propietarios de servicios y la comunidad. Los niveles de servicio de resolución de problemas NO están al mismo nivel que un contrato de soporte técnico de Microsoft de pago.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>¿Podemos convertir las rutas de aprendizaje de Microsoft 365 en un subsitio de nuestra colección de sitios principal de SharePoint?

No. El sitio se basa en una plantilla de sitio de comunicación, que siempre está pensada para ser una colección de sitios raíz.

> [!NOTE]
> Es importante tener en cuenta los permisos que los usuarios finales necesitarán para acceder al sitio. La mayoría de las organizaciones han definido grupos de usuarios o de seguridad. Debe agregar los grupos de seguridad adecuados al nuevo portal de formación una vez que esté listo para iniciarlo en su comunidad de empleados.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>Necesito reinstalar el sitio; ¿Qué debo hacer?

Siga las instrucciones de instalación [publicadas aquí](custom_provision.md).

> [!NOTE]
> Si ha deshabilitado la telemetría en la instalación anterior y desea continuar con la telemetría deshabilitada, deberá seguir las instrucciones para deshabilitar la telemetría aquí.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Hemos realizado actualizaciones de nuestra implementación de las rutas de aprendizaje de Microsoft 365. ¿Perderemos estas actualizaciones (realizadas en plantillas de sitio, listas de reproducción) si reinstalamos el sitio?

Las personalizaciones de páginas individuales y listas de reproducción personalizadas se perderán si reinstala el sitio en la instalación actual.  
