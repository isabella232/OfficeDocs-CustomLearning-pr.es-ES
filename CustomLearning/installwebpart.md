# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="4ef14-101">Instalar personalizados Webpart de solución de aprendizaje</span><span class="sxs-lookup"><span data-stu-id="4ef14-101">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="4ef14-102">Requisitos previos para una instalación de todo el inquilino</span><span class="sxs-lookup"><span data-stu-id="4ef14-102">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="4ef14-p101">Para instalar el elemento Web de aprendizaje personalizado para el inquilino de todo debe disponer de permisos administrativos de Office 365.  Si no tiene estos permisos puede trabajar con el Administrador de Office 365 o instale el elemento Web de una colección de sitios individuales.</span><span class="sxs-lookup"><span data-stu-id="4ef14-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="4ef14-105">Usted o el Administrador de Office 365 debe tener el programa de instalación y configura un [Catálogo de aplicaciones](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) de todo el inquilino o un [Catálogo de aplicaciones de colección de sitios](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)para recibir el elemento Web.]</span><span class="sxs-lookup"><span data-stu-id="4ef14-105">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="4ef14-p102">Sólo se admite SharePoint Online. El elemento web no es compatible para la instalación en cualquier versión de SharePoint local.</span><span class="sxs-lookup"><span data-stu-id="4ef14-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="4ef14-108">Agregar el elemento Web de aprendizaje personalizado a su inquilino</span><span class="sxs-lookup"><span data-stu-id="4ef14-108">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="4ef14-p103">Descargue el elemento Web de aprendizaje personalizado y guárdelo en la unidad local.  Este archivo se denomina "ms-custom-learning.sppkg".  No cambie el nombre o el sufijo del archivo.</span><span class="sxs-lookup"><span data-stu-id="4ef14-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="4ef14-112">Desplácese hasta el [portal de administración de Office 365](https://admin.microsoft.com/AdminPortal/Home#/homepage) para el inquilino</span><span class="sxs-lookup"><span data-stu-id="4ef14-112">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="4ef14-p104">En la barra de navegación izquierdo, seleccione centros de administrador de SharePoint. Se abrirá en una ficha nueva, en el centro de administración de SharePoint seleccionadas aplicaciones, catálogo de aplicaciones, aplicaciones para SharePoint</span><span class="sxs-lookup"><span data-stu-id="4ef14-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="4ef14-115">Seleccione carga el elemento Web y elija el archivo "ms-custom-learning.sppkg" que descargó</span><span class="sxs-lookup"><span data-stu-id="4ef14-115">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="4ef14-116">Para esta comprobación de la instalación de todo el inquilino la casilla junto a "Hacer esta solución esté disponible para todos se sitúa en la organización."</span><span class="sxs-lookup"><span data-stu-id="4ef14-116">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  

![Implementar solución](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="4ef14-118">Agregar el elemento Web de aprendizaje de cliente a una página de SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="4ef14-118">Add the Customer Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="4ef14-p105">Después de instalar Learning personalizado en el inquilino puede agregar el elemento Web a una página de SharePoint. Cuando lo hace, repentinamente formación de Office 365 está disponible.</span><span class="sxs-lookup"><span data-stu-id="4ef14-p105">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do, suddenly Office 365 training is available to you.</span></span> 

1. <span data-ttu-id="4ef14-121">Agregue el elemento Web de aprendizaje personalizado en un diseño de columnas de ancho completo:</span><span class="sxs-lookup"><span data-stu-id="4ef14-121">Add the Custom Learning webpart in a full width column layout:</span></span>

![Diseño de página de SharePoint](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="4ef14-p106">En la página de SharePoint, seleccione la sección Agregar y, a continuación, seleccione la columna de ancho completo.  Verá el mensaje siguiente:</span><span class="sxs-lookup"><span data-stu-id="4ef14-p106">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="4ef14-p107">Seleccione Microsoft Learning.  Ahora debería ver lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="4ef14-p107">Select Microsoft Learning.  You should now see the following:</span></span> 

![Custom webpart de aprendizaje](media/clo365addwebpart.png)

 <span data-ttu-id="4ef14-129">Ahora puede hacer clic en los mosaicos para explorar el contenido predeterminado incluido en la solución.</span><span class="sxs-lookup"><span data-stu-id="4ef14-129">You can now click on the tiles to explore the default content included in the solution.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="4ef14-130">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="4ef14-130">Next Steps</span></span>
- <span data-ttu-id="4ef14-131">Explore el [contenido predeterminado](webpartcontent.md) incluido en el elemento Web.</span><span class="sxs-lookup"><span data-stu-id="4ef14-131">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="4ef14-132">[Personalizar](customization.md) la experiencia de aprendizaje para la organización.</span><span class="sxs-lookup"><span data-stu-id="4ef14-132">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="4ef14-133">[Impulsar la adopción](driveadoption.md) de la solución de formación.</span><span class="sxs-lookup"><span data-stu-id="4ef14-133">[Drive adoption](driveadoption.md) of your training solution.</span></span>

