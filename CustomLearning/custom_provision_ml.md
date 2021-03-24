---
author: pkrebs
ms.author: pkrebs
title: Aprovisionar una nueva solución multilingüe de caminos de aprendizaje
ms.date: 02/10/2019
description: Aprovisionar el sitio de rutas de aprendizaje de Microsoft 365 a través del servicio de aprovisionamiento de SharePoint
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint online
ms.openlocfilehash: 19de14ba0785fa394dfe65e50ba8c4f27864cccf
ms.sourcegitcommit: 907c657e7cc5a4a44d2b9f38cc35fea9ac5c5943
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/24/2021
ms.locfileid: "51163007"
---
# <a name="provision-a-new-learning-pathways-multilingual-solution"></a>Aprovisionar una nueva solución multilingüe de caminos de aprendizaje
Las organizaciones que no tienen caminos de aprendizaje aprovisionados en su inquilino pueden usar el Servicio de aprovisionamiento de SharePoint para agregar la solución de caminos de aprendizaje multilingüe. Con esta opción, la plantilla de SharePoint caminos de aprendizaje se traduce a nueve idiomas y se puede usar con un mínimo de modificación. 

> [!IMPORTANT]
> Si ya tienes las rutas de aprendizaje aprovisionadas en el espacio empresarial, se recomienda seguir la ruta de actualización para [las](custom_update_ml.md) rutas de aprendizaje. Si instala caminos de aprendizaje sobre una instancia existente en el inquilino, es posible que se pierdan los cambios realizados en la plantilla o listas de reproducción del sitio de caminos de aprendizaje.

## <a name="prerequisites-for-multilingual-support"></a>Requisitos previos para la compatibilidad multilingüe
 
Para configurar correctamente las rutas de aprendizaje de Microsoft 365 con el servicio de aprovisionamiento, la persona que realiza el aprovisionamiento debe cumplir los siguientes requisitos previos: 
 
- La persona que aprovisiona las rutas de aprendizaje debe ser un administrador de inquilinos del espacio empresarial donde se aprovisionarán las rutas de aprendizaje.  
- Un catálogo de aplicaciones de inquilino debe estar disponible en la opción Aplicaciones del Centro de administración de SharePoint. Si su organización no tiene un Catálogo de aplicaciones de inquilino de SharePoint, consulte la documentación [de SharePoint Online](/sharepoint/use-app-catalog) para crear uno. Debe esperar al menos dos horas después de crear el Catálogo de aplicaciones antes de aprovisionar las rutas de aprendizaje.  
- La persona que aprovisiona las rutas de aprendizaje debe ser un propietario de la colección de sitios del Catálogo de aplicaciones de inquilino. Si la persona que aprovisiona las rutas de aprendizaje no es un propietario de la colección de sitios del Catálogo de aplicaciones, [complete estas instrucciones](addappadmin.md) y continúe. 

## <a name="ensure-the-tenant-admin-account-doesnt-have-a-language-selected"></a>Asegúrese de que la cuenta de administrador de inquilinos no tenga un idioma seleccionado
Antes de aprovisionar rutas de aprendizaje, asegúrese de que la cuenta de administrador del inquilino no tenga un idioma seleccionado. Este es el modo de comprobar si la cuenta de administrador no tiene un idioma seleccionado. 
1.  Con tu perfil de administrador perimetral, ve a office.com.
2.  Escriba las credenciales de usuario (si es necesario).
3.  En Microsoft 365, haga clic en **Todas las aplicaciones** > Delve. 
4.  Haga **clic en Actualizar**  >  **perfil**.
5.  Desplácese hacia abajo en la página y haga clic en **Cómo puedo cambiar la configuración regional y de idioma.**
6.  Haga **clic aquí** y, a continuación, haga clic en los puntos **suspensivos ...**.
7.  En **Mis idiomas para mostrar,** debería ver **No hay idiomas seleccionados**. Si se selecciona un idioma, anule la selección.

