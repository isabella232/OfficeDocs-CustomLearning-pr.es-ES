# <a name="customize-the-services-and-playlists"></a><span data-ttu-id="d44ca-101">Personalizar los servicios y las listas de reproducción</span><span class="sxs-lookup"><span data-stu-id="d44ca-101">Customize the Services and Playlists</span></span>

<span data-ttu-id="d44ca-p101">De forma predeterminada la experiencia del sitio y el elemento Web incluyen contenido para todos los servicios de Office 365.  Si sólo hay todos o algunos de estos servicios están disponibles en su compañía puede ajustar el contenido que está disponible para los usuarios.  En este artículo se va a personalizar el contenido del elemento Web.</span><span class="sxs-lookup"><span data-stu-id="d44ca-p101">By default both the site experience and the webpart include content for all Office 365 services.  If only all or some of these services are available in your company you can adjust what content is available to your users.  In this article we will customize the webpart content.</span></span>  

## <a name="customizing-the-webpart-content"></a><span data-ttu-id="d44ca-105">Personalizar el contenido del elemento Web</span><span class="sxs-lookup"><span data-stu-id="d44ca-105">Customizing the webpart content</span></span>

<span data-ttu-id="d44ca-106">El elemento Web de aprendizaje personalizado proporciona dos características claves:</span><span class="sxs-lookup"><span data-stu-id="d44ca-106">The Custom Learning webpart provides two key features:</span></span>
- <span data-ttu-id="d44ca-107">Mostrar u ocultar tecnologías</span><span class="sxs-lookup"><span data-stu-id="d44ca-107">Hide/Show Technologies</span></span>
- <span data-ttu-id="d44ca-108">Crear una lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="d44ca-108">Create a Playlist</span></span>

### <a name="hide-or-show-technology-categories"></a><span data-ttu-id="d44ca-109">Ocultar o mostrar categorías de tecnología</span><span class="sxs-lookup"><span data-stu-id="d44ca-109">Hide or Show Technology Categories</span></span>

<span data-ttu-id="d44ca-110">Para ocultar y mostrar el contenido en el elemento Web:</span><span class="sxs-lookup"><span data-stu-id="d44ca-110">To hide and show content in the Web part:</span></span> 
1.  <span data-ttu-id="d44ca-111">Haga clic en el menú desplegable en el elemento Web, a continuación, haga clic en Mostrar u ocultar tecnologías</span><span class="sxs-lookup"><span data-stu-id="d44ca-111">Click the dropdown menu on the webpart, then click Hide/Show Technologies</span></span>

![Opción de menú](media/clohideshow.png)

2. <span data-ttu-id="d44ca-113">Seleccione un checkox para ocultar o mostrar una tecnología y seleccione **Aplicar**.</span><span class="sxs-lookup"><span data-stu-id="d44ca-113">Select a checkox to hide or show a technology and select **Apply**.</span></span>

![Opciones de tecnología](media/clohideshow1.png)

### <a name="create-a-playlist"></a><span data-ttu-id="d44ca-115">Crear una lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="d44ca-115">Create a Playlist</span></span>

