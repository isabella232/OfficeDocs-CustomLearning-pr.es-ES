---
author: pkrebs
ms.author: pkrebs
title: Actualización de aprendizaje personalizada
ms.date: 02/10/2019
description: Aprendizaje personalizado de la configuración manual del elemento Web de Office 365
ms.openlocfilehash: f9729c922b374cc6b775737fa7c7c76a4719534c
ms.sourcegitcommit: b6617bbbaee0784d6216e96052c2469f97cf51e9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2019
ms.locfileid: "30411900"
---
# <a name="manual-upgrade-for-custom-learning"></a>Actualización manual de aprendizaje personalizado

Aprendizaje personalizado para Office 365 proporciona un proceso de actualización manual para organizaciones que participaron en pilotos anteriores. Con el proceso de actualización, las organizaciones pueden seguir usando su sitio de aprendizaje personalizado actual y actualizarlo agregando el nuevo y mejorado elemento Web de aprendizaje personalizado a su catálogo de aplicaciones de SharePoint y, a continuación, ejecutando un script de PowerShell. A continuación, se proporciona información general sobre el proceso de actualización: 

- Validar que la persona responsable de cargar el nuevo elemento Web y que ejecuta el script de PowerShell tiene los permisos necesarios
- Cargar el elemento Web, el archivo customlearning. sppkg, en el catálogo de aplicaciones del espacio empresarial de Office 365
- Ejecutar un script de PowerShell que configurará el inquilino con los artefactos adecuados necesarios para el aprendizaje personalizado
- Navegue a la página CustomLearningAdmin. aspx en el sitio de aprendizaje personalizado para inicializar la configuración de CContent personalizada.

## <a name="prerequisites"></a>Requisitos previos
Para garantizar una actualización correcta del aprendizaje personalizado, se deben cumplir los siguientes requisitos previos. 

- Debe tener configurado un catálogo de aplicaciones para todos los inquilinos. Si no tiene un catálogo de aplicaciones del espacio empresarial, consulte [configurar el inquilino de Office 365](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) y siga la sección crear un sitio del catálogo de aplicaciones. 
- Si ya se ha aprovisionado el catálogo de aplicaciones de todo el espacio empresarial, necesita tener acceso a una cuenta que tenga derechos para cargar un paquete en él. Por lo general, se trata de una cuenta con el rol de administrador de SharePoint. 
- Si una cuenta con el rol de administrador de SharePoint no funciona: vaya al centro de administración de SharePoint, seleccione el catálogo de aplicaciones, haga clic en propietarios e inicie sesión como uno de los administradores de la colección de sitios o agregue la cuenta de administrador de SharePoint que produjo el error en el sitio. Lista de administradores de la colección. 

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>Paso 1: obtener el paquete de elementos Web y la secuencia de comandos de instalación de GitHub
Como parte del proceso de instalación, necesitará el paquete de elementos Web de aprendizaje personalizado y el script de configuración de PowerShell.

1. Vaya al [repositorio de github de aprendizaje personalizado](https://github.com/pnp/custom-learning-office-365).
2. Haga clic en **clonar o descargar**y, a continuación, **Descargue zip**.   
3. Guarde el archivo **zip** en una ubicación de la unidad local.
4. Extraiga el archivo **zip** en la unidad local.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Paso 2: cargar el elemento Web en el catálogo de aplicaciones del espacio empresarial
Para configurar el aprendizaje personalizado para Office 365, debe cargar el archivo customlearning. sppkg en el catálogo de aplicaciones de todo el inquilino e implementarlo. Para obtener instrucciones detalladas sobre cómo agregar una aplicación al catálogo de aplicaciones, vea [usar el catálogo de aplicaciones para hacer que las aplicaciones empresariales personalizadas estén disponibles en su entorno de SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) .

1. En Office 365, haga clic en **Administrador**.
2. En **centros de administración**, haga clic en **SharePoint**.
3. Haga clic en **aplicaciones** > **Catálogo** > **de aplicaciones distribute apps for SharePoint.**
4. Haga clic en **cargar** > **archivos de selección**.
5. En la carpeta en la que guardó el archivo ZIP, seleccione **** la carpeta WebPart y, a continuación, seleccione **customlearning. sppkg.**
6. Haga clic en **Implementar**.

## <a name="step-5--execute-powershell-configuration-script"></a>Paso 5: ejecutar el script de configuración de PowerShell
Un script `CustomLearningConfiguration.ps1` de PowerShell se incluye en la descarga de zip desde github. Debe ejecutar el script para crear tres propiedades de [inquilino](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) que usa la solución. Además, el script crea dos [páginas de aplicación de elemento único](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) en la biblioteca de páginas del sitio para hospedar los elementos Web de administrador y de usuario en una ubicación conocida. Estas son las páginas de la aplicación:

- CustomAdministration. aspx
- CustomViewer. aspx

### <a name="to-run-the-powershell-script"></a>Para ejecutar el script de PowerShell
- Con PowerShell, ejecute el `CustomLearningConfiguration.ps1` script que se encuentra en la carpeta WebPart desde el archivo zip de github. Si se ejecuta correctamente, verá tres pares clave-valor y **Administrador de aprendizaje personalizado para desactivado...** en la ventana de comandos.

### <a name="disabling-telemetry-collection"></a>DesHabilitar la colección de telemetría
Aprendizaje personalizado incluye el seguimiento de telemetría de anonimizan, que de forma predeterminada se establece en activado. Si desea desactivar el seguimiento de telemetría, cambie el `CustomlearningConfiguration.ps1` script para establecer la `$optInTelemetry` variable en. `$false`

## <a name="step-6---initialize-web-part-custom-configuration"></a>Paso 6: inicializar la configuración personalizada del elemento Web
Una vez ejecutado correctamente el script de PowerShell, navegue `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`a. Al abrir **CustomLearningAdmin. aspx** se inicializa el elemento de lista **CustomConfig** que configura el aprendizaje personalizado para el primer uso. Debería ver una página similar a la siguiente:

![CG-adminapppage. png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Agregar propietarios al sitio
Como administrador de inquilinos, es poco probable que sea la persona que va a personalizar el sitio, por lo que necesitará asignar algunos propietarios al sitio. Los propietarios tienen privilegios administrativos en el sitio para que puedan modificar las páginas del sitio y remarcar el sitio. También tienen la posibilidad de ocultar y mostrar contenido entregado a través del elemento Web de aprendizaje personalizado. También tendrán la capacidad de crear una lista de reproducción personalizada y asignarlas a subcategorías personalizadas.  

1. En el menú **configuración** de SharePoint, haga clic en **permisos del sitio**.
2. Haga clic en **Configuración avanzada de permisos**.
3. Haga clic en **aprendizaje personalizado para los propietarios de Office 365**.
4. Haga clic en **nuevo** > **Agregar usuarios a este grupo**, agregue a los usuarios que desea que sean propietarios y, a continuación, haga clic en **compartir**.

La actualización ha finalizado. Para obtener más información sobre cómo adaptar el sitio de aprendizaje y el elemento web personalizados para su entorno, vea [customize the Training Experience](custom_overview.md).

## <a name="upgrade-instructions-for-site-owners"></a>Instrucciones de actualización para los propietarios del sitio
Aprendizaje personalizado para Office 365 ha incorporado una amplia variedad de mejoras en el elemento Web. El trabajo con el elemento Web se describe con detalle en la sección [personalizar la experiencia de aprendizaje](custom_overview.md) . Por ahora, el propietario del sitio debe:  

- Compruebe que el elemento Web de aprendizaje personalizado para Office 365 está disponible. 
- Reemplazar el elemento Web existente en páginas con el nuevo elemento Web
- Reemplazar los vínculos que apuntan al elemento web antiguo

### <a name="verify-the-custom-learning-for-office-365-web-part-is-available"></a>Comprobar que el elemento Web de aprendizaje personalizado para Office 365 está disponible
1.  En el sitio de aprendizaje personalizado, haga clic en **configuración**y, a continuación, haga clic en ***Agregar una página**.
2.  Haga clic **+** en el icono de la página para agregar un elemento Web y, a continuación, seleccione el elemento Web **de aprendizaje personalizado para Office 365** . La página debería tener ahora un aspecto similar al del siguiente gráfico:

[CG-adminapppage. png](media/cg-adminapppage.png)
 
### <a name="replace-the-old-web-part-with-the-new-web-part"></a>Reemplazar el elemento web antiguo con el nuevo elemento Web
Antes de reemplazar el elemento Web de aprendizaje personalizado o realizar cambios en el sitio, le recomendamos que lea la documentación [personalizar la experiencia de aprendizaje](custom_overview.md) , ya que explica cómo usar el nuevo elemento Web. 

Para actualizar el sitio de aprendizaje personalizado, reemplace las instancias existentes del elemento Web con el nuevo elemento Web. Aunque no podemos estar seguro de dónde se ha agregado el elemento Web, la guía para pilotos anteriores era agregar el elemento Web a las siguientes páginas, por lo que busque reemplazar el elemento Web en estas páginas:

- Get-started-with-Office-365. aspx
- Get-started-with-Microsoft-Teams. aspx
- Get-started-with-OneDrive. aspx
- Get-started-with-SharePoint. aspx

### <a name="replace-existing-links-to-the-web-part"></a>Reemplazar los vínculos existentes al elemento Web
Con las mejoras del nuevo elemento Web, se ha cambiado la forma en que se vincula a una lista de reproducción. Como parte de la actualización, debe reemplazar los vínculos al elemento Web, incluidos los elementos de menú, y los vínculos de la Página principal. Antes de reemplazar el elemento Web de aprendizaje personalizado o realizar cambios en el sitio, le recomendamos que lea la documentación [personalizar la experiencia de aprendizaje](custom_overview.md) , ya que explica cómo usar el nuevo elemento Web. 

## <a name="recreate-existing-playlists"></a>Volver a crear listas de reproducción existentes 
Para asegurarse de que las listas de reproducción funcionan correctamente, se deben volver a crear todas las listas de reproducción que se hayan creado con la versión anterior del elemento Web. Antes de eliminar las listas de reproducción, cree una lista de las listas de reproducción personalizadas y los activos asociados para poder volver a crearlas fácilmente con el nuevo elemento Web de aprendizaje personalizado. Haga una copia de una lista de reproducción y, a continuación, elimínela. Puede usar el campo JSONData para realizar una copia del contenido de una lista de reproducción antes de eliminarlo. Esto hará que sea más fácil crear más adelante.


• En el sitio de aprendizaje personalizado, haga clic en configuración > contenido del sitio. • Seleccione una lista de reproducción, seleccione los puntos suspensivos, seleccione Editar y, a continuación, copie el contenido del campo JSONData y guárdelo en el Bloc de notas o en un documento independiente para consultarlo más adelante. Seleccione Cancelar.
• Seleccione la lista de reproducción, seleccione los puntos suspensivos y, después, seleccione eliminar.
• Ya está listo para volver a crear la lista de reproducción con el nuevo elemento Web.
Para obtener instrucciones sobre cómo usar el nuevo elemento Web de aprendizaje personalizado de Office https://docs.microsoft.com/en-us/office365/customlearning/custom_overview365, consulte.

## <a name="step-8---chan"></a>Paso 8: Chan

### <a name="next-steps"></a>Pasos siguientes
- [Personalice](custom_overview.md) la experiencia de aprendizaje para su organización.