### <a name="to-provision-learning-pathways"></a>Para aprovisionar caminos de aprendizaje

1. Vaya a la página de soluciones de caminos de aprendizaje de [Microsoft 365](https://provisioning.sharepointpnp.com/details/3df8bd55-b872-4c9d-88e3-6b2f05344239).
2. Haga **clic en Agregar a su espacio empresarial.** Si no ha iniciado sesión en su inquilino, el servicio de aprovisionamiento pedirá sus credenciales de administrador de inquilinos. 
3. En el cuadro de diálogo Permisos solicitados, seleccione **Consentimiento en nombre de su organización** y, a continuación, seleccione **Aceptar**.

El servicio de aprovisionamiento requiere estos permisos para crear el catálogo de aplicaciones de inquilino, instalar la aplicación en el catálogo de aplicaciones del inquilino y aprovisionar la plantilla de sitio. No hay ningún impacto general en el espacio empresarial. Estos permisos se usan explícitamente para la instalación de la solución. Debe aceptar estos permisos para continuar con la instalación.

4. Rellene los campos de la página de información de aprovisionamiento según corresponda para su instalación. Como mínimo, debe escribir la dirección de correo electrónico en la que desea recibir notificaciones sobre el proceso de aprovisionamiento y el prefijo de la dirección URL del sitio que se aprovisionará.  
> [!NOTE]
> Haga que los empleados puedan usar la dirección URL de destino de manera fácil con nombres como "/sites/MyTraining" o "/teams/LearnMicrosoft365".

![inst_options.png](media/inst_options.png)

6. Haga **clic en Aprovisionar** cuando esté listo para instalar rutas de aprendizaje en el entorno de inquilino.  El proceso de aprovisionamiento puede tardar hasta 15 minutos. Recibirá una notificación por correo electrónico cuando el sitio esté listo. 

> [!IMPORTANT]
> El administrador de inquilinos que aprovisiona el sitio de rutas de aprendizaje debe ir al sitio y, a continuación, abrir **CustomLearningAdmin.aspx para** inicializar las propiedades de administración de caminos de aprendizaje. En este momento, el administrador de inquilinos también debe asignar propietarios al sitio. 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Validar el aprovisionamiento correcto e inicializar la lista CustomConfig

Una vez completado el aprovisionamiento, el administrador de inquilinos que aprovisionó el sitio recibe un correo electrónico del Servicio de aprovisionamiento pnP. El correo electrónico contiene un vínculo al sitio. En este momento, el administrador de inquilinos debe ir al sitio mediante el vínculo proporcionado en el correo electrónico y configurar el sitio para su primer uso:

- Vaya a `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`. Al abrir **CustomLearningAdmin. aspx** se inicializa el elemento de lista de **CustomConfig** que configura las rutas de aprendizaje para el primer uso. Debería ver una página con este aspecto:

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Agregar propietarios al sitio
Como administrador de inquilinos, es poco probable que seas la persona que personalización del sitio, por lo que tendrás que asignar algunos propietarios al sitio. Los propietarios tienen privilegios administrativos en el sitio para que puedan modificar las páginas del sitio y cambiar el nombre del sitio. También tienen la capacidad de ocultar y mostrar contenido y crear subcategorías y listas de reproducción personalizadas.  

1. En el menú Configuración **de** SharePoint, haga clic **en Permisos del sitio**.
2. Haga **clic en Configuración avanzada de permisos**.
3. Haga clic **en Caminos de aprendizaje de Microsoft 365 Propietarios**.
4. Haga **clic en** Agregar nuevos usuarios a este grupo y, a continuación, agregue las personas que desea que sean  >  propietarios. 
5. Agregue un vínculo a [Explorar el sitio](custom_exploresite.md) en el mensaje Compartir y, a continuación, haga clic en **Compartir**.

## <a name="add-translators-to-the-site"></a>Agregar traductores al sitio
Si va a usar traductores para el sitio, puede asignarles permisos. Los traductores requieren permisos de miembro o superiores. 

## <a name="choose-options-for-using-multiple-languages-on-the-site"></a>Elegir opciones para usar varios idiomas en el sitio
El servicio de aprovisionamiento de SharePoint crea el sitio Caminos de aprendizaje en nueve idiomas. Se aplican las siguientes recomendaciones:
- Desactivar los idiomas que no desea admitir
- Si no admite un sitio multilingüe, desactive la característica multilingüe. Vea la sección "Desactivar compatibilidad multilingüe" más adelante en este tema.

### <a name="remove-languages-you-dont-want-to-support"></a>Quitar idiomas que no desea admitir
Para las organizaciones que deciden admitir solo un idioma, además del idioma inglés predeterminado, se recomienda quitar los idiomas que no son compatibles. 
1. En el sitio Caminos de aprendizaje, seleccione **Configuración** en la parte superior derecha de la página y, a continuación, seleccione **Información del sitio**.
2. En la parte inferior del panel de información del sitio, seleccione **Ver toda la configuración del sitio**.
3. En **Administración del sitio**, seleccione Configuración de **idioma**.
4. En **Habilitar que las páginas y las noticias se traduzcan a varios idiomas,** deslice el botón de alternancia a **On**. Debe ser On de forma predeterminada.
5. En Agregar o quitar idiomas de sitio, haga clic en **Quitar** para quitar los idiomas que no necesita para el sitio. A continuación se muestra un ejemplo de la página Configuración de idioma para mostrar el italiano admitido para el sitio, además del idioma inglés predeterminado.

![custom_update_ml_langsettings.png](media/custom_update_ml_langsettings.png)

> [!NOTE]
> Al quitar idiomas, no se puede quitar el idioma inglés predeterminado. 

### <a name="assign-translators"></a>Asignar traductores
Si va a traducir páginas, asigne opcionalmente uno o más traductores para cada idioma (excepto el idioma predeterminado del sitio). 
- En la **columna Traductor,** empiece a escribir el nombre de una persona que desea ser traductora y, a continuación, seleccione el nombre de la lista. 

> [!NOTE]
> Cualquier persona de Active Directory de su organización se puede asignar como traductor. Las personas asignadas como traductores no tendrán automáticamente los permisos adecuados. Cuando alguien sin permisos de edición para un sitio intente obtener acceso al sitio, se le dirigirá a una página web donde pueda solicitar acceso.

## <a name="turn-off-multilingual-support"></a>Desactivar la compatibilidad multilingüe
Si no desea un sitio multilingüe, por ejemplo, desea un sitio solo en inglés, se recomienda desactivar la característica multilingüe. 

1. En el sitio Caminos de aprendizaje, seleccione **Configuración** en la parte superior derecha de la página y, a continuación, seleccione **Información del sitio**.
2. En la parte inferior del panel de información del sitio, seleccione **Ver toda la configuración del sitio**.
3. En **Administración del sitio**, seleccione Configuración de **idioma**.
4. En **Habilitar que las páginas y las noticias se traduzcan a varios idiomas,** deslice el botón de alternancia a **On**. Debe ser On de forma predeterminada.
- En **Habilitar que se traduzcan** páginas y noticias, seleccione **Desactivar**. 

### <a name="add-languages"></a>Agregar idiomas
Las rutas de aprendizaje admiten 9 idiomas, pero se recomienda agregar solo los idiomas que necesita para admitir el sitio de rutas de aprendizaje. Puede agregar langauges en cualquier momento. 
- En **Agregar o quitar idiomas de sitio,** empiece a escribir un nombre de idioma en Seleccionar o **escribir** un idioma, o elija un idioma en la lista desplegable. Puede repetir este paso para agregar varios idiomas. Puede agregar o quitar idiomas de su sitio en cualquier momento si vuelve a esta página.