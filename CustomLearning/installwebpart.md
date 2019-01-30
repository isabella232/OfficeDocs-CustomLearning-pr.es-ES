# <a name="installing-the-custom-learning-solution-webpart"></a>Instalar personalizados Webpart de solución de aprendizaje

## <a name="prerequisites-for-a-tenant-wide-installation"></a>Requisitos previos para una instalación de todo el inquilino

- Para instalar el elemento Web de aprendizaje personalizado para el inquilino de todo debe disponer de permisos administrativos de Office 365.  Si no tiene estos permisos puede trabajar con el Administrador de Office 365 o instale el elemento Web de una colección de sitios individuales.
- Usted o el Administrador de Office 365 debe tener el programa de instalación y configura un [Catálogo de aplicaciones](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) de todo el inquilino o un [Catálogo de aplicaciones de colección de sitios](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)para recibir el elemento Web.]
- Sólo se admite SharePoint Online. El elemento web no es compatible para la instalación en cualquier versión de SharePoint local.

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a>Agregar el elemento Web de aprendizaje personalizado a su inquilino 

1. Descargue el elemento Web de aprendizaje personalizado y guárdelo en la unidad local.  Este archivo se denomina "ms-custom-learning.sppkg".  No cambie el nombre o el sufijo del archivo. 
2. Desplácese hasta el [portal de administración de Office 365](https://admin.microsoft.com/AdminPortal/Home#/homepage) para el inquilino
3. En la barra de navegación izquierdo, seleccione centros de administrador de SharePoint. Se abrirá en una ficha nueva, en el centro de administración de SharePoint seleccionadas aplicaciones, catálogo de aplicaciones, aplicaciones para SharePoint 
4. Seleccione carga el elemento Web y elija el archivo "ms-custom-learning.sppkg" que descargó
5. Para esta comprobación de la instalación de todo el inquilino la casilla junto a "Hacer esta solución esté disponible para todos se sitúa en la organización."  

![Implementar solución](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a>Agregar el elemento Web de aprendizaje de cliente a una página de SharePoint Online

Después de instalar Learning personalizado en el inquilino puede agregar el elemento Web a una página de SharePoint. Cuando lo hace, repentinamente formación de Office 365 está disponible. 

1. Agregue el elemento Web de aprendizaje personalizado en un diseño de columnas de ancho completo:

![Diseño de página de SharePoint](media/clo365fullcolumnwidth.png)

2. En la página de SharePoint, seleccione la sección Agregar y, a continuación, seleccione la columna de ancho completo.  Verá el mensaje siguiente:

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. Seleccione Microsoft Learning.  Ahora debería ver lo siguiente: 

![Custom webpart de aprendizaje](media/clo365addwebpart.png)

 Ahora puede hacer clic en los mosaicos para explorar el contenido predeterminado incluido en la solución.  

## <a name="next-steps"></a>Pasos siguientes
- Explore el [contenido predeterminado](webpartcontent.md) incluido en el elemento Web.
- [Personalizar](customization.md) la experiencia de aprendizaje para la organización.
- [Impulsar la adopción](driveadoption.md) de la solución de formación.

