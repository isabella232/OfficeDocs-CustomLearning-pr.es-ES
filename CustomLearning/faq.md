---
author: karuanag
ms.author: karuanag
title: Preguntas más frecuentes sobre los caminos de aprendizaje de Microsoft 365
ms.date: 02/10/2019
description: Información sobre las preguntas más frecuentes para los caminos de aprendizaje de Microsoft 365
ms.openlocfilehash: 26d6c7140b4d387e13b907033ea53b752f5e20ea
ms.sourcegitcommit: 0077704d7edcc26eda76900115716fc5b7b1c518
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/21/2019
ms.locfileid: "34334724"
---
# <a name="frequently-asked-questions"></a>Preguntas más frecuentes

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>¿Cuáles son los requisitos para instalar los caminos de aprendizaje de Microsoft 365 en mi entorno de inquilino?

- SharePoint Online y sitios de comunicación habilitados.
- La persona que se va a aprovisionar CLO365 debe ser el administrador de inquilinos del inquilino de destino para la instalación.
- El "Catálogo de aplicaciones" del espacio empresarial debe estar disponible en la opción "aplicaciones" del centro de administración de SharePoint.
- Si se crea un nuevo catálogo de aplicaciones, es necesario un tiempo de espera de 30 minutos o más para que el catálogo de aplicaciones se aprovisione por completo. Si se intenta aprovisionar los caminos de aprendizaje de Microsoft 365 directamente después de crear el catálogo de aplicaciones del inquilino, se producirá un error de aprovisionamiento de la solución de rutas de aprendizaje. 
- La persona que se va a aprovisionar CLO365 debe ser un administrador de la colección de sitios del catálogo de aplicaciones en el inquilino de destino para la instalación.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>¿Por qué Microsoft pide permisos de espacio empresarial al instalar los caminos de aprendizaje de Microsoft 365 

- El servicio de aprovisionamiento de SharePoint Online usa los permisos para aprovisionar el sitio de SharePoint de rutas de aprendizaje, crear las páginas del sitio e instalar la aplicación de caminos de aprendizaje de Microsoft 365 en su espacio empresarial. Ésta es la única razón por la que nos solicitamos los permisos. Sin los permisos solicitados, el servicio de aprovisionamiento de SharePoint no puede ejecutar los comandos que instalan automáticamente la plantilla de sitio de rutas de aprendizaje y el elemento Web. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>¿Cuáles son las implicaciones de las rutas de aprendizaje de Microsoft 365 en una versión preliminar beta? 

Las rutas de aprendizaje de Microsoft 365 se encuentran actualmente en versión preliminar. Tenga en cuenta lo siguiente cuando evalúe, planee e implemente los caminos de aprendizaje de Microsoft 365:

- Al igual que con cualquier solución beta, nuestro equipo de administración de servicios se reserva el derecho de realizar cambios en el servicio y sus componentes. A medida que estamos resolviendo activamente los errores y los problemas de experiencia del usuario, es probable que necesite actualizar el elemento Web.
- Para actualizar el elemento Web, deberá descargarlo de nuestro repositorio de GitHub y cargarlo en el catálogo de aplicaciones del espacio empresarial. Consulte la sección "actualización de la soluci?" del archivo [Léame](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) de rutas de aprendizaje de Microsoft 365. 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>¿En qué idiomas están disponibles los caminos de aprendizaje de Microsoft 365?

Las rutas de aprendizaje de Microsoft 365 actualmente solo están disponibles en inglés. El aprovisionamiento automático de un extremo a otro solo funciona con inquilinos en inglés. La implementación de la compatibilidad multilingüe para estos nueve idiomas se ha previsto en el CY19 Q3: 

- Chino (simplificado) 
- Neerlandés (Países Bajos) 
- Francés  
- Alemán 
- Italiano (Italia) 
- Japonés (Japón)  
- Portugués (Brasil) 
- Ruso (Ruso)  
- Español 

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>¿Cuánto tiempo se tarda en instalar el sitio en el entorno de inquilinos?

