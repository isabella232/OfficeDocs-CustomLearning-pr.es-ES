---
title: Microsoft 365 preguntas más frecuentes sobre las rutas de aprendizaje
author: karuanag
ms.author: karuanag
manager: alexb
ms.date: 02/10/2019
description: Información de preguntas más frecuentes para Microsoft 365 de aprendizaje
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: 82a7e777490e13fde6fef5add40beee417050027
ms.sourcegitcommit: d05381fc4a58cf2949773d73877bacc5ef3a7ca6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/01/2021
ms.locfileid: "60048727"
---
# <a name="frequently-asked-questions"></a>Preguntas frecuentes

## <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>¿Cuáles son los requisitos para instalar Microsoft 365 de aprendizaje en mi entorno de inquilino?

- Tener habilitados SharePoint Online y los sitios de comunicación.
- La persona que va a aprovisionar Microsoft 365 de aprendizaje debe ser el administrador de inquilinos del espacio empresarial de destino para su instalación.
- Un espacio empresarial "Catálogo de aplicaciones" debe estar disponible dentro de la opción "Aplicaciones" del Centro SharePoint administración.
- Si se crea un nuevo Catálogo de aplicaciones, se requiere un tiempo de espera de 30 minutos o más para que el Catálogo de aplicaciones se aprovisione por completo. Si se intenta aprovisionar Microsoft 365 de aprendizaje directamente después de crear el catálogo de aplicaciones del espacio empresarial, se producirá un error de aprovisionamiento de la solución de caminos de aprendizaje.
- La persona que va a aprovisionar Microsoft 365 de aprendizaje debe ser un administrador de la colección de sitios del catálogo de aplicaciones en el espacio empresarial de destino para su instalación.

## <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>¿Por qué Microsoft pide permisos de inquilino al instalar Microsoft 365 de aprendizaje?

El servicio SharePoint Online Provisioning usa los permisos para aprovisionar el sitio de Learning Pathways SharePoint, crear las páginas del sitio e instalar la aplicación de caminos de aprendizaje de Microsoft 365 en su inquilino. Ese es el único motivo por el que solicitamos los permisos. Sin los permisos solicitados, el servicio SharePoint aprovisionar no puede ejecutar los comandos que instalan automáticamente la plantilla de sitio y el elemento web de caminos de aprendizaje.
![Captura de pantalla de la solicitud de permisos](media/faqs-permissions-request-screenshot.png "Solicitud de permisos") Si aún tiene dudas sobre este nivel de acceso, puede conceder los permisos e implementar las plantillas de sitio que le interesen y, a continuación, quitar inmediatamente los permisos concedidos a la aplicación en la Tienda de aplicaciones de [Azure](https://myapps.microsoft.com).

## <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>¿Cuánto tiempo se necesita para instalar el sitio en nuestro entorno de inquilino?

Debe tardar menos de 15 minutos. No se incluye el tiempo necesario para personalizar el sitio y adaptarlo a sus necesidades.

## <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>¿Microsoft 365 caminos de aprendizaje es una solución de código abierto y cuáles son las implicaciones?

Microsoft 365 de aprendizaje es una solución de software de código abierto (OSS) y, como tal, conlleva un conjunto de ventajas y consideraciones para el sistema operativo:

### <a name="benefits"></a>Ventajas 

- **Microsoft 365 de aprendizaje es una solución gratuita:** Los clientes pueden instalar la solución en su inquilino, personalizarla y ponerla a disposición de los usuarios finales.
- **El sistema operativo permite un desarrollo y colaboración rápidos:** Todas las soluciones de código abierto están disponibles para una amplia comunidad de colaboradores. Microsoft está comprometido con este método para impulsar la innovación. Para garantizar que ofrecemos una experiencia que beneficia al conjunto más amplio de nuestros clientes, nuestro equipo principal de administración de servicios se reservará el derecho de determinar qué contribuciones se combinan en nuestra compilación oficial.  
- **El sistema operativo habilita la colaboración con partners:** Microsoft está trabajando con varios partners de aprendizaje para apoyar sus esfuerzos en futuras extensiones y contribuciones a Microsoft 365 de aprendizaje. Proporcionaremos más información a medida que estos planes estén finalizados.

### <a name="implications"></a>Implicaciones

- **OSS no es un producto comercialmente disponible:** Los productos comerciales incluyen actualización y revisión y se incluyen en contratos de soporte técnico basados en tarifas. Aunque Actualmente Microsoft ofrece documentación, actualización y revisión para las rutas de aprendizaje Microsoft 365, se basa en nuestro compromiso de mejorar este escenario empresarial en particular. Aunque nuestros planes son seguir invirtiendo en caminos de aprendizaje, tenga en cuenta que nuestro equipo de administración de servicios puede cambiar estrategias en el futuro. Los cambios futuros en Microsoft 365 de aprendizaje se comunicarán antes de que entren en vigor.
- **Como sistema operativo, Microsoft 365** caminos de aprendizaje se admiten a través de una lista de problemas en línea en GitHub: Microsoft 365 caminos de aprendizaje no están cubiertos por ningún contrato de soporte técnico de Microsoft existente. Los problemas enviados se han Microsoft 365 los propietarios del servicio de caminos de aprendizaje y la comunidad. Los niveles de servicio de resolución de problemas NO están al mismo nivel que un contrato de soporte técnico de Microsoft de pago.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-sub-site-of-our-primary-sharepoint-site-collection"></a>¿Podemos convertir las rutas Microsoft 365 aprendizaje en un subs sitios de nuestra colección SharePoint de sitios?

No. El sitio se basa en una plantilla de sitio de comunicación, que siempre está pensada para ser una colección de sitios raíz.

> [!NOTE]
> Es importante tener en cuenta los permisos que los usuarios finales necesitarán para acceder al sitio. La mayoría de las organizaciones han definido grupos de usuarios o de seguridad. Debe agregar los grupos de seguridad adecuados al nuevo portal de formación una vez que esté listo para iniciarlo en su comunidad de empleados.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>Necesito reinstalar el sitio; ¿Qué debo hacer?

Siga las instrucciones de instalación [publicadas aquí](custom_provision.md).

> [!NOTE]
> Si ha deshabilitado la telemetría en la instalación anterior y desea continuar con la telemetría deshabilitada, deberá seguir las instrucciones para deshabilitar la telemetría [aquí](https://github.com/pnp/custom-learning-office-365/blob/a7168c97a76e0b4122e3ddfc530f6a10c724c3e1/installation/README.md).

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Hemos realizado actualizaciones de nuestra implementación de Microsoft 365 de aprendizaje. ¿Perderemos estas actualizaciones (realizadas en plantillas de sitio, listas de reproducción) si reinstalamos el sitio?

Las personalizaciones de páginas individuales y listas de reproducción personalizadas se perderán si reinstala el sitio en la instalación actual.  
