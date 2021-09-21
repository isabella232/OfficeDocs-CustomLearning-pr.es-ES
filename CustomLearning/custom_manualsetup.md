---
author: pkrebs
ms.author: pkrebs
title: Learning manual de rutas de acceso
ms.date: 07/06/2020
description: Microsoft 365 manual de rutas de aprendizaje
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: 7c6fc47336d354304164cebd95768a4bf97ee60f
ms.sourcegitcommit: 6005c2551bdea334767e6a056fdcb79533f2c858
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/21/2021
ms.locfileid: "59460968"
---
# <a name="learning-pathways-manual-setup"></a>Learning manual de rutas de acceso

Microsoft 365 de aprendizaje ofrece una configuración manual para organizaciones que necesitan soporte técnico para uno de los siguientes escenarios: 

- Su organización tiene un sitio de comunicación SharePoint en línea dedicado a la formación y desea agregar rutas de aprendizaje a ese sitio. En este escenario, el elemento web caminos de aprendizaje no se ha configurado en el sitio.

- Desea instalar rutas de aprendizaje para el soporte multilingüe en uno de los sitios de comunicación SharePoint de la organización. El sitio tiene o tendrá un idioma predeterminado que no es inglés y es uno de los idiomas admitidos por las rutas de aprendizaje. Estos son los idiomas admitidos por las rutas de aprendizaje:

- Inglés
- Chino (simplificado)
- Francés
- Alemán
- Italiano (Italia)
- Japonés (Japón)
- Portugués (Brasil)
- Ruso (ruso)
- Spanish

La configuración manual de las rutas de aprendizaje requiere experiencia trabajando con Windows PowerShell y el Shell SharePoint administración en línea. Este es un resumen de los pasos para la configuración manual de las rutas de aprendizaje: 

- Valide que ha cumplido todos los requisitos previos.
- Comprueba la configuración de idioma predeterminada para el sitio. Si está bien, continúe con la instalación manual. Si necesita una configuración de idioma predeterminada diferente, deberá crear un nuevo sitio. 
- Instale el archivo customlearning.sppkg en el catálogo de aplicaciones SharePoint inquilino.
- Aprovisionar e identificar un sitio de comunicación moderno para que actúe como su sitio principal Microsoft 365 caminos de aprendizaje.
- Ejecute un script de PowerShell que configurará el espacio empresarial con los artefactos de los que dependen las rutas de aprendizaje.
- Vaya a la página de sitio CustomLearningAdmin.aspx para cargar el elemento web de administración para inicializar la configuración de contenido personalizado.

## <a name="prerequisites"></a>Requisitos previos
Para garantizar una correcta configuración manual del elemento web caminos de aprendizaje, deben cumplirse los siguientes requisitos previos. 

- Debe haber configurado y configurado el Catálogo de aplicaciones para todo el espacio empresarial. Consulta [Configurar el espacio empresarial Office 365 y](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) sigue la sección del sitio "Crear catálogo de aplicaciones". 
- Si el Catálogo de aplicaciones de todo el espacio empresarial ya se ha aprovisionado, necesitarás acceso a una cuenta que tenga derechos para cargar un paquete en él. Por lo general, esta cuenta tiene un SharePoint de administrador. 
- Si una cuenta con ese rol no funciona, vaya al Centro de administración de SharePoint y busque los administradores de colecciones de sitios para la colección de sitios del Catálogo de aplicaciones e inicie sesión como uno de los administradores de la colección de sitios o agregue la cuenta de administrador de SharePoint que no pudo a los administradores de la colección de sitios. 
- También necesitarás acceso a una cuenta que sea un administrador SharePoint inquilino.

## <a name="step-1---check-your-language-settings"></a>Paso 1: comprobar la configuración de idioma
Como primer paso del proceso de instalación manual, compruebe la configuración del idioma del sitio. Estas son las opciones posibles:

### <a name="option-1---you-dont-want-multilingual-support"></a>Opción 1: no desea compatibilidad multilingüe
Si no desea compatibilidad multilingüe para su sitio, asegúrese de que está desactivado.
1.  En el SharePoint de comunicación, **seleccione Configuración** Información del sitio Ver toda la configuración  >    >  **del** sitio Configuración de  >  **idioma**. 
2.  Establezca el modificador Habilitar páginas y noticias para que se **traduzcan** a varios idiomas en **Desactivado**.
3.  Haga clic en **Guardar**. 
4.  Continúe con el paso 2.

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>Opción 2: desea compatibilidad multilingüe y está bien con el idioma predeterminado
Un SharePoint de comunicación tiene un idioma predeterminado. El idioma predeterminado determina el idioma en el que se ven las rutas de aprendizaje, incluida la página Administración de caminos de aprendizaje. La configuración de idioma predeterminada se establece cuando se crea el sitio por primera vez y no se puede cambiar después. Antes de continuar con la configuración manual, asegúrese de que está bien con el idioma predeterminado del sitio de destino.

