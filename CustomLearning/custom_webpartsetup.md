---
author: pkrebs
ms.author: pkrebs
title: Aprovisionar el sitio de aprendizaje personalizado
ms.date: 02/10/2019
description: Aprovisionar el sitio de aprendizaje personalizado para Office 365 a través del motor de aprovisionamiento de SharePoint
ms.openlocfilehash: 83d76d2d12e9dfc0f39ef55c58443cb3fda2a2d9
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523614"
---
# <a name="provision-custom-learning"></a>Aprovisionar aprendizaje personalizado

Con el servicio de aprovisionamiento de SharePoint Online, un administrador de inquilinos de Office 365 puede iniciar el proceso de aprovisionamiento con unos pocos clics sencillos. El servicio de aprovisionamiento es la forma recomendada para aprovisionar aprendizaje personalizado. Es rápido y sencillo, y tarda solo unos minutos en iniciar el proceso. Sin embargo, antes de empezar con el servicio de aprovisionamiento, asegúrese de que cumple con los requisitos previos para el aprovisionamiento.

## <a name="prerequisites"></a>Requisitos previos
 
Para configurar correctamente el aprendizaje personalizado con el servicio de aprovisionamiento de [SharePoint Online](https://provisioning.sharepointpnp.com)provisioning, la persona que realiza el aprovisionamiento debe cumplir los siguientes requisitos previos: 
 
- La persona que aprovisiona el aprendizaje personalizado debe ser un administrador de inquilinos del inquilino en el que se aprovisionará el aprendizaje personalizado.  
- Un catálogo de aplicaciones del espacio empresarial debe estar disponible en la opción de aplicaciones del centro de administración de SharePoint. Si su organización no tiene un catálogo de aplicaciones del espacio empresarial de SharePoint, consulte la [documentación de SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) para crear uno.  
- La persona que aprovisiona el aprendizaje personalizado debe ser un propietario de la colección de sitios del catálogo de aplicaciones del espacio empresarial. Si la persona que aprovisiona el aprendizaje personalizado no es un propietario de la colección de sitios del catálogo de aplicaciones, [complete estas instrucciones](addappadmin.md) y continúe. 

### <a name="to-provision-custom-learning"></a>Para aprovisionar aprendizaje personalizado

1. Vaya a http://provisioning.sharepointpnp.com e **inicie sesión** desde la esquina superior derecha de la Página principal.  Inicie sesión con las credenciales del inquilino de destino donde tiene previsto instalar la plantilla de sitio.

![pnphome. png](media/inst_signin.png)

2. Borre el **consentimiento en nombre de su organización** y seleccione **Aceptar**.

![a](media/inst_perms.png)

3. Seleccione **aprendizaje personalizado para Office 365** en la galería de soluciones.

![a](media/inst_select.png)

4. En la Página principal de la solución, seleccione **Agregar al espacio empresarial** .

![inst_select. png](media/inst_add.png)

5. Complete los campos en la página de información de aprovisionamiento según corresponda para su instalación. Como mínimo, escriba la dirección de correo electrónico donde desea obtener las notificaciones sobre el proceso de aprovisionamiento y la dirección URL de destino para el que se va a aprovisionar el sitio.  
> [!NOTE]
> Haga que la dirección URL de destino del sitio sea descriptiva para los empleados, como "/sites/MyTraining" o "/teams/LearnOffice365".

![inst_options. png](media/inst_options.png)

6. Seleccione **provisión** cuando esté listo para instalar aprendizaje personalizado en su entorno de espacio empresarial.  El proceso de aprovisionamiento llevará hasta 15 minutos. Recibirá una notificación por correo electrónico (a la dirección de correo electrónico de notificación que escribió en la página de aprovisionamiento) cuando el sitio esté preparado para el acceso.

> [!IMPORTANT]
> El administrador de inquilinos que aprovisiona el sitio de aprendizaje personalizado debe ir al sitio y, a continuación, abrir CustomLearningAdmin. aspx para inicializar las propiedades de administración de aprendizaje personalizadas. En este momento, el administrador de inquilinos también debe asignar propietarios al sitio. 

## <a name="validate-provisioning-success"></a>Validar el éxito del aprovisionamiento

Cuando el aprovisionamiento haya finalizado, el administrador de inquilinos recibirá un correo electrónico del servicio de aprovisionamiento de PnP. El administrador puede copiar el vínculo en el sitio proporcionado en el correo electrónico y, a continuación, seguir las instrucciones para ir al sitio. Como alternativa, el administrador de inquilinos puede navegar a <YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin. aspx. Esto inicializa el elemento de lista CustomConfig que configura el aprendizaje personalizado para su primer uso. La persona que abre la página por primera vez debe ser un administrador de inquilinos, un administrador de la colección de sitios o el propietario del sitio. Debería ver una página similar a la siguiente: 

## <a name="add-owners-to-site"></a>Agregar propietarios al sitio
Como administrador de inquilinos, es poco probable que sea la persona que va a personalizar el sitio, por lo que necesitará asignar propietarios al sitio. Los propietarios tienen privilegios administrativos en el sitio para que puedan modificar las páginas del sitio y remarcar el sitio. También tienen la posibilidad de ocultar y mostrar contenido entregado a través del elemento Web de aprendizaje personalizado. También tendrán la capacidad de crear una lista de reproducción personalizada y asignarlas a subcategorías personalizadas.  

1. En el menú **configuración** de SharePoint, haga clic en **permisos del sitio**.
2. Haga clic en **Configuración avanzada de permisos**.
3. Haga clic en **aprendizaje personalizado para los propietarios de Office 365**.
4. Haga clic en **nuevo** > **Agregar usuarios a este grupo**, agregue a los usuarios que desea que sean propietarios y, a continuación, haga clic en **compartir**.

8. Haga clic en la **siguiente** opción en la esquina superior derecha de la página para seguir el sitio.  

### <a name="next-steps"></a>Pasos siguientes
- Explore el [contenido predeterminado](sitecontent.md) incluido en el elemento Web.
