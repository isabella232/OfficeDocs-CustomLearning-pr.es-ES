---
author: pkrebs
ms.author: pkrebs
title: Aprovisionar el sitio de aprendizaje personalizado
ms.date: 02/10/2019
description: Aprovisionar el sitio de aprendizaje personalizado para Office 365 a través del motor de aprovisionamiento de SharePoint
ms.openlocfilehash: 868708f9f096c84d5ebc5f9bc4e21e558da84d2b
ms.sourcegitcommit: 5ea8d7fdc255ef7de06f41b3c794bc40551cf5bb
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/14/2019
ms.locfileid: "30577866"
---
# <a name="provision-custom-learning"></a>Aprovisionar aprendizaje personalizado 

Con el servicio de aprovisionamiento de SharePoint Online, un administrador de inquilinos de Office 365 puede iniciar el proceso de aprovisionamiento con unos pocos clics sencillos. El servicio de aprovisionamiento es la forma recomendada para aprovisionar aprendizaje personalizado. Es rápido y sencillo, y tarda solo unos minutos en iniciar el proceso. Sin embargo, antes de empezar con el servicio de aprovisionamiento, asegúrese de que cumple con los requisitos previos para el aprovisionamiento.

## <a name="prerequisites"></a>Requisitos previos
 
Para configurar correctamente el aprendizaje personalizado con el servicio de aprovisionamiento, la persona que realiza el aprovisionamiento debe cumplir los siguientes requisitos previos: 
 
- La persona que aprovisiona el aprendizaje personalizado debe ser un administrador de inquilinos del inquilino en el que se aprovisionará el aprendizaje personalizado.  
- Un catálogo de aplicaciones del espacio empresarial debe estar disponible en la opción de aplicaciones del centro de administración de SharePoint. Si su organización no tiene un catálogo de aplicaciones del espacio empresarial de SharePoint, consulte la [documentación de SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) para crear uno.  
- La persona que aprovisiona el aprendizaje personalizado debe ser un propietario de la colección de sitios del catálogo de aplicaciones del espacio empresarial. Si la persona que aprovisiona el aprendizaje personalizado no es un propietario de la colección de sitios del catálogo de aplicaciones, [complete estas instrucciones](addappadmin.md) y continúe. 

### <a name="to-provision-custom-learning"></a>Para aprovisionar aprendizaje personalizado

1. Vaya a http://provisioning.sharepointpnp.com e **inicie sesión** desde la esquina superior derecha de la Página principal.  Inicie sesión con las credenciales del inquilino de destino donde tiene previsto instalar la plantilla de sitio.

![pnphome. png](media/inst_signin.png)

2. Borre el **consentimiento en nombre de su organización** y seleccione **Aceptar**.

![a](media/inst_perms.png)

3. Desplácese hacia abajo en la página, seleccione la pestaña **soluciones** y, después, seleccione **aprendizaje personalizado para Office 365**. 

![a](media/inst_select.png)

4. Seleccione **Agregar al espacio empresarial**

![inst_select. png](media/inst_add.png)

5. Complete los campos en la página de información de aprovisionamiento según corresponda para su instalación. Como mínimo, escriba la dirección de correo electrónico donde desea obtener las notificaciones sobre el proceso de aprovisionamiento y la dirección URL de destino para el que se va a aprovisionar el sitio.  
> [!NOTE]
> Haga que la dirección URL de destino del sitio sea descriptiva para los empleados, como "/sites/MyTraining" o "/teams/LearnOffice365".

![inst_options. png](media/inst_options.png)

6. Seleccione **provisión** cuando esté listo para instalar aprendizaje personalizado en su entorno de espacio empresarial.  El proceso de aprovisionamiento llevará hasta 15 minutos. Recibirá una notificación por correo electrónico (a la dirección de correo electrónico de notificación que escribió en la página de aprovisionamiento) cuando el sitio esté preparado para el acceso. 

> [!IMPORTANT]
> El administrador de inquilinos que aprovisiona el sitio de aprendizaje personalizado debe ir al sitio y, a continuación, abrir **CustomLearningAdmin. aspx** para inicializar las propiedades de administración de aprendizaje personalizadas. En este momento, el administrador de inquilinos también debe asignar propietarios al sitio. 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Validar el aprovisionamiento correcto e inicializar la lista de CustomConfig

Cuando el aprovisionamiento haya finalizado, el administrador de inquilinos que aprovisionó el sitio recibirá un correo electrónico del servicio de aprovisionamiento de PnP. El correo electrónico contiene un vínculo al sitio. En este momento, el administrador de inquilinos debe ir al sitio mediante el vínculo proporcionado en el correo electrónico y configurar el sitio para el primer uso:

- Vaya a `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`. Al abrir **CustomLearningAdmin. aspx** se inicializa el elemento de lista **CustomConfig** que configura el aprendizaje personalizado para el primer uso. Debería ver una página similar a la siguiente:

![CG-adminapppage. png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Agregar propietarios al sitio
Como administrador de inquilinos, es poco probable que sea la persona que va a personalizar el sitio, por lo que necesitará asignar algunos propietarios al sitio. Los propietarios tienen privilegios administrativos en el sitio para que puedan modificar las páginas del sitio y remarcar el sitio. También tienen la posibilidad de ocultar y mostrar contenido entregado a través del elemento Web de aprendizaje personalizado. Además, tendrán la capacidad de crear listas de reproducción personalizadas y asignarlas a subcategorías personalizadas.  

1. En el menú **configuración** de SharePoint, haga clic en **permisos del sitio**.
2. Haga clic en **Configuración avanzada de permisos**.
3. Haga clic en **aprendizaje personalizado para los propietarios de Office 365**.
4. Haga clic en **nuevo** > **Agregar usuarios a este grupo**y, a continuación, agregue las personas que desea que sean propietarios. 
5. Agregue un vínculo para [explorar el sitio](custom_exploresite.md) en el mensaje de uso compartido y, a continuación, haga clic en **compartir**.

### <a name="next-steps"></a>Pasos siguientes
- Explore el [contenido predeterminado](custom_exploresite.md) proporcionado en el sitio y el elemento Web.
