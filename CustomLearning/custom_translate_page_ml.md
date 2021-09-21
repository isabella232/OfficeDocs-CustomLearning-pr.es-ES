---
author: pkrebs
ms.author: pkrebs
title: Traducir páginas del sitio
ms.date: 07/06/2020
description: Traducir páginas del sitio
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 87130512dafe55ddd7dd0ac4f0667efb2108f360
ms.sourcegitcommit: 6005c2551bdea334767e6a056fdcb79533f2c858
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/21/2021
ms.locfileid: "59460928"
---
# <a name="translate-site-pages"></a>Traducir páginas del sitio
Antes de empezar a traducir el sitio de rutas de aprendizaje, es importante comprender algunos conceptos clave de cómo funciona la característica multilingüe con las rutas de aprendizaje. 
- Información del sitio: la navegación, el logotipo y las traducciones de nombres de sitio requieren que el sitio se vea y traduzca en el perfil de idioma del usuario.  
- El elemento web caminos de aprendizaje debe visualizarse con el perfil de idioma del usuario para que aparezca en un idioma que no sea inglés. El elemento web y el contenido proporcionado por Microsoft ya están traducidos por usted. Para obtener más información acerca de los perfiles de idiomas, vea [Cambiar el idioma personal y la configuración regional.](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7)
- La forma en que configura las rutas de aprendizaje determina si tiene las páginas traducidas disponibles. Los nuevos sitios aprovisionados con el Microsoft 365 de búsqueda tendrán páginas traducidas en nueve idiomas disponibles. Los sitios o sitios actualizados que cree necesitarán traducción manual. Consulte [Opciones de configuración para las rutas de aprendizaje multilingües.](custom_setupoptions_ml.md)
- La compatibilidad multilingüe con las rutas de aprendizaje está habilitada SharePoint las características multilingües en línea para los sitios de comunicación. Para obtener información sobre SharePoint multilingües en línea, vea Crear sitios de comunicación [multilingües, páginas y noticias](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c). 

## <a name="working-with-a-newly-provisioned-site"></a>Trabajar con un sitio recién aprovisionado
Si aprovisionó un nuevo sitio de rutas de aprendizaje desde el servicio de Microsoft 365 de búsqueda, las páginas traducidas ya están disponibles. De forma predeterminada, el sitio proporciona las páginas siguientes:

- Home.aspx
- Start-with-Six-Simple-Steps.aspx
- Get-started-with-Microsoft-365.aspx
- Get-started-with-Microsoft-Teams.aspx
- Get-started-with-SharePoint.aspx
- Get-started-with-OneDriive.aspx
- Ask-questions-and-get-help.aspx
- Eventos de aprendizaje calendar.aspx
- Become-a-Champion.aspx
- Recommended-Playlists.aspx
- Learning de administración de rutas de acceso

## <a name="view-translated-pages-from-the-newly-provisioned-site"></a>Ver páginas traducidas desde el sitio recién aprovisionado
Para familiarizarse con el sitio de caminos de aprendizaje traducido, echemos un vistazo a algunas páginas traducidas.

### <a name="view-the-translated-home-page"></a>Ver la página principal traducida
En la página principal de caminos de aprendizaje, seleccione un idioma en el desplegable de idioma como se muestra en el ejemplo siguiente. En el ejemplo, verá el italiano seleccionado en la esquina superior derecha y se traducen todos los elementos de página.

![custom_ml página principal](media/custom_ml_pages_home.png)

### <a name="view-the-translated-microsoft-365-training-page"></a>Ver la página de aprendizaje Microsoft 365 traducción
Ahora echemos un vistazo a la página de Microsoft 365 aprendizaje. 

1. En la página principal del sitio de caminos de **aprendizaje,** **haga clic Microsoft 365 aprendizaje.**
2. En la esquina superior derecha de la página, seleccione un idioma. En este ejemplo, se selecciona italiano.

![custom_ml_ de aprendizaje](media/custom_ml_pages_training.png)

