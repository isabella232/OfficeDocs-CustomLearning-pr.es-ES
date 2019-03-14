---
author: pkrebs
ms.author: pkrebs
title: Configuración independiente del elemento Web
ms.date: 02/10/2019
description: Aprendizaje personalizado de la configuración manual del elemento Web de Office 365
ms.openlocfilehash: 8bf6292518c36eda74a49f9968c8e0559fcf8320
ms.sourcegitcommit: 5ea8d7fdc255ef7de06f41b3c794bc40551cf5bb
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/14/2019
ms.locfileid: "30577856"
---
# <a name="stand-alone-web-part-setup"></a>Configuración independiente del elemento Web

Aprendizaje personalizado ofrece una configuración de elementos Web manual e independiente para aquellas organizaciones que ya tienen establecido un sitio de comunicación moderna de SharePoint online dedicado a la formación, o que solo quieren configurar el elemento Web de aprendizaje personalizado en su propio sitio de comunicación. Tenga en cuenta que la configuración manual requiere experiencia en el uso de Windows PowerShell y el shell de administración de SharePoint Online. Los pasos para una configuración manual del elemento Web de aprendizaje personalizado como se indica a continuación:

- Compruebe que ha cumplido todos los requisitos previos.
- Instale el archivo customlearning. sppkg en el catálogo de aplicaciones del inquilino de Office 365.
- Aprovisionar o identificar un sitio de comunicación moderno para que actúe como el sitio principal de aprendizaje personalizado para Office 365.
- Ejecute un script de PowerShell que configurará el inquilino con los artefactos apropiados de los que depende el aprendizaje personalizado.
- Navegue a la página del sitio CustomLearningAdmin. aspx para cargar el elemento Web de administración para inicializar la configuración de contenido personalizada.

> [!NOTE]
> Si está buscando una forma rápida y sencilla de configurar el aprendizaje personalizado, vea proVision [Custom Learning](custom_provision.md).

## <a name="prerequisites"></a>Requisitos previos
Para garantizar una configuración manual correcta del elemento Web de aprendizaje personalizado, se deben cumplir los siguientes requisitos previos. 

- Debe tener instalado y configurado el catálogo de aplicaciones de todo el inquilino. Consulte [configurar su inquilino de Office 365](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) y seguir la sección crear un sitio de catálogo de aplicaciones. 
- Si ya se ha aprovisionado el catálogo de aplicaciones de todo el inquilino, necesitará tener acceso a una cuenta que tenga derechos para cargar un paquete para completar este proceso de configuración. Por lo general, se trata de una cuenta con el rol de administrador de SharePoint. 
- Si una cuenta con ese rol no funciona, vaya al centro de administración de SharePoint y busque los administradores de la colección de sitios para la colección de sitios del catálogo de aplicaciones e inicie sesión como uno de los administradores de la colección de sitios, o bien agregue la cuenta de administrador de SharePoint. se produjeron errores en los administradores de la colección de sitios. 
- También necesitará tener acceso a una cuenta que sea administrador de inquilinos de SharePoint.

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>Paso 1: obtener el paquete de elementos Web y la secuencia de comandos de instalación de GitHub
Como parte del proceso de instalación, necesitará el paquete de elementos Web de aprendizaje personalizado y el script de configuración de PowerShell.

