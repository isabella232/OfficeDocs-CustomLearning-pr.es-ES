---
author: pkrebs
ms.author: pkrebs
title: Modelos de integración de socios
ms.date: 3/9/2019
description: Modelos de integración de socios
ms.service: sharepoint online
ms.openlocfilehash: 91980782f64d101d3128daff81ed4e2b6205faa8
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/23/2020
ms.locfileid: "48234142"
---
# <a name="partner-integration-models"></a>Modelos de integración de socios
Aunque no es posible complementar el contenido de las rutas de aprendizaje de Microsoft 365 de forma directa del servicio de aprovisionamiento de SharePoint Online, hay varios modelos de integración que los asociados pueden aprovechar para crear ofertas de servicio de valor agregado alineadas. Los modelos de integración del asociado se presentan en orden de complejidad ascendente y niveles de inversión. Por lo tanto, nuestra orientación es desarrollar su experiencia y expartirla con niveles más avanzados en función de los modelos de negocio.

![cg-part-intmodel.png](media/cg-part-intmodel.png) 

## <a name="how-should-i-get-started"></a>¿Cómo debo empezar? 
Para empezar, siga estos procedimientos recomendados.     

### <a name="1-begin-with-building-expertise-as-an-enabler"></a>1. Comience con la experiencia del edificio como un habilitador. 
Puede ayudar de inmediato un porcentaje de la base de clientes mediante la habilitación de su portal de aprendizaje de rutas de aprendizaje y la realización de curation de contenido de Microsoft dirigidas. Para obtener instrucciones sobre el aprovisionamiento de rutas de aprendizaje, consulte https://docs.microsoft.com/office365/customlearning/custom_provision .  

### <a name="2-then-extend-your-services-as-an-integrator"></a>2. a continuación, amplíe los servicios como un integrador
Realice una devolución de automatización en el análisis de la inversión, en función de la cantidad de contenido o de las necesidades de integración de servicios. Por ejemplo, es posible que no tenga sentido realizar el desarrollo y los costos operativos con respecto a nuestras pautas de integración de contenido si puede crear rápidamente de forma manual una lista o listas de reproducción personalizadas específicas que apunten a su contenido para pagar o hacer referencia a sus servicios.

### <a name="3-when-the-return-on-investment-makes-sense--consider-redistribution"></a>3. cuando la devolución de la inversión tenga sentido, tenga en cuenta la redistribución 
Cuando la rentabilidad de la inversión tenga sentido, tenga en cuenta la redistribución (o el trabajo con asociados de aprendizaje de caminos relacionados) para crear soluciones reempaquetadas. Se basan en el marco de patrones y prácticas de SharePoint, que proporciona soluciones para extraer sitios personalizados y luego implementarlos en entornos de clientes. 

## <a name="partner-provided-content-integration-guidelines"></a>Instrucciones para la integración de contenido proporcionada por el asociado
El contenido para los caminos de aprendizaje de Microsoft 365 está controlado por un conjunto de archivos JSON que actúan como manifiestos de contenido para el paquete de aprendizaje. Hay tres archivos: metadata.js, playlists.jsy assets.jsen. Estos archivos deben estructurarse para que se correspondan con los modelos que reconoce el elemento Web y, a continuación, se hospeda desde una red de entrega de contenido (CDN) para permitir que el elemento web los cargue. Microsoft proporcionará plantillas iniciales de estos archivos para ayudarle a empezar.  

**Declinación de responsabilidades:** la estructura del archivo JSON está sujeta a cambios en función de un trabajo de solución próximo. El programa de adopción anticipada del socio de caminos de aprendizaje de Microsoft 365 (EAP) se informará de los cambios inminentes de este tipo. Junto con cualquier orientación sobre la compatibilidad con versiones anteriores de los clientes o la transición. 

### <a name="download-the-microsoft-365-learning-pathways-solution"></a>Descargue la solución de caminos de aprendizaje de Microsoft 365
Puede descargar la solución de caminos de aprendizaje de Microsoft 365, junto con los archivos JSON, desde el repositorio de GitHub: https://github.com/pnp/custom-learning-office-365 . Tenga en cuenta que en este momento, Microsoft no va a realizar la solicitud de extracción de GitHub en la solución. Pero puede usar los archivos de GitHub como punto de partida para crear su propio paquete de contenido personalizado. 