1.  En el SharePoint de comunicación, **seleccione Configuración** Información del sitio Ver toda la configuración  >    >  **del** sitio Configuración de  >  **idioma**. 
2.  Establezca el modificador Habilitar páginas y noticias para que se **traduzcan** a varios idiomas en **On**.
    - Si está de acuerdo con el idioma que aparece en la parte superior de la lista en **Idioma**, puede agregar idiomas adicionales y, a continuación, haga clic en **Guardar**. Continúe con el paso 2.
    - Si desea un idioma predeterminado diferente al que se ha seleccionado para el sitio, deberá crear un nuevo sitio de comunicación de SharePoint con el idioma que desee. Continúe con la opción 3. 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>Opción #3: desea compatibilidad multilingüe, pero desea un idioma predeterminado diferente para el sitio
Con esta opción, se crea un nuevo sitio de SharePoint de comunicación en línea con el idioma predeterminado que desee y, a continuación, se establece la configuración de idioma del sitio. 
1.  Para crear un nuevo SharePoint de comunicación, vea [Create a communication site in SharePoint Online](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb). Al crear el sitio, asegúrese de establecer el idioma en el idioma predeterminado que desea para las rutas de aprendizaje. 
2. En el sitio que ha creado, seleccione **Configuración**  >  **Información del sitio** Ver toda la configuración  >  **del** sitio Configuración  >  **de idioma**. 
2.  Establezca el modificador Habilitar páginas y noticias para que se **traduzcan** a varios idiomas en **On**.
3. Agregue idiomas adicionales, si es necesario, y, a continuación, haga clic **en Guardar**. 
4. Continúe con el paso 2. 

>! [Nota] Si necesita migrar contenido personalizado de un sitio a un sitio recién creado, consulte la sección "Migrar contenido personalizado" más adelante en este documento. 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>Paso 2: obtener el paquete de elementos web y el script de instalación desde GitHub
Como parte del proceso de instalación, necesitará el paquete de elementos web Microsoft 365 caminos de aprendizaje y el script de instalación de PowerShell.