<span data-ttu-id="d44ca-p102">Una lista de reproducción es un compliation de "activos". Un "activo" es una página de SharePoint o un elemento existente de contenido de aprendizaje de Microsoft. Cuando se crea una lista de reproducción seleccione los activos que van conjuntamente para crear una ruta de aprendizaje para el usuario.</span><span class="sxs-lookup"><span data-stu-id="d44ca-p102">A playlist is a compliation of "assets". An "asset" is a SharePoint page or existing item of Microsoft training content. When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="d44ca-p103">La ventaja de la adición de las páginas de SharePoint es que puede crear las páginas de SharePoint con un YouTube vídeos o vídeos que se hospeda en su organización. También puede crear las páginas con formularios u otro contenido de Office 365.</span><span class="sxs-lookup"><span data-stu-id="d44ca-p103">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization. You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="d44ca-121">Paso 1: Crear una página de SharePoint para la lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="d44ca-121">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="d44ca-p104">En este ejemplo, crearemos en primer lugar una página de SharePoint para agregar a la lista de reproducción. Crearemos una página con un elemento web de vídeo de YouTube y el elemento web de texto.  Estas instrucciones suponen que está utilizando el servicio de SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="d44ca-p104">In this example, we’ll first create a SharePoint page to add to the playlist. We’ll create a page with a YouTube video web part and Text web part.  These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="d44ca-125">Crear una nueva página</span><span class="sxs-lookup"><span data-stu-id="d44ca-125">Create a new page</span></span>
1.  <span data-ttu-id="d44ca-126">Seleccione la configuración menú > contenidos del sitio > las páginas del sitio > nuevo > página del sitio.</span><span class="sxs-lookup"><span data-stu-id="d44ca-126">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="d44ca-127">En el área de título, escriba Use el cuadro de comando de los equipos</span><span class="sxs-lookup"><span data-stu-id="d44ca-127">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="d44ca-128">Seleccione la sección Agregar una nueva y, a continuación, seleccione dos columnas.</span><span class="sxs-lookup"><span data-stu-id="d44ca-128">Select the Add a new section, and then select Two Columns.</span></span>