### <a name="metadatajson-structure"></a>Metadata.jsen la estructura
Puede considerar este archivo como el cerebro de los menús y la estructura. Contiene toda la estructura de navegación y listas de selección para los datos de los otros dos archivos. 


|              Nombre        |                     Descripción                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|**Tecnologías**              |El contenido se etiqueta y se puede ocultar en función de la tecnología a la que se asigna.                 |  
|&nbsp;&nbsp;Identificador                |GUID que representa la tecnología                                                           |  
|&nbsp;&nbsp;Denomina              |Nombre para mostrar de la tecnología                                                             |
|&nbsp;&nbsp;*Asuntos []*     |Una matriz de temas que son un subconjunto de la tecnología                                   | 
|&nbsp;&nbsp;&nbsp;&nbsp;Identificador    |GUID que representa el asunto                                                              |
|&nbsp;&nbsp;&nbsp;&nbsp;Denomina  |Nombre para mostrar del asunto                                                                |
|**Categories []**             |Las categorías informan a la navegación del elemento Web. Cada categoría representa un nivel superior de la navegación                                                                                                                 |
|&nbsp;&nbsp;Identificador                |GUID que representa la categoría o Subcategoría                                                 |
|&nbsp;&nbsp;Denomina              |Nombre para mostrar de la categoría o Subcategoría                                                  |
|&nbsp;&nbsp;Imagen             |Dirección URL de la imagen que se debe mostrar en la experiencia de usuario (relativa a la base de la red CDN)            |
|&nbsp;&nbsp;TechnologyId      |El GUID de la tecnología a la que está relacionado este contenido (opcional: cadena vacía)            |
|&nbsp;&nbsp;SubjectId         |El GUID del tema con el que está relacionado este contenido (opcional: cadena vacía)               |
|&nbsp;&nbsp;Orígenes            |De la matriz de origen, que no se usa específicamente en la experiencia del usuario que no sea datos personalizados agregados por el usuario, se marca como "inquilino" y el área de administración de la experiencia de usuario no permite la edición de nada no marcado como "tenant".                           |
|&nbsp;&nbsp;*Subcategoras []*|Las subcategorías son básicamente el nivel de navegación desde el nivel 2 hacia abajo. La estructura es la misma que una categoría que solo está anidada.          |
|**Audiencias []**             |Cuando las listas de reproducción asociadas a una categoría o subcategoría son varias audiencias etiquetadas, un selector estará disponible para mostrar las audiencias disponibles. |         
|&nbsp;&nbsp;Identificador                |GUID de la audiencia                                                                       |  
|&nbsp;&nbsp;Denomina              |Nombre para mostrar de la audiencia                                                               |       
|**Orígenes []**               |Matriz de cadenas que etiquetan contenido con su origen, que no se usa específicamente en una experiencia de usuario distinta de los datos personalizados agregados por el usuario, se marca como "tenant" y el área de administración de la UX no permite la edición de nada que no esté marcado como "tenant".                                                   |  
|**Niveles []**               |Cuando las listas de reproducción asociadas a una categoría o subcategoría tienen varios niveles etiquetados, un selector estará disponible para mostrar los niveles disponibles.             |  
|&nbsp;&nbsp;Identificador                |GUID del nivel                                                                          |  
|&nbsp;&nbsp;Denomina              |Nombre para mostrar del nivel                                                                  | 
|**StatusTag [ ]**           |La etiqueta de estado es identificar el contenido con varios Estados que se expondrán en la experiencia de usuario. Algunas de estas marcas se mostrarán al consumidor y otras solo al administrador.                                                   |  
|&nbsp;&nbsp;Identificador                |GUID de la StatugTag                                                                      |  
|&nbsp;&nbsp;Denomina              |Nombre para mostrar de la StatusTag                                                              | 
|**Telemetría []**            |                                                                                           |  
|&nbsp;&nbsp;AppInsightsKey    |GUID de la clave de la aplicación Insights que ha configurado para realizar un seguimiento de la carga del elemento Web del visor. Un administrador puede desactivar el seguimiento para todo el inquilino, pero la información enviada es anonimizan usuario con el identificador de inquilino. Consulte esta sección para obtener más información. https://github.com/pnp/custom-learning-office-365#disabling-telemetry-collection               |  
|**Version**                   |La solución usa la información de versión para indicar a los administradores que el elemento Web se ha actualizado y también permite que el elemento Web actualice automáticamente el contenido personalizado a la versión más reciente del manifiesto si se han realizado cambios significativos.         | 
|&nbsp;&nbsp;Complemento          |La versión del manifiesto                                               |
|&nbsp;&nbsp;ManifestMinWebPart|La versión mínima del elemento Web que funciona con la versión del manifiesto.             |
|&nbsp;&nbsp;CurrentWebPart    |Dirección URL de la imagen que se debe mostrar en la experiencia de usuario (relativa a la base de la red CDN)            |
|&nbsp;&nbsp;Reviertel           |La dirección URL del repositorio donde se encuentran las instrucciones de actualización del elemento Web.                    |
|**Paquetes de contenido**             |En este momento, no se admiten los paquetes de contenido para CDN adicionales. Los paquetes de contenido permiten a Microsoft sugerir otras soluciones creadas por Microsoft que se pueden aprovisionar a través del servicio de aprovisionamiento que aprovechan M365LP para entregar contenido y se encuentran en y por sí mismos redes CDN personalizadas.       | 
|&nbsp;&nbsp;Identificador                |GUID del paquete de contenido/red CDN                                                              |
|&nbsp;&nbsp;Denomina              |Nombre para mostrar de la red CDN                                                                   |
|&nbsp;&nbsp;Descriptiva       |Descripción que se va a mostrar en la interfaz de usuario para agregar un paquete de contenido                               |
|&nbsp;&nbsp;Imagen             |Imagen que se mostrará en la interfaz de usuario para agregar un paquete de contenido                                     |
|&nbsp;&nbsp;ProvisionURL      |La dirección URL del paquete del servicio de aprovisionamiento para crear la colección de sitios del paquete de contenido.  |
|&nbsp;&nbsp;CDNbase           |La dirección URL base para los manifiestos del paquete de contenido                                       |
|AssetOrigins                  |Matriz de origen de dirección URL que se utiliza en el assets.jsen el archivo que se describe más adelante. Si la dirección URL de origen lo admite, se enviará un mensaje post a help_getClientHeight. Una respuesta en la propiedad data de: "help_getClientHeight = {height of Content}" (por ejemplo, "help_getClientHeight = 5769") permitirá cambiar el tamaño del iFrame al alto apropiado del contenido entramado.         |