- Vaya a [las rutas de aprendizaje GitHub Repository](https://github.com/pnp/custom-learning-office-365).
- Haga **clic en** Descargar para guardar el paquete y el script del elemento web en una unidad local. El script y el paquete de elementos web se usarán en los pasos posteriores de este proceso.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Paso 2: Upload el elemento web al Catálogo de aplicaciones de inquilino
Para configurar las Microsoft 365 aprendizaje, cargue el archivo customlearning.sppkg en el Catálogo de aplicaciones de todo el espacio empresarial e impleméntelo. Consulta [Usar el Catálogo de](/sharepoint/use-app-catalog) aplicaciones para que las aplicaciones empresariales personalizadas estén disponibles para tu entorno de SharePoint Online para obtener instrucciones detalladas sobre cómo agregar una aplicación al Catálogo de aplicaciones.

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>Paso 3: Aprovisionar e identificar un sitio de comunicación moderno
Identifique un sitio de SharePoint de comunicación existente o aprovisione uno nuevo en su SharePoint en línea. Para obtener más información sobre cómo aprovisionar un sitio de comunicación, vea Crear un sitio de comunicación [en SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) y siga los pasos para crear un sitio de comunicación.

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>Paso 4: agregar la aplicación Microsoft 365 caminos de aprendizaje al sitio

1. En el SharePoint, haga clic en el menú Sistema y, a continuación, **haga clic en Agregar una aplicación**. 
2. En **Aplicaciones ,** haga clic en Desde su **organización** y, a continuación, haga clic en Caminos de aprendizaje para **Office 365**. 

## <a name="step-5---set-permissions-for-the-site"></a>Paso 5: Establecer permisos para el sitio
Asegúrese de que se han establecido los siguientes permisos para el sitio:
- **Administrador de la colección** de sitios o parte del grupo Propietarios: permisos necesarios para inicializar el elemento de lista CustomConfig que configura las rutas de aprendizaje para su primer uso. 
- **Grupo de miembros:** permisos necesarios para administrar rutas de aprendizaje, como ocultar y mostrar contenido, y administrar listas de reproducción personalizadas
- **Grupo de visitantes:** permisos necesarios para ver el contenido del sitio. 

## <a name="step-6--execute-powershell-configuration-script"></a>Paso 6: Ejecutar script de configuración de PowerShell
Se incluye un script de PowerShell que deberá ejecutar para crear tres `CustomLearningConfiguration.ps1` propiedades [de inquilino](/sharepoint/dev/spfx/tenant-properties) que usa la solución. Además, el script crea dos [páginas](/sharepoint/dev/spfx/web-parts/single-part-app-pages) de aplicación de un solo elemento en la biblioteca de páginas del sitio para hospedar los elementos web de administrador y usuario en una ubicación conocida.

1. Si aún no has descargado el Shell de administración SharePoint online, descárbalo ahora. Consulte [SharePoint Descarga del Shell de administración en línea](https://go.microsoft.com/fwlink/p/?LinkId=255251).
2. Es posible que deba establecer una directiva de ejecución de PowerShell para ejecutar el script. Para obtener más información, vea [About Execution Policies](/powershell/module/microsoft.powershell.core/about/about_execution_policies).
3. Ejecute el `CustomLearningConfiguration.ps1` script. Además de las credenciales de administrador de inquilinos, el script le pedirá el nombre del inquilino y el nombre del sitio. Teniendo en cuenta el siguiente ejemplo para la dirección URL del sitio, , es el nombre `https://contoso.sharepoint.com/sites/O365CL` del inquilino y es el nombre del `contoso` `O365CL` sitio. 

### <a name="disabling-telemetry-collection"></a>Deshabilitar la colección de telemetría
Parte de esta solución incluye la opción de seguimiento de telemetría anonimizada, que de forma predeterminada está establecida en on. Si está realizando una instalación manual y desea desactivar el seguimiento de telemetría, cambie el script para establecer la variable $optInTelemetry en $false y ejecute `CustomlearningConfiguration.ps1` el script.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Validar el aprovisionamiento correcto e inicializar la lista CustomConfig

Después de ejecutar correctamente el script de PowerShell, navegue al sitio, inicialice el elemento de lista **CustomConfig** que configura las rutas de aprendizaje para su primer uso y valide que el sitio funciona.

- Ve a `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. Al abrir **CustomLearningAdmin. aspx** se inicializa el elemento de lista de **CustomConfig** que configura las rutas de aprendizaje para el primer uso. Debería ver una página con este aspecto:

![Página de la aplicación de administración](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Agregar propietarios al sitio
Como administrador de inquilinos, es poco probable que seas la persona que personalización del sitio, por lo que tendrás que asignar algunos propietarios al sitio. Los propietarios tienen privilegios administrativos en el sitio para que puedan modificar las páginas del sitio y cambiar el nombre del sitio. También tienen la capacidad de ocultar y mostrar el contenido entregado a través del elemento web caminos de aprendizaje. Además, tendrán la capacidad de crear listas de reproducción personalizadas y asignarlas a subcategorías personalizadas.  

1. En el menú SharePoint **Configuración,** haga clic en **Permisos del sitio**.
2. Haga **clic en Permisos Configuración**.
3. Haga **clic en Caminos de aprendizaje para Office 365 Propietarios**.
4. Haga **clic en** Agregar nuevos usuarios a este grupo y, a continuación, agregue las personas que desea que sean  >  propietarios. 
5. Agregue un vínculo a [Explorar el sitio](custom_exploresite.md) en el mensaje Compartir y, a continuación, haga clic en **Compartir**.

## <a name="migrate-custom-content"></a>Migrar contenido personalizado
Después de restablecer el sitio de rutas de aprendizaje siguiendo los pasos anteriores, deberá mover el contenido de la lista **CustomPlaylists** y la lista **CustomAssets.** También puede, opcionalmente, mover las páginas personalizadas reales que forma parte de los activos personalizados si viven en el sitio de rutas de aprendizaje existentes y su intención es eliminarlo. La tarea puede ser difícil porque para todos los elementos de la lista **CustomPlaylists,** el identificador del elemento de lista de la **lista CustomAssets** está en el campo JSONData de cada elemento de lista de listas de reproducción. Por lo tanto, simplemente mover el contenido de la **lista CustomPlaylists** de un sitio al otro no será suficiente. Además, la **lista CustomAssets** contiene la dirección URL absoluta de la página del activo personalizado en el campo JSONData del elemento de lista. Si los activos no se mueven y no se cambia el nombre del sitio (cambiando así la dirección URL absoluta a la página del activo), **customAssets** puede permanecer. Pero tendrá que corregir manualmente las entradas. Dada la complejidad de este tipo de migración, le recomendamos que considere la posibilidad de alistar uno de nuestros asociados de caminos de aprendizaje para ayudarle a realizar esta transición. 

### <a name="next-steps"></a>Siguientes pasos
- Vea [Personalizar las rutas de aprendizaje](custom_overview.md). 
- Vea [Traducir páginas de sitio](custom_translate_page_ml.md).