![Agregue dos columnas](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="d44ca-130">En el cuadro izquierdo, seleccione Agregar un nuevo elemento web y, a continuación, seleccione incrustar.</span><span class="sxs-lookup"><span data-stu-id="d44ca-130">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="d44ca-131">En un explorador Web, vaya a esta dirección URL https://youtu.be/wYrRCRphrp0 y obtener el código para insertar el vídeo.</span><span class="sxs-lookup"><span data-stu-id="d44ca-131">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="d44ca-132">En el elemento SharePoint Web, seleccione Agregar incrustar código y, a continuación, péguelo en el cuadro Insertar.</span><span class="sxs-lookup"><span data-stu-id="d44ca-132">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="d44ca-133">En el cuadro de la derecha, seleccione Agregar un nuevo elemento web y, a continuación, seleccione texto.</span><span class="sxs-lookup"><span data-stu-id="d44ca-133">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="d44ca-p105">En un explorador Web, vaya a esta dirección URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b y copie el bloque Try se! Instrucciones de la página y péguelas en el elemento Web de texto. La página debe tener un aspecto similar al siguiente.</span><span class="sxs-lookup"><span data-stu-id="d44ca-p105">In a Web browser, go to this URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it! Instructions from the page and paste them into the Text Web part. Your page should look like the following.</span></span> 

![Insertar página](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="d44ca-138">Haga clic en publicar y, a continuación, copie la dirección URL de la página y péguelo en el Bloc de notas</span><span class="sxs-lookup"><span data-stu-id="d44ca-138">Click Publish, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="d44ca-139">Paso 2: Crear la lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="d44ca-139">Step 2: Create the Playlist</span></span>
1.  <span data-ttu-id="d44ca-p106">Vaya a donde ha instalado el elemento Web de aprendizaje personalizado. En la experiencia del sitio completo está hospedado en la página de recursos de aprendizaje de Office 365.</span><span class="sxs-lookup"><span data-stu-id="d44ca-p106">Navigate to where you have installed the Custom Learning webpart. In the full site experience it is hosted on the Office 365 training page.</span></span> 
2.  <span data-ttu-id="d44ca-142">En el menú desplegable, seleccione Crear nueva lista de reproducción.</span><span class="sxs-lookup"><span data-stu-id="d44ca-142">From the dropdown menu select Create New Playlist.</span></span> 

![Crear lista de reproducción personalizada](media/clo365createplaylist.png)

3.  <span data-ttu-id="d44ca-144">Rellene los valores como se muestra en el ejemplo siguiente y seleccione **crear**.</span><span class="sxs-lookup"><span data-stu-id="d44ca-144">Fill in the values as shown in the example below and select **Create**.</span></span> 

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="d44ca-145">Paso 3: Agregar activos a la lista de reproducción</span><span class="sxs-lookup"><span data-stu-id="d44ca-145">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="d44ca-146">En este paso, agregará los activos existentes de Microsoft y la página de SharePoint que creó para la lista de reproducción.</span><span class="sxs-lookup"><span data-stu-id="d44ca-146">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1.  <span data-ttu-id="d44ca-147">Haga clic en el botón menú y, a continuación, haga clic en Agregar activo existente.</span><span class="sxs-lookup"><span data-stu-id="d44ca-147">Click the menu button, then click Add Existing Asset.</span></span>

![Adición de activos](media/clo365addasset.png)

2.  <span data-ttu-id="d44ca-149">Filtrar en aplicaciones de Office 365 > formación de equipos de Microsoft</span><span class="sxs-lookup"><span data-stu-id="d44ca-149">Filter on Office 365 Apps > Microsoft Teams Training</span></span>
3.  <span data-ttu-id="d44ca-150">Agregar Welcome to Microsoft Teams, obtener su equipo y en funcionamiento e iniciar chats y realizar llamadas.</span><span class="sxs-lookup"><span data-stu-id="d44ca-150">Add Welcome to Microsoft Teams, Get your team up and running, and Start chats and make calls.</span></span>
4.  <span data-ttu-id="d44ca-151">Seleccione el menú botón > crear activos.</span><span class="sxs-lookup"><span data-stu-id="d44ca-151">Select the menu button > Create Asset.</span></span>
5.  <span data-ttu-id="d44ca-152">Tipo de utilizar el cuadro de comando de los equipos en el cuadro Título de activos.</span><span class="sxs-lookup"><span data-stu-id="d44ca-152">Type Use the Teams command box in the Asset title box.</span></span> 
6.  <span data-ttu-id="d44ca-153">Pegue el uso de SharePoint la URL de página del cuadro del comando de los equipos que copió en el campo de contenido activo.</span><span class="sxs-lookup"><span data-stu-id="d44ca-153">Paste the SharePoint Use the Teams command box page URL you copied in the Asset content field.</span></span> 
7.  <span data-ttu-id="d44ca-p107">Navegar a la > de las listas de reproducción personalizadas de página principal > ahora su primer días con los equipos > utilizar el cuadro de comando de los equipos. La página debe tener un aspecto similar al siguiente.</span><span class="sxs-lookup"><span data-stu-id="d44ca-p107">Now navigate back to the Home Page > Custom Playlists > Your first days with Teams > Use the Teams command box. Your page should look like the following.</span></span> 

![página creada](media/clo365createplaylist2.png)

<span data-ttu-id="d44ca-157">La lista de reproducción con este contenido ahora estará disponible en cualquier lugar tiene instalado / incrustado el elemento Web de aprendizaje personalizado.</span><span class="sxs-lookup"><span data-stu-id="d44ca-157">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

#### <a name="things-to-think-about"></a><span data-ttu-id="d44ca-158">Aspectos a tener en cuenta</span><span class="sxs-lookup"><span data-stu-id="d44ca-158">Things to Think About</span></span>

<span data-ttu-id="d44ca-p108">Listas de reproducción personalizadas se pueden usar para ayudar a los usuarios finales en un vareity de tareas.  ¿Dispone de un tiempo desactiva el formulario de solicitud?  ¿Un formulario para solicitar equipamiento de hardware?  Los activos de aprendizaje existentes se pueden programar en la experiencia.</span><span class="sxs-lookup"><span data-stu-id="d44ca-p108">Custom playlists can be used to assist your end users in a vareity of tasks.  Do you have a time off request form?  A form to request hardware equipment?  Any existing training assets can be programmed into the experience.</span></span>  