### <a name="playlistsjson-structure"></a>Playlists.jsen la estructura
playlists.json: el manifiesto de listas de reproducción es una matriz de objetos que describe los metadatos sobre una lista de reproducción y los activos incluidos en la lista de reproducción.

|              Nombre        |                     Descripción                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|Id                            |GUID que representa la lista de reproducción                                                             |  
|El título                         |Nombre para mostrar de la lista de reproducción                                                               |
|Imagen                         |Dirección URL relativa (desde la red CDN) a una imagen para visualizar la lista de reproducción                              |                      
|LevelId                       |Nivel asociado                                                                           |
|AudienceId                   |Audiencia asociada                                                                        |
|TechnologyId                 |Tecnología asociada                                                                      |
|SubjectId                    |Nombre para mostrar de la categoría o Subcategoría                                                  |
|Origen                        |De la matriz de origen, no se usa específicamente en una experiencia de usuario que no sea datos personalizados agregados por el usuario, se marca como "tenant" y el área de administración de la UX no permite la edición de nada que no esté marcado como "tenant".                                              |
|CatId                         |La categoría o identificador de subcategoría que representa el contenedor en el que se debe mostrar la lista de reproducción. Actualmente, el manifiesto no es compatible con la selección de una categoría o subcategoría como contenedor si también tiene elementos secundarios de la subcategoría.        |
|Descripción                   |Se mostró una descripción de cada lista de reproducción en la experiencia de usuario                                           |
|StatusTagId                   |Etiqueta de estado asociada                                                                      |
|StatusNote                    |Notas sobre el contenido que se muestra a los administradores                                            |
|*Activos []*                        |Una matriz de GUID para los activos que forman parte de esta lista de reproducción, en orden de presentación.        |         

