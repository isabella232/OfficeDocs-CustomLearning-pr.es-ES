---
author: karuanag
ms.author: karuanag
title: Preguntas más frecuentes sobre las soluciones de aprendizaje personalizado para Office 365
ms.date: 02/10/2019
description: Información sobre las preguntas más frecuentes sobre aprendizaje personalizado para Office 365
ms.openlocfilehash: 7da1f3da197fc298c83eac89e3455312cba7a851
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "32056016"
---
# <a name="frequently-asked-questions"></a>Preguntas más frecuentes

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a>1. ¿Cuáles son los requisitos para instalar aprendizaje personalizado para Office 365 en mi entorno de inquilino?

- SharePoint Online y sitios de comunicación habilitados.
- La persona que se va a aprovisionar CLO365 debe ser el administrador de inquilinos del inquilino de destino para la instalación.
- El "Catálogo de aplicaciones" del espacio empresarial debe estar disponible en la opción "aplicaciones" del centro de administración de SharePoint.
- La persona que se va a aprovisionar CLO365 debe ser un administrador de la colección de sitios del catálogo de aplicaciones en el inquilino de destino para la instalación.

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a>2. ¿Qué idiomas está disponible en aprendizaje personalizado para Office 365 en?

Aprendizaje personalizado para Office 365 actualmente está disponible solo en inglés. El aprovisionamiento automático de un extremo a otro solo funciona con inquilinos en inglés. Es posible que se agreguen otros idiomas en las versiones futuras.

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>3. ¿Cuánto tiempo se tarda en instalar el sitio en nuestro entorno de inquilino?

En función de las pruebas de la instalación, esta tardará menos de 15 minutos. Esto no incluye el tiempo necesario para personalizar el sitio según sus necesidades.

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a>4. ¿podemos hacer que el aprendizaje personalizado para Office 365 sea un subsitio de nuestra colección de sitios de SharePoint principal?

No. El sitio se basa en una plantilla de sitio de comunicación, que siempre está pensada como una colección de sitios raíz.

> [!NOTE]
> Es importante tener en cuenta los permisos que deben tener los usuarios finales para obtener acceso al sitio. La mayoría de las organizaciones tienen definidos seguridad o grupos de usuarios. Debe agregar los grupos de seguridad adecuados a su nuevo portal de formación cuando esté listo para iniciarlo en su comunidad de empleados.

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a>5. es necesario volver a instalar el sitio; ¿Qué debo hacer?

Siga las instrucciones de instalación publicadas [aquí](custom_provision.md).

> [!NOTE]
> Si ha deshabilitado la telemetría en su instalación anterior y desea continuar con la telemetría deshabilitada, tendrá que seguir las instrucciones para deshabilitar la telemetría aquí.

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>6. hemos realizado actualizaciones a nuestra implementación de aprendizaje personalizado para Office 365. Se perderán estas actualizaciones (hechas a la plantilla de sitio, listas de reproducción) si se vuelve a instalar el sitio.

Las personalizaciones de páginas individuales y listas de reproducción personalizadas se perderán si vuelve a instalar el sitio a través de la instalación actual.  