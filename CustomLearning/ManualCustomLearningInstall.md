---
author: pkrebs
ms.author: pkrebs
title: Instalación manual de caminos de aprendizaje
ms.date: 02/18/2019
manager: bpardi
description: Instalación manual de caminos de aprendizaje
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: 6f106b569602730f16fc2b6f8a09fa44667e32e1
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575975"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>Instalación y configuración manual de Aprendizaje personalizado para Office 365

El elemento web de aprendizaje personalizado de Microsoft se compila [con la SharePoint Framework](/sharepoint/dev/spfx/sharepoint-framework-overview) versión 1.7.1.

Para instalar y configurar manualmente el elemento web y la colección de sitios, deberá completar los pasos siguientes:

1. Valide que ha cumplido todos los requisitos previos.
1. Instale el archivo customlearning.sppkg en el catálogo de aplicaciones Office 365 inquilino.
1. Aprovisionar e identificar un sitio de comunicación moderno para que actúe como su aprendizaje personalizado para Office 365 sitio principal.
1. Ejecute un script de PowerShell que configurará el espacio empresarial con los artefactos adecuados de los que depende aprendizaje personalizado.
1. Vaya a la página de sitio CustomLearningAdmin.aspx para cargar el elemento web de administración para inicializar la configuración de contenido personalizada.

## <a name="prerequisites"></a>Requisitos previos

Debe haber configurado y configurado el Catálogo de aplicaciones para todo el espacio empresarial. Consulta [Configurar el espacio empresarial Office 365 y](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) sigue la sección Crear sitio del catálogo de aplicaciones. Si el Catálogo de aplicaciones de todo el espacio empresarial ya se ha aprovisionado, necesitarás acceso a una cuenta que tenga derechos para cargar un paquete en él para completar este proceso de configuración. Por lo general, esta cuenta tiene el SharePoint de administrador. Si una cuenta con ese rol no funciona, vaya al Centro de administración de SharePoint y busque los administradores de la colección de sitios para la colección de sitios del catálogo de aplicaciones e inicie sesión como uno de los administradores de la colección de sitios o agregue la cuenta de administrador de SharePoint que no pudo con los administradores de la colección de sitios. También necesitarás acceso a una cuenta que sea un administrador SharePoint inquilino.

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>Upload el elemento web al Catálogo de aplicaciones de inquilino

Para configurar El aprendizaje personalizado para Office 365, cargue el archivo customlearning.sppkg en el Catálogo de aplicaciones de todo el espacio empresarial e impleméntelo. Consulta [Usar el Catálogo de](/sharepoint/use-app-catalog) aplicaciones para que las aplicaciones empresariales personalizadas estén disponibles para tu entorno de SharePoint Online para obtener instrucciones detalladas sobre cómo agregar una aplicación al catálogo de aplicaciones.

## <a name="provisionidentify-modern-communication-site"></a>Aprovisionar e identificar sitio de comunicación moderna

Identifique un sitio de SharePoint de comunicación existente o aprovisione uno nuevo en su SharePoint en línea. Para obtener más información acerca de cómo aprovisionar un sitio de comunicación, vea Crear un sitio de comunicación en [SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) y siga los pasos para crear un sitio de comunicación.

## <a name="set-permissions-for-the-site"></a>Establecer permisos para el sitio

Querrá agregar todos los usuarios que deberían poder ver contenido al grupo Visitantes y a todos los usuarios que deberían poder administrar listas de reproducción personalizadas al grupo Miembros. Para configurar el sitio para Aprendizaje personalizado la primera vez que el usuario debe ser un administrador de la colección de sitios o parte del grupo Propietarios.

Agregue Aprendizaje personalizado para Office 365 aplicación a la colección de sitios.

## <a name="execute-powershell-configuration-script"></a>Ejecutar script de configuración de PowerShell

Se incluye un script de PowerShell que deberá ejecutar para crear tres `CustomLearningConfiguration.ps1` propiedades [de inquilino](/sharepoint/dev/spfx/tenant-properties) que usa la solución. Además, el script crea dos [páginas](/sharepoint/dev/spfx/web-parts/single-part-app-pages) de aplicación de un solo elemento en la biblioteca de páginas del sitio para hospedar los elementos web de administrador y usuario en una ubicación conocida.

### <a name="disabling-telemetry-collection"></a>Deshabilitar la colección de telemetría

Parte de esta solución incluye la suscripción de seguimiento de telemetría anonimizada, que de forma predeterminada está establecida en on. Si realiza una instalación manual y desea desactivar el seguimiento de telemetría, cambie el script para establecer la variable $optInTelemetry `CustomlearningConfiguration.ps1` en $false.

Si no realiza una instalación manual y desea desactivar el seguimiento de telemetría, se ha incluido un script independiente que al ejecutarse deshabilitará el seguimiento `TelemetryOptOut.ps1` de telemetría.

## <a name="initialize-web-part-custom-configuration"></a>Inicializar la configuración personalizada del elemento web

Después de ejecutar correctamente el script de PowerShell, vaya a `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` . Esto inicializa el elemento de lista CustomConfig que configura el aprendizaje personalizado para su primer uso.

La configuración ya está completa y puede seguir adelante con el uso de Aprendizaje personalizado para Office 365. Consulte la documentación del usuario para obtener más información.