En función de las pruebas de la instalación, esta tardará menos de 15 minutos. Esto no incluye el tiempo necesario para personalizar el sitio según sus necesidades.

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>¿Microsoft 365 Learning ruta una solución de código abierto y cuáles son las implicaciones?

Las rutas de aprendizaje de Microsoft 365 son una solución de software de código abierto (OSS) y, como tales, tienen un conjunto de ventajas y consideraciones del alemán al SO:

#### <a name="benefits"></a>Ventajas 
- Los **caminos de aprendizaje de Microsoft 365 son una solución gratuita:** Los clientes pueden instalar la solución en su espacio empresarial, personalizarla y ponerla a disposición de los usuarios finales.
- Los **sistemas operativos permiten el desarrollo y la colaboración rápidos:**  Todas las soluciones de código abierto están disponibles para una amplia comunidad de colaboradores.  Microsoft se compromete a este método de impulsar la innovación.  Para asegurarse de que proporcionamos una experiencia que beneficia al más amplio conjunto de nuestros clientes, nuestro equipo de administración de servicios principal se reservará el derecho de determinar qué contribuciones se combinan en nuestra compilación oficial.  
- Los **sistemas operativos permiten la colaboración con los Partners:** Microsoft trabaja con varios socios de aprendizaje para apoyar sus esfuerzos en futuras extensiones y contribuciones a los caminos de aprendizaje de Microsoft 365. Proporcionaremos más información a medida que estos planes se terminen. 
    
#### <a name="implications"></a>Percusión
- Los **sistemas operativos no son un producto disponible comercialmente:** Los productos comerciales incluyen la actualización y la revisión, y se incluyen en los contratos de asistencia basada en honorarios. Mientras que Microsoft ofrece actualmente documentación, actualización y revisión para los caminos de aprendizaje de Microsoft 365, se basa en nuestro compromiso de mejorar este escenario empresarial en particular. Nuestros planes van a seguir invirtiendo en caminos de aprendizaje, pero los clientes deben tener en cuenta que el equipo de administración de servicios puede cambiar las estrategias en el futuro. Todos los cambios futuros en los caminos de aprendizaje de Microsoft 365 se comunicarán antes de que surtan efecto. 
- **Como sistemas operativos, los caminos de aprendizaje de microsoft 365 se admiten a través de una lista de problemas en línea en github**: los caminos de aprendizaje de Microsoft 365 no están cubiertos por ningún contrato de soporte técnico de Microsoft existente. Los problemas presentados están clasificados por los propietarios del servicio de los caminos de aprendizaje de Microsoft 365 y la comunidad. Los niveles de servicio de resolución de problemas no se encuentran en el mismo nivel que el de un contrato de soporte de Microsoft pagado.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>¿Podemos hacer que Microsoft 365 Learning enrutara un subsitio de nuestra colección de sitios de SharePoint principal?

No. El sitio se basa en una plantilla de sitio de comunicación, que siempre está pensada como una colección de sitios raíz.

> [!NOTE]
> Es importante tener en cuenta los permisos que deben tener los usuarios finales para obtener acceso al sitio. La mayoría de las organizaciones tienen definidos seguridad o grupos de usuarios. Debe agregar los grupos de seguridad adecuados a su nuevo portal de formación cuando esté listo para iniciarlo en su comunidad de empleados.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>Es necesario volver a instalar el sitio; ¿Qué debo hacer?

Siga las instrucciones de instalación publicadas [aquí](custom_provision.md).

> [!NOTE]
> Si ha deshabilitado la telemetría en su instalación anterior y desea continuar con la telemetría deshabilitada, tendrá que seguir las instrucciones para deshabilitar la telemetría aquí.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Hemos realizado actualizaciones a nuestra implementación de los caminos de aprendizaje de Microsoft 365. Se perderán estas actualizaciones (hechas a la plantilla de sitio, listas de reproducción) si se vuelve a instalar el sitio.

Las personalizaciones de páginas individuales y listas de reproducción personalizadas se perderán si vuelve a instalar el sitio a través de la instalación actual.  