### <a name="assetjson-structure"></a>Asset.jsen la estructura
playlists.json: el manifiesto de listas de reproducción es una matriz de objetos que describe los metadatos sobre una lista de reproducción y los activos incluidos en la lista de reproducción.

|              Nombre        |                     Descripción                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|Id                            |GUID que representa la lista de reproducción                                                             |  
|El título                         |Nombre para mostrar de la lista de reproducción                                                               |
|Descripción                   |---                                                                                           |                      
|URL                           |La dirección URL de origen para el activo, que se aplicará al iFrame                                  |
|TechnologyId                  |Tecnología asociada                                                                      |
|SubjectId                     |Asunto asociado                                                                         |
|Origen                        |Nombre para mostrar de la categoría o Subcategoría                                                  |
|StatusTagId                   |Etiqueta de estado asociada                                                                      |
|StatusNote                    |Notas sobre el contenido que se muestra a los administradores.                                           |

### <a name="caching"></a>Almacenamiento en caché
La versión actual del elemento Web del visor usa una versión en caché de los archivos del manifiesto durante 24 horas. Transcurridas 24 horas, el primer usuario que ha encontrado el elemento Web asume el rendimiento necesario para actualizar la caché mediante la descarga de los manifiestos de la red CDN de origen y la combinación de la información con las tecnologías ocultas y las listas de reproducción, así como la combinación de subcategorías, listas de reproducción y activos personalizados. De forma alternativa, el elemento Web de administración siempre descarga el contenido de los manifiestos y los combina en y actualiza la memoria caché.  Por lo tanto, en otras palabras, el administrador puede forzar una actualización de caché en cualquier momento si carga el elemento Web de administración, conocido como ir a la página de administración.

## <a name="content-pack-guidelines"></a>Instrucciones del paquete de contenido
La característica de paquete de contenido Desbloquea los siguientes escenarios:
- La capacidad de los socios para redistribuir el contenido de aprendizaje personalizado agregado de valor personalizado adaptado al entorno de los clientes
- La capacidad de las organizaciones con un equipo de aprendizaje seguro y el soporte técnico de TI para crear contenido de aprendizaje personalizado dirigido a sus propios sistemas y gobernanza internos.
- La capacidad para que Microsoft entregue caminos de aprendizaje adicionales en el futuro que los clientes pueden participar

Este conjunto de documentación actual está destinado de forma intencionada a los asociados debido a la complejidad de la característica. El equipo de servicio está trabajando activamente para mejorar la compatibilidad con el escenario #2, en el futuro. 

### <a name="how-content-packs-work"></a>Funcionamiento de los paquetes de contenido
Microsoft usa páginas de GitHub como origen de red de entrega de contenido (CDN) para sus archivos de manifiesto e imágenes. Tenemos una carpeta docs en la raíz de nuestro repositorio de GitHub que incluye subcarpetas para cada versión de los archivos del manifiesto. Dentro de cada carpeta hay tres archivos de manifiesto, más una carpeta de imágenes para almacenar todas las imágenes de categorías, subcategorías y listas de reproducción. 

Es importante que mantenga la misma estructura de versiones que Microsoft tiene que elegir para extender la solución de rutas de aprendizaje con su propio paquete de contenido. El punto de conexión de la red CDN no debe incluir la carpeta versión, ya que la versión del manifiesto que admite el elemento Web es compatible y se anexa automáticamente a la dirección URL de la red CDN. Obviamente le proporcionaremos tiempo para crear nuevas instancias de los archivos del manifiesto en cualquier momento en que se revisen.

![cg-part-json-folder.png](media/cg-part-json-folder.png) 

Para obtener más información sobre cómo usar las páginas de GitHub como su origen de red CDN, consulte la siguiente documentación de ayuda: [https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages](https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages) .

La solución de Microsoft hace que la información sobre los activos se abra al público, ya que no hay seguridad alguna que tenga acceso a estos archivos. Creemos que debe haber una capa de contenido gratuita para un consumidor, lo que decía que si necesita una pared de pago para parte o todo el contenido, necesitará implementar esto de forma distinta dentro de las limitaciones técnicas de la solución y el uso de páginas de GitHub no es en absoluto un requisito. Cualquier proveedor de CDN que quiera usar es adecuado si mantiene la estructura de numeración de versiones que hemos esquematizado. Como se indicó anteriormente, la versión de la estructura del manifiesto que admite el elemento Web está integrada en el código y se anexa automáticamente a la dirección URL de la red CDN. 

