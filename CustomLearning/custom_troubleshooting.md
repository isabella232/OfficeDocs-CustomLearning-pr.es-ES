---
author: pkrebs
ms.author: pkrebs
title: Solución de problemas de caminos de aprendizaje de Microsoft 365
ms.date: 02/10/2019
description: Aprenda a solucionar problemas relacionados con los caminos de aprendizaje de Microsoft 365
ms.openlocfilehash: de46b9c754dac36de230b36ec4a5542518a1dcd5
ms.sourcegitcommit: 1a111a49a0413a56a880e29109ba01b5e5f33d09
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/20/2019
ms.locfileid: "34247685"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a>Solución de problemas de caminos de aprendizaje de Microsoft 365

A continuación, se indican sugerencias de solución de problemas para los problemas que pueden producirse con las rutas de aprendizaje de Microsoft 365 o el servicio de aprovisionamiento de SharePoint Online.

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>Cómo saber si tiene permisos de administrador de inquilinos

Iniciar sesión en el servicio de aprovisionamiento de SharePoint Online y aprovisionar el aprendizaje personalizado requiere permisos de administrador de inquilinos. Si tiene problemas de inicio de sesión con el servicio de aprovisionamiento de SharePoint Online, asegúrese de que se le ha asignado el rol de administrador global. La solución de aprendizaje personalizada requiere permisos de administrador de inquilinos, que de lo contrario se conoce como rol de administrador global de Office 365. Siga estos pasos para determinar si se le ha asignado el rol de administrador global.

1.  Inicie sesión en Office.com.
2.  Haga clic en **Administración**
3.  En **usuarios**, seleccione **usuarios activos** .
4.  Buscar su nombre
5.  Haga clic en su nombre en los resultados de búsqueda. Debe ver el administrador global de su rol.

![CG-globaladminrole. png](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>Si no tiene la función de administrador global
- Busque un administrador global de la organización y pídale que inicie sesión en el servicio o pídale que le asigne el rol de administrador global.

## <a name="tenant-app-catalog-troubleshooting"></a>Solución de problemas del catálogo de aplicaciones del espacio empresarial
El aprendizaje personalizado requiere que se aprovisione un catálogo de aplicaciones en el inquilino de destino. La creación de un catálogo de aplicaciones requiere permisos de administrador global. A continuación, se describen los pasos para solucionar problemas de catálogo de aplicaciones comunes:

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>Cómo saber si tiene un catálogo de aplicaciones del espacio empresarial 
Para empezar, asegúrese de que tiene permisos de administrador global. Vea los pasos para los permisos de administrador de inquilinos más arriba.

1. En Office 365, haga clic en **Administrador**, haga clic en la flecha de expansión >, haga clic en **Mostrar todos los** > **centros** > de administración**SharePoint**.
2. Haga clic en**Catálogo de aplicaciones**de**aplicaciones** > de **Centro** > de administración clásica de SharePoint.
3. En **aplicaciones**, debería ver un icono titulado **distribuir aplicaciones para SharePoint**. Si ve el icono, tiene un catálogo de aplicaciones del espacio empresarial. Vea la sección **Cómo asegurarse de que es un sitio colllection...** a continuación. Si no ve el icono, tendrá que crear un catálogo de aplicaciones del espacio empresarial para el inquilino. Vea la sección **Cómo crear un catálogo de aplicaciones del espacio empresarial** a continuación.

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>Cómo garantizar que es el propietario de una colección de sitios en el catálogo de aplicaciones del espacio empresarial 
Para aprovisionar los caminos de aprendizaje de Microsoft 365, tendrá que ser un propietario de la colección de sitios en el catálogo de aplicaciones del espacio empresarial. Esta es la manera de determinar si es propietario.

1. En Office 365, haga clic en **Administrador**, haga clic en la flecha de expansión >, haga clic en **Mostrar todos los** > **centros** > de administración**SharePoint**.
2. Haga clic en **centro de administración clásico de SharePoint**y, a continuación, seleccione el **Catálogo de aplicaciones**.
3. Seleccione **propietario**y, a continuación, asegúrese de que es el propietario de la colección de sitios. Debe tener un aspecto similar a este.
 
![CG-sitecollectionowner. png](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>Procedimiento para crear un catálogo de aplicaciones del espacio empresarial si no existe ninguno 
1. Inicie sesión en Office 365 con su cuenta de administrador de SharePoint Online.
2. Haga clic en **Administrador**.
3. En **centros de administración**, haga clic en **SharePoint**. 
4. Haga clic en**Catálogo**de aplicaciones de **aplicaciones** > .
5. Haga clic en **crear un nuevo sitio de catálogo de aplicaciones**y, a continuación, haga clic en **Aceptar**. 
6.  Escriba la información para el catálogo de aplicaciones. Es posible que quiera incluir más de un administrador. A continuación, se muestra un ejemplo.  

![CG-appcatalogfinish. png](media/cg-appcatalogfinish.png)

7.  Eso es todo. Ya ha terminado. Pero antes de pasar a aprovisionar el aprendizaje personalizado, debe esperar al menos 30 minutos para asegurarse de que la creación del catálogo de aplicaciones se ha completado. 

> [!IMPORTANT]
> Espere al menos 30 minutos después de crear el catálogo de aplicaciones del espacio empresarial antes de aprovisionar aprendizaje personalizado. Esto garantiza que el proceso de aprovisionamiento del catálogo de aplicaciones se haya completado dentro de SharePoint. 