- Vaya al [repositorio de github de aprendizaje personalizado](https://github.com/pnp/custom-learning-office-365).
- Haga clic en **Descargar** para guardar el paquete de elementos Web y el script en una unidad local. Utilizará el script y el paquete de elementos Web en pasos posteriores de este proceso.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Paso 2: cargar el elemento Web en el catálogo de aplicaciones del espacio empresarial
Para configurar el aprendizaje personalizado para Office 365, debe cargar el archivo customlearning. sppkg en el catálogo de aplicaciones de todo el inquilino e implementarlo. Para obtener instrucciones detalladas sobre cómo agregar una aplicación al catálogo de aplicaciones, vea [usar el catálogo de aplicaciones para hacer que las aplicaciones empresariales personalizadas estén disponibles en su entorno de SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) .

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>Paso 3: aprovisionar o identificar un sitio de comunicación moderno
Identifique un sitio de comunicación de SharePoint existente o bien aprovisione uno nuevo en el espacio empresarial de SharePoint Online. Para obtener más información sobre cómo aprovisionar un sitio de comunicación, vea [crear un sitio de comunicación en SharePoint Online](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) y siga los pasos para crear un sitio de comunicación.

## <a name="step-4---add-the-custom-learning-for-office-365-app-to-the-site"></a>Paso 4: agregar la aplicación aprendizaje personalizado para Office 365 al sitio

1. En el sitio de SharePoint, haga clic en el menú sistema y, a continuación, haga clic en **Agregar una aplicación**. 
2. En **sus aplicaciones**, haga clic en **desde su organización**y, a continuación, haga clic en **aprendizaje personalizado para Office 365**. 

## <a name="step-5---set-permissions-for-the-site"></a>Paso 5: establecer permisos para el sitio
Asegúrese de que se han establecido los siguientes permisos para el sitio:
- **Administrador de la colección de sitios o parte del grupo propietarios** -permisos necesarios para inicializar el elemento de lista CustomConfig que configura el aprendizaje personalizado para su primer uso. 
- **Grupo miembros** : permissons necesario para administrar el aprendizaje personalizado, incluidos ocultar y mostrar contenido y administrar listas de reproducción personalizadas
- **Grupo visitantes** : permisos necesarios para ver el contenido del sitio. 

## <a name="step-6--execute-powershell-configuration-script"></a>Paso 6: ejecutar el script de configuración de PowerShell
Se incluye un `CustomLearningConfiguration.ps1` script de PowerShell que tendrá que ejecutar para crear tres [propiedades de inquilino](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) que use la solución. Además, el script crea dos [páginas de aplicación de elemento único](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) en la biblioteca de páginas del sitio para hospedar los elementos Web de administrador y de usuario en una ubicación conocida.

1. Si aún no ha descargado el shell de administración de SharePoint Online, Descárguelo ahora. Vea [Descargar Shell de administración de SharePoint Online](https://go.microsoft.com/fwlink/p/?LinkId=255251).
2. Es posible que deba establecer una directiva de ejecución de PowerShell para ejecutar el script. Para obtener más información, consulte [acerca de las directivas de ejecución](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).
3. Ejecute el `CustomLearningConfiguration.ps1` script. Además de las credenciales de administrador de espacios empresariales, el script le pedirá el nombre del espacio empresarial y el nombre del sitio. Teniendo en cuenta el siguiente ejemplo para la dirección `https://contoso.sharepoint.com/sites/O365CL`URL `contoso` del sitio,, es `O365CL` el nombre del espacio empresarial y es el nombre del sitio. 

### <a name="disabling-telemetry-collection"></a>DesHabilitar la colección de telemetría
Parte de esta solución incluye el seguimiento de telemetría de anonimizan, que de forma predeterminada se establece en activado. Si va a realizar una instalación manual y desea desactivar el seguimiento de telemetría, cambie el `CustomlearningConfiguration.ps1` script para establecer la variable $optInTelemetry en $false y ejecute el script.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Validar el aprovisionamiento correcto e inicializar la lista de CustomConfig

Una vez ejecutado correctamente el script de PowerShell, navegue hasta el sitio, inicialice el elemento de lista **CustomConfig** que configura el aprendizaje personalizado para el primer uso y valide que el sitio esté funcionando.

- Vaya a `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. Al abrir **CustomLearningAdmin. aspx** se inicializa el elemento de lista **CustomConfig** que configura el aprendizaje personalizado para el primer uso. Debería ver una página similar a la siguiente:

![CG-adminapppage. png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Agregar propietarios al sitio
Como administrador de inquilinos, es poco probable que sea la persona que va a personalizar el sitio, por lo que necesitará asignar algunos propietarios al sitio. Los propietarios tienen privilegios administrativos en el sitio para que puedan modificar las páginas del sitio y remarcar el sitio. También tienen la posibilidad de ocultar y mostrar contenido entregado a través del elemento Web de aprendizaje personalizado. Además, tendrán la capacidad de crear listas de reproducción personalizadas y asignarlas a subcategorías personalizadas.  

1. En el menú **configuración** de SharePoint, haga clic en **permisos del sitio**.
2. Haga clic en **Configuración avanzada de permisos**.
3. Haga clic en **aprendizaje personalizado para los propietarios de Office 365**.
4. Haga clic en **nuevo** > **Agregar usuarios a este grupo**y, a continuación, agregue las personas que desea que sean propietarios. 
5. Agregue un vínculo para [explorar el sitio](https://docs.microsoft.com/en-us/Office365/CustomLearning/custom_explore) en el mensaje de uso compartido y, a continuación, haga clic en **compartir**.

### <a name="next-steps"></a>Pasos siguientes
- [Personalice](custom_overview.md) la experiencia de aprendizaje para su organización.