¿Qué traducciones son visibles cuando se selecciona el idioma?
- La SharePoint se traduce como se muestra en el gráfico anterior. Observe que el texto del banner de página está ahora en italiano.

¿Qué son las traducciones no visibles?
- El nombre del sitio está en inglés
- La navegación del sitio está en inglés
- El elemento web caminos de aprendizaje está en inglés

## <a name="view-the-fully-translated-site"></a>Ver el sitio completamente traducido 
Para ver un sitio completamente traducido en un idioma específico, incluidas las páginas del sitio, la navegación y el elemento web, el idioma personal y la configuración regional del usuario deben establecerse para ese idioma. Para obtener más información sobre cómo establecer el idioma y la configuración regional, vea [Cambiar el idioma personal y la configuración regional.](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7) Se recomienda usar una cuenta independiente o que otro usuario con la configuración de idioma diferente vea las páginas traducidas.  

## <a name="working-with-an-updated-or-manually-installed-learning-pathways-site"></a>Trabajar con un sitio de rutas de aprendizaje actualizado o instalado manualmente
Si actualizó un sitio Learning Pathways o instaló manualmente el elemento web en un sitio existente, deberá traducir manualmente las páginas del sitio. El elemento web y el contenido de las rutas de aprendizaje ya están traducidos y aparecerán en el idioma preferido del usuario. Para traducir páginas, consulta las siguientes instrucciones "Crear páginas para los idiomas que quieras". 

## <a name="create-pages-for-the-languages-you-want"></a>Crear páginas para los idiomas que desee
Una vez que hayas habilitado el sitio para características multilingües y hayas elegido los idiomas que quieres que estén disponibles, puedes crear las páginas de traducción que quieras. 

1. Vaya a la página de idioma predeterminada que desea que esté disponible en otro idioma.
2. En la barra superior, seleccione **Traducción**.
3. Seleccione **Crear** para los idiomas que desee.

> [!IMPORTANT]
> Después de crear las páginas de traducción, debe publicar (o volver a publicar) la página de idioma predeterminada para asegurarse de que:
>- Las páginas de traducción se muestran en el sitio de idioma correspondiente.
>- Las páginas de traducción se muestran correctamente en el elemento web Noticias y los elementos web contenido resaltado.
>- El desplegable de idioma en la parte superior del sitio incluye todos los idiomas que ha habilitado.
>- Se notifica a los traductores de la solicitud de traducción.

Después de crear las páginas, el estado de la página (borrador guardado, publicado, y así sucesivamente) se muestra en el panel de traducción junto a cada idioma. Además, los traductores que asignó recibirán una notificación por correo electrónico de que se solicita una traducción.

### <a name="view-the-fully-translated-site-in-a-specific-language"></a>Ver el sitio completamente traducido en un idioma específico
Para ver un sitio completamente traducido en un idioma específico, incluidas las páginas del sitio, la navegación y el elemento web, el idioma personal y la configuración regional del usuario deben establecerse para ese idioma. Para obtener más información sobre cómo establecer el idioma y la configuración regional, vea [Cambiar el idioma personal y la configuración regional.](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7) Ten en cuenta que es mejor usar una cuenta independiente o que otro usuario con la configuración de idioma diferente vea las páginas traducidas.

## <a name="what-does-a-translator-do"></a>¿Qué hace un traductor?
 Después de configurar el sitio en inglés, un usuario con el español como su idioma personal preferido, por ejemplo, edita y traduce manualmente el título, la navegación y el contenido del pie de página al español. Un usuario con el alemán como su idioma personal preferido hace lo mismo con el alemán. Una vez traducido el contenido, se mostrará a todos los usuarios de esos idiomas preferidos. El elemento web recoge el idioma preferido del usuario y muestra el contenido traducido a ese idioma. 

