---
author: karuanag
ms.author: karuanag
title: Preguntas más frecuentes para aprendizaje personalizado para soluciones de Office 365
ms.date: 02/10/2019
description: Información de preguntas para aprendizaje personalizado para Office 365 más frecuentes
ms.openlocfilehash: d8b5104e8feeaa4e70296f61594233b27363481b
ms.sourcegitcommit: f93a6a691331515ba10f4d43b491928ec268f0ec
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/12/2019
ms.locfileid: "29952657"
---
# <a name="frequently-asked-questions"></a>Preguntas más frecuentes

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a>1. ¿Cuáles son los requisitos para instalar Learning personalizados para Office 365 en mi entorno inquilino?

- SharePoint Online y los sitios de comunicación habilitado.
- La persona que va a ser aprovisionamiento CLO365 debe ser el Administrador de inquilinos del inquilino de destino para la instalación.
- Un 'catálogo de aplicaciones de ' inquilino debe estar disponible dentro de la opción 'Aplicaciones' del centro de administración de SharePoint.
- La persona que va a ser aprovisionamiento CLO365 debe ser un administrador de colección de sitios del catálogo de aplicaciones en el inquilino de destino para la instalación.

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a>2. ¿qué idiomas está disponible en la aprendizaje personalizado para Office 365?

Personalizado de aprendizaje para Office 365 está actualmente disponible solo en inglés. El aprovisionamiento automático end-to-end sólo funciona con los inquilinos en inglés. Pueden agregar idiomas adicionales en futuras versiones.

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>3. ¿cuánto tiempo se tarda en instalar el sitio en nuestro entorno de inquilino?

En función de las pruebas de la instalación, debe tardar menos de 15 minutos. Esto no incluye el tiempo necesario para personalizar el sitio según sus requisitos.

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a>¿4. podemos realizar personalizados un subsitio de nuestra colección de sitios de SharePoint principal de aprendizaje de Office 365?

No. El sitio se basa en una plantilla de sitio de comunicación, que siempre está pensada para ser una colección de sitios raíz.

> [!NOTE]
> Es importante tener en cuenta los permisos de que los usuarios finales se necesitan obtener acceso al sitio. La mayoría de las organizaciones han definido grupos de seguridad o usuario. Debe agregar los grupos de seguridad adecuados a su portal de aprendizaje de nuevo una vez que esté listo para iniciar a su comunidad de empleado.

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a>5. necesario volver a instalar el sitio; ¿Qué debo hacer?

Siga la instalación instrucciones publicado [aquí](installsitepackage.md).

> [!NOTE]
> Si hubiera deshabilitado telemetría en su instalación previa y desea continuar con la telemetría deshabilitado, debe seguir las instrucciones para deshabilitar la telemetría aquí.

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>6. se realizaron actualizaciones a la implementación de aprendizaje personalizado para Office 365. ¿Se perderán estas actualizaciones (realizadas en la plantilla de sitio, listas de reproducción) si se vuelve a instalar el sitio?

Si reinstala el sitio a través de la instalación actual, se perderán las personalizaciones realizadas en páginas individuales y listas de reproducción personalizadas.  