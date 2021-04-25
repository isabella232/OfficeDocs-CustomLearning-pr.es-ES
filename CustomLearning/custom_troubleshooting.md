---
author: pkrebs
ms.author: pkrebs
title: Solución de problemas de las formas de aprendizaje de Microsoft 365
ms.date: 02/10/2019
description: Obtenga información sobre cómo solucionar problemas de las rutas de aprendizaje de Microsoft 365
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 7190688d574042c8a1b8dfb67c8b246dfbf8c927
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000306"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a>Solucionar problemas de las rutas de aprendizaje de Microsoft 365

Estas son sugerencias para solucionar problemas que pueden producirse con las rutas de aprendizaje de Microsoft 365 o el servicio de aprovisionamiento de SharePoint Online.

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>Cómo saber si tiene permisos de administrador de inquilinos

Iniciar sesión en el servicio de aprovisionamiento de SharePoint Online y el aprovisionamiento de Aprendizaje personalizado requiere permisos de administrador de inquilinos. Si tiene problemas de inicio de sesión con el servicio de aprovisionamiento de SharePoint Online, asegúrese de que se le ha asignado el rol de administrador global. La solución de aprendizaje personalizado requiere permisos de administrador de inquilinos, también conocido como rol de administrador global de Office 365. Este es el modo de determinar si se le asignó el rol Administrador global.

1.  Inicie sesión en Office.com.
2.  Haga clic **en Administrador**
3.  En **Usuarios**, seleccione **Usuarios activos**
4.  Buscar su nombre
5.  Haga clic en su nombre en Resultados de búsqueda. Debería ver El administrador global de su rol.
![Página de ejemplo que enumera el rol junto con licencias, pertenencias a grupos y otra información.](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>Si no tiene el rol de administrador global
- Busque un administrador global en su organización y haga que esa persona inicie sesión en el servicio o que le asigne el rol de administrador global.

## <a name="tenant-app-catalog-troubleshooting"></a>Solución de problemas del Catálogo de aplicaciones de inquilino
El aprendizaje personalizado requiere que se aprovisione un Catálogo de aplicaciones en el inquilino de destino. La creación de un catálogo de aplicaciones requiere permisos de administrador global. Estos son los pasos para solucionar problemas comunes del Catálogo de aplicaciones:

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>Cómo saber si tienes un catálogo de aplicaciones de inquilino 
Para empezar, asegúrese de que tiene permisos de administrador global. Consulta los pasos para los permisos de administrador de inquilinos anteriores.

1. En Office 365, haga clic en **Administrador**, haga clic en la flecha expandir >, haga clic **en Mostrar todos** los centros de  >  **administración**  >  **de SharePoint**.
2. Haga **clic en Classic Admin SharePoint Center**  >  **apps** App  >  **Catalog**.
3. En **Aplicaciones,** debería ver un icono titulado **Distribuir aplicaciones para SharePoint**. Si ve el icono, tiene un Catálogo de aplicaciones de inquilinos. Vea la **sección Cómo asegurarse de que es una intercalación** de sitios... a continuación. Si no ves el icono, deberás crear un catálogo de aplicaciones de inquilino para tu inquilino. Consulta la **sección Cómo crear un catálogo de aplicaciones de** inquilino a continuación.

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>Cómo asegurarse de que es propietario de una colección de sitios en el Catálogo de aplicaciones de inquilinos 
Para aprovisionar las rutas de aprendizaje de Microsoft 365, deberás ser propietario de una colección de sitios en el Catálogo de aplicaciones de inquilinos. Este es el modo de determinar si es un propietario.

1. En Office 365, haga clic en **Administrador**, haga clic en la flecha expandir >, haga clic **en Mostrar todos** los centros de  >  **administración**  >  **de SharePoint**.
2. Haga **clic en Centro de Administración clásica de SharePoint** y, a continuación, seleccione el catálogo de **aplicaciones**.
3. Seleccione **Propietario** y, a continuación, asegúrese de que es un propietario de la colección de sitios. Debería tener un aspecto parecido a este.
![Página Administrar administradores.](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>Cómo crear un Catálogo de aplicaciones de inquilinos si no existe uno 
1. Inicie sesión en Office 365 con su cuenta de administrador de SharePoint Online.
2. Haga clic en **Administrador**.
3. En **Centros de administración,** haga clic **en SharePoint**. 
4. Haga clic **en Catálogo de**  >  **aplicaciones**.
5. Haga **clic en Crear un nuevo sitio de catálogo de** aplicaciones y, a continuación, haga clic en **Aceptar**. 
6.  Escribe la información del Catálogo de aplicaciones. Es posible que desee incluir más de un administrador. A continuación se muestra un ejemplo.  
![Formulario para escribir información para un nuevo catálogo de aplicaciones.](media/cg-appcatalogfinish.png)

7.  Eso es todo. Ya ha terminado. Pero antes de pasar al aprovisionamiento de Aprendizaje personalizado, debes esperar al menos 30 minutos para asegurarte de que la creación del Catálogo de aplicaciones se haya completado. 

> [!IMPORTANT]
> Espere al menos 30 minutos después de crear el Catálogo de aplicaciones de inquilino antes de aprovisionar Aprendizaje personalizado. Esto garantiza que el proceso de aprovisionamiento del Catálogo de aplicaciones esté completo en SharePoint. 