Los traductores traducen manualmente las copias de la página de idioma predeterminada a los idiomas especificados. Cuando se crean las copias de las páginas, se notifica a los traductores por correo electrónico si se ha especificado un traductor. El correo electrónico incluye un vínculo a la página de idioma predeterminada y a la página de traducción recién creada. El traductor:
1. Seleccione el **botón Empezar a traducir** en el correo electrónico.
2. Seleccione **Editar** en la parte superior derecha de la página y traduzca el contenido.
3. Cuando haya terminado, seleccione Guardar como borrador **(si** no está listo para que sea visible para los lectores) o  si la página está lista para ser visible para todos los usuarios que usan ese idioma en el sitio, seleccione Publicar o **Publicar** noticias .

Para obtener más información sobre el proceso de traducción, vea Crear sitios de [comunicación multilingües, páginas y noticias](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c). 

## <a name="updating-the-default-language-page"></a>Actualización de la página de idioma predeterminada
Cuando se actualiza la página de idioma predeterminada, la página debe volver a publicarse. A continuación, se notifica por correo electrónico a los traductores de las páginas de traducción que se ha realizado una actualización para que se puedan realizar actualizaciones en las páginas de traducción individuales.

## <a name="set-up-a-multilingual-site-name-navigation-and-footer"></a>Configurar un nombre de sitio multilingüe, navegación y pie de página
Para mostrar el nombre del sitio, la navegación y el pie de página de su sitio en los diferentes idiomas que ha puesto a disposición, cada uno debe ser traducido manualmente.

Por ejemplo, digamos que ha creado un sitio de comunicación con un idioma por defecto, el inglés, y ha habilitado el sitio para los idiomas español y alemán. Cuando se crea un sitio, se establece el nombre del sitio y la descripción en el idioma predeterminado (en este caso, el inglés). También puede actualizar el nombre y la descripción del sitio después de su creación. Luego crea los nodos de navegación y el contenido del pie de página en inglés.

Después de que el sitio se configura en inglés, un usuario con el español como su idioma personal preferido edita manualmente y traduce el título, la descripción, la navegación y el contenido del pie de página al español. Un usuario con el alemán como su idioma personal preferido hace lo mismo con el alemán. Una vez traducido el contenido, se mostrará a todos los usuarios de esos idiomas preferidos. 

> [! NOTAS]
>- Los usuarios que traduzcan el contenido del sitio para sus idiomas preferidos deben ser miembros del grupo Propietarios del sitio o tener permisos de sitio equivalentes.
>- Si se realiza un cambio en el nombre del sitio, la navegación o el pie de página en el idioma predeterminado, el elemento traducido correspondiente a otro idioma no se actualiza automáticamente a menos que elija sobrescribir las traducciones de sitio existentes. Si lo hace, el elemento traducido se reemplaza por la actualización en el idioma predeterminado y tendría que traducirse manualmente de nuevo. Para sobrescribir las traducciones, vaya a la página Idiomas del sitio para el idioma predeterminado y seleccione Mostrar configuración avanzada. A continuación, deslice el botón de alternancia para Sobrescribir traducciones a On. Esta opción no se aplica al contenido de páginas o noticias.

### <a name="to-view-the-fully-translated-site-in-a-specific-language"></a>Para ver el sitio completamente traducido en un idioma específico
Para ver un sitio completamente traducido en un idioma específico, incluidas las páginas del sitio, la navegación y el elemento web, el idioma personal y la configuración regional del usuario deben establecerse para ese idioma. Para obtener más información sobre cómo establecer el idioma y la configuración regional, vea [Cambiar el idioma personal y la configuración regional.](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7) Se recomienda usar una cuenta independiente o que otro usuario con la configuración de idioma diferente vea las páginas traducidas.

## <a name="for-more-information"></a>Más información
- Para obtener más información acerca de cómo traducir SharePoint de sitio de comunicación, vea Crear sitios de comunicación multilingües, [páginas y noticias](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).
- Para obtener más información acerca de cómo personalizar las rutas de aprendizaje, [vea Personalizar Learning caminos](custom_overview.md).  