### <a name="content-pack-integration-guidance"></a>Guía de integración del paquete de contenido 
Los elementos Web de administrador y visor se han ampliado para permitir que el consumidor configure puntos de conexión de la red CDN adicionales en su inquilino, lo que permitirá al elemento Web del visor seleccionar la red CDN que deben origen de los datos que muestran. 

Tramas clave que se deben tener en cuenta para esta característica: 
- Este es el principal aplicable a los escenarios de redistribución de asociados (donde la configuración manual de la lista de reproducción es demasiado engorroso) 
- Los paquetes de contenido personalizados son una característica avanzada que solo deben usar los socios con experiencia en la administración de contenido Web. Los orígenes de contenido no confiables pueden introducir contenido no seguro en el sitio. Solo debe agregar orígenes en los que confíe.

> **Importante** Antes de agregar un paquete de contenido personalizado, debe haber proporcionado rutas de aprendizaje de Microsoft 365 3,0 o posterior. Para informataion sobre el aprovisionamiento de caminos de aprendizaje de Microsoft 365, consulte [provision microsoft 365 Learning Pathways](https://docs.microsoft.com/office365/customlearning/custom_provision).

### <a name="content-whitelisting"></a>Lista de retenciones de contenido
Como asociado, tiene la responsabilidad de ayudar a los consumidores a asegurarse de que el contenido se encuentra en la lista de su entorno. Le sugerimos que cree un escenario de prueba en su entorno para validar que el contenido puede ser iFrame en una página de SharePoint dentro de su firewall. Siga las instrucciones [de creación de páginas de SharePoint para las listas de reproducción personalizadas](https://docs.microsoft.com/office365/customlearning/custom_createnewpage) para confirmar que este es el caso.

### <a name="add-a-content-pack-to-learning-pathways"></a>Adición de un paquete de contenido a las rutas de aprendizaje
Una vez que haya creado el JSON modificado y definido su red CDN, puede Agregar el paquete de contactos a las rutas de aprendizaje. 

1. En la página de **Inicio** del sitio de caminos de aprendizaje, seleccione **Inicio** y, a continuación, haga clic en administración de **rutas de aprendizaje**. 
2. En la página **Administración** , haga clic en **... Agregue el paquete de contenido** en la esquina superior derecha de la página.
3. Haga clic en paquete de contenido personalizado y, a continuación, escriba un nombre para el paquete de contenido y, a continuación, especifique la red CDN donde se encuentran los archivos JSON.

![cg-part-addconpack.png](media/cg-part-addconpack.png)

4. Haga clic en **Guardar **. El contenido del paquete de contenido personalizado debería aparecer ahora en la página de administración. Aquí le mostramos un ejemplo. 

![cg-part-addconpackex.png](media/cg-part-addconpackex.png)

### <a name="filter-to-the-content-pack-in-the-web-part"></a>Filtrar al paquete de contenido en el elemento Web
Con las rutas de aprendizaje, puede Agregar el elemento Web de rutas de aprendizaje a una página, filtrar el elemento Web para que apunte al origen del paquete de contenido personalizado y, a continuación, filtrar el elemento Web a la categoría, subcategoría, lista de reproducción y elemento que desee. 

1. En el sitio de caminos de aprendizaje, haga clic en **nueva**y, a continuación, en **Página**.
2. Haga clic en **en blanco**y, a continuación, en **Crear página**.
3. Asigne un nombre a la página. 
4. Haga clic en **+ Agregar una nueva sección** en el lado izquierdo de la página.
5. Haga clic **+** en la parte superior central de la sección nueva y, a continuación, agregue el elemento Web de **caminos de aprendizaje de Microsoft 365** .
6. Haga clic en el elemento Web y, a continuación, haga clic en el icono **Editar** .
7. En el cuadro **Seleccionar origen de aprendizaje** , seleccione el paquete de contenido personalizado y, a continuación, filtre el elemento Web por el contenido que desee. A continuación, se proporciona un ejemplo del elemento Web filtrado para una lista de reproducción de un paquete de contenido personalizado.

![cg-part-conpackfilter.png](media/cg-part-conpackfilter.png)  




