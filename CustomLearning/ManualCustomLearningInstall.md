# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>Instalación y configuración manual del aprendizaje personalizado para Office 365

El elemento Web de aprendizaje personalizado de Microsoft se compila con [SharePoint Framework](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/sharepoint-framework-overview) versión 1.7.1.

Para instalar y configurar manualmente el elemento Web y la colección de sitios, deberá completar los siguientes pasos:

1. Compruebe que ha cumplido todos los requisitos previos.
1. Instale el archivo customlearning. sppkg en el catálogo de aplicaciones del inquilino de Office 365.
1. Aprovisionar o identificar un sitio de comunicación moderno para que actúe como el sitio principal de aprendizaje personalizado para Office 365.
1. Ejecute un script de PowerShell que configurará el inquilino con los artefactos apropiados de los que depende el aprendizaje personalizado.
1. Navegue a la página del sitio CustomLearningAdmin. aspx para cargar el elemento Web de administración para inicializar la configuración de contenido personalizada.

## <a name="prerequisites"></a>Requisitos previos

Debe tener instalado y configurado el catálogo de aplicaciones de todo el inquilino. Consulte [configurar su inquilino de Office 365](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) y seguir la sección crear un sitio de catálogo de aplicaciones. Si ya se ha aprovisionado el catálogo de aplicaciones de todo el inquilino, necesitará tener acceso a una cuenta que tenga derechos para cargar un paquete para completar este proceso de configuración. Por lo general, se trata de una cuenta con el rol de administrador de SharePoint. Si una cuenta con ese rol no funciona, vaya al centro de administración de SharePoint y busque los administradores de la colección de sitios para la colección de sitios del catálogo de aplicaciones e inicie sesión como uno de los administradores de la colección de sitios, o bien agregue la cuenta de administrador de SharePoint. se produjeron errores en los administradores de la colección de sitios. También necesitará tener acceso a una cuenta que sea administrador de inquilinos de SharePoint.

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>Cargar el elemento Web en el catálogo de aplicaciones del espacio empresarial

Para configurar el aprendizaje personalizado para Office 365, debe cargar el archivo customlearning. sppkg en el catálogo de aplicaciones de todo el inquilino e implementarlo. Para obtener instrucciones detalladas sobre cómo agregar una aplicación al catálogo de aplicaciones, vea [usar el catálogo de aplicaciones para hacer que las aplicaciones empresariales personalizadas estén disponibles en su entorno de SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) .

## <a name="provisionidentify-modern-communication-site"></a>Aprovisionar/identificar sitio de comunicación moderno

Identifique un sitio de comunicación de SharePoint existente o bien aprovisione uno nuevo en el espacio empresarial de SharePoint Online. Para obtener más información sobre cómo aprovisionar un sitio de comunicación, vea [crear un sitio de comunicación en SharePoint Online](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) y siga los pasos para crear un sitio de comunicación.

## <a name="set-permissions-for-the-site"></a>Establecer permisos para el sitio

Querrá agregar a todos los usuarios que deberían poder ver contenido en el grupo visitantes y todos los usuarios que deben poder administrar las listas de reproducción personalizadas en el grupo miembros. Para configurar el sitio para aprendizaje personalizado la primera vez que el usuario debe ser administrador de la colección de sitios o parte del grupo de propietarios.

Agregar la aplicación aprendizaje personalizado para Office 365 a la colección de sitios.

## <a name="execute-powershell-configuration-script"></a>Ejecutar script de configuración de PowerShell

Se incluye un `CustomLearningConfiguration.ps1` script de PowerShell que tendrá que ejecutar para crear tres [propiedades de inquilino](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) que use la solución. Además, el script crea dos [páginas de aplicación de elemento único](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) en la biblioteca de páginas del sitio para hospedar los elementos Web de administrador y de usuario en una ubicación conocida.

### <a name="disabling-telemetry-collection"></a>DesHabilitar la colección de telemetría

Parte de esta solución incluye el seguimiento de telemetría de anonimizan, que de forma predeterminada se establece en activado. Si va a realizar una instalación manual y desea desactivar el seguimiento de telemetría, cambie el `CustomlearningConfiguration.ps1` script para establecer la variable $optInTelemetry en $false.

Si no está realizando una instalación manual y desea desactivar el seguimiento de telemetría, se ha incluido un script `TelemetryOptOut.ps1` independiente que, cuando se ejecuta, deshabilita el seguimiento de telemetría.

## <a name="initialize-web-part-custom-configuration"></a>Inicializar la configuración personalizada del elemento Web

Una vez ejecutado correctamente el script de PowerShell, navegue `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`a. Esto inicializa el elemento de lista CustomConfig que configura el aprendizaje personalizado para su primer uso.

La configuración se ha completado y puede avanzar con el uso de aprendizaje personalizado para Office 365. Para obtener más información, consulte la documentación del usuario.