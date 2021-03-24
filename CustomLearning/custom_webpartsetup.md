---
author: pkrebs
ms.author: pkrebs
title: Aprovisionar el sitio de aprendizaje personalizado
ms.date: 02/10/2019
description: Aprovisionar el sitio de aprendizaje personalizado para Office 365 a través del motor de aprovisionamiento de SharePoint
ms.service: sharepoint online
ms.openlocfilehash: be45ade7588f08801062710d310ca967ddd23926
ms.sourcegitcommit: 907c657e7cc5a4a44d2b9f38cc35fea9ac5c5943
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/24/2021
ms.locfileid: "51162927"
---
# <a name="provision-custom-learning"></a>Aprovisionar aprendizaje personalizado

Con el Servicio de aprovisionamiento de SharePoint Online, un administrador de inquilinos de Office 365 puede iniciar el proceso de aprovisionamiento con unos clics sencillos. El servicio de aprovisionamiento es la forma recomendada de aprovisionar aprendizaje personalizado. Es rápido, fácil y tarda solo unos minutos en iniciar el proceso. Sin embargo, antes de empezar a usar el servicio de aprovisionamiento, asegúrese de que ha cumplido los requisitos previos para el aprovisionamiento.

## <a name="prerequisites"></a>Requisitos previos
 
Para configurar correctamente aprendizaje personalizado con el servicio de aprovisionamiento de [SharePoint Online Service,](https://provisioning.sharepointpnp.com)la persona que realiza el aprovisionamiento debe cumplir los siguientes requisitos previos: 
 
- La persona que aprovisiona Aprendizaje personalizado debe ser un administrador de inquilinos del espacio empresarial en el que se aprovisionará Aprendizaje personalizado.  
- Un catálogo de aplicaciones de inquilino debe estar disponible en la opción Aplicaciones del Centro de administración de SharePoint. Si su organización no tiene un catálogo de aplicaciones de inquilino de SharePoint, consulte la [documentación de SharePoint Online](/sharepoint/use-app-catalog) para crear uno.  
- La persona que aprovisiona Aprendizaje personalizado debe ser el propietario de una colección de sitios del Catálogo de aplicaciones de inquilino. Si la persona que aprovisiona Aprendizaje personalizado no es un propietario de la colección de sitios del Catálogo de [aplicaciones, complete estas instrucciones](addappadmin.md) y continúe. 

### <a name="to-provision-custom-learning"></a>Para aprovisionar aprendizaje personalizado

1. Vaya a e inicie sesión desde la esquina superior http://provisioning.sharepointpnp.com derecha de la página principal.   Inicie sesión con las credenciales del inquilino de destino donde tiene previsto instalar la plantilla de sitio.

![pnphome.png](media/inst_signin.png)

2. Desactive el **consentimiento en nombre de su organización** y seleccione **Aceptar**.

![en ](media/inst_perms.png)

3. Seleccione **Aprendizaje personalizado para Office 365** en la galería de soluciones.

![en ](media/inst_select.png)

4. En la página principal de la solución, **seleccione Agregar a su inquilino**

![inst_select.png](media/inst_add.png)

5. Rellene los campos de la página de información de aprovisionamiento según corresponda para su instalación. Como mínimo, escriba la dirección de correo electrónico en la que desea obtener notificaciones sobre el proceso de aprovisionamiento y la dirección URL de destino del sitio al que se aprovisionará.  
> [!NOTE]
> Haga que la dirección URL de destino del sitio sea algo descriptivo para sus empleados, como "/sites/MyTraining" o "/teams/LearnOffice365".

![inst_options.png](media/inst_options.png)

6. Seleccione **Aprovisionar** cuando esté listo para instalar Aprendizaje personalizado en el entorno de inquilino.  El proceso de aprovisionamiento tardará 15 minutos como máximo. Recibirá una notificación por correo electrónico (en la dirección que haya introducido en la página de aprovisionamiento para recibir notificaciones) cuando el sitio esté preparado para el acceso.

> [!IMPORTANT]
> El administrador de inquilinos que aprovisiona el sitio de aprendizaje personalizado debe ir al sitio y, a continuación, abrir CustomLearningAdmin.aspx para inicializar las propiedades del administrador de aprendizaje personalizado. En este momento, el administrador de inquilinos también debe asignar propietarios al sitio. 

## <a name="validate-provisioning-success"></a>Validar el éxito del aprovisionamiento

Una vez completado el aprovisionamiento, el administrador de inquilinos recibe un correo electrónico del servicio de aprovisionamiento pnP. El administrador puede copiar el vínculo al sitio proporcionado en el correo electrónico y, a continuación, seguir las instrucciones para ir al sitio. Como alternativa, el administrador de inquilinos puede navegar hasta <your-site-collection-url>/SitePages/CustomLearningAdmin.aspx. Esto inicializa el elemento de lista CustomConfig que configura El aprendizaje personalizado para su primer uso. La persona que abre esta página por primera vez debe ser un administrador de inquilinos, un administrador de la colección de sitios o el propietario del sitio. Debería ver una página con este aspecto: 

## <a name="add-owners-to-site"></a>Agregar propietarios al sitio
Como administrador de inquilinos, es poco probable que seas la persona que personalización del sitio, por lo que tendrás que asignar propietarios al sitio. Los propietarios tienen privilegios administrativos en el sitio para que puedan modificar las páginas del sitio y cambiar el nombre del sitio. También tienen la capacidad de ocultar y mostrar el contenido entregado a través del elemento web aprendizaje personalizado. También tendrán la capacidad de crear listas de reproducción personalizadas y asignarlas a subcategorías personalizadas.  

1. En el menú Configuración **de** SharePoint, haga clic **en Permisos del sitio**.
2. Haga **clic en Configuración avanzada de permisos**.
3. Haga **clic en Aprendizaje personalizado para propietarios de Office 365.**
4. Haga **clic en** Agregar nuevos usuarios a este grupo, agregue las personas que desea que sean  >  propietarios y, a continuación, haga clic en **Compartir**.

8. Haga clic **en la opción** Siguiente en la esquina superior derecha de la página para seguir el sitio.  

### <a name="next-steps"></a>Siguientes pasos
- Explore el [contenido predeterminado](sitecontent.md) incluido en el elemento web.