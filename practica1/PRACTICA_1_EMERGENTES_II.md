1.  **Explique que son los sistemas empresariales**

> Son sistemas que son muy importantes dentro de una organización, los cuales se encarga del funcionamiento de las tareas dentro de ella, como el gestionamiento de datos, organización de documentación entre otros, el cual el mal funcionamiento podría causar perdidas irremediables para tal.

2.  **Describa cuales son las características más importantes de una aplicación empresarial**

> Entre las mas resaltantes se puede tener:

-   Acceso a base datos

-   Operaciones transaccionales, mejor manejo de base de datos en varios estados.

-   Son sistemas escalables, pueden crecer mediante actualizaciones.

-   Disponibles, se puede acceder en cualquier parte y hora (24/7).

-   Seguras, entre ellas la perimetral, cuentas de administrador.

-   Integración, se puede relacionar con varios sistemas con facilidad.

-   Arquitectura multicapa, división clara de responsabilidades, logra un sistema más mantenible y extensible.

3.  **Investigue y proponga cinco (5) instituciones que requerirían aplicaciones de misión crítica. Justifique su respuesta.**

-   ***Impuestos Nacionales,*** se requiere la disponibilidad para la consulta y pago por bancas online, para una mejor organización.

-   ***Aduana Nacional,*** para el control y gestión de mercadería.

-   ***Aseguradoras de vida (Previsión, futuro, etc.),*** ya que en cualquier momento uno desea sacar algún documento que concierne a tramites personales.

-   ***Hospitales (Privadas y Públicas),*** son necesarias para poder consultar los médicos de turno, para todo tipo de emergencia.

-   ***Tránsito,*** es necesario para el acceso a la base de datos, generación de boletas, y pagos en línea.

4.  **Explique cuáles son las diferencias entre la escalabilidad horizontal y escalabilidad vertical.**

> La diferencia entre la escalabilidad son que la horizontal se refiere al aumento de equipos, o servidores. Mientras que la vertical se refiere al aumento de componentes a los equipos.

5.  **Que es un servidor Web y que es un servidor de aplicaciones**

> Se refiere que es un servicio para despachar o mostrar las paginas web a los usuarios, mientras que los servidores de aplicaciones dan un servicio a las computadoras personas de los clientes.

6.  ![](Z:\Escritorio\imagenes\web.jpg){width="7.802169728783902in" height="4.220779746281715in"}**Con un gráfico explique cómo funciona el protocolo HTTP**

7.  **Explique los elementos importantes de REQUEST en HTTP**

-   HTTP method (the action to be performed), Dentro del mensaje "PETICIONES", existen varios métodos que envia y recibe parámetros o variables.

-   The page to access( a url), Se puede acceder desde una URL propuesta por el host o el administrador de la pagina WEB.

-   Form parameters(like arguments to a method), Se puede mandar parámetros, mediante formularios, para ser procesados por los mismos métodos que se declaran.

8.  **Explique los elementos importantes de RESPONSE en HTTP**

-   A status code (for whether the request was successfull), se puede ver si la solicitud de la petición fue realizada con éxito.

-   Content type (text, picture, HTML, etc), Puede dar como respuesta Texto, Imagen, Archivos HTML, etc.

-   The content (the actual HTML, image,etc), su contenido son archivos multimedia que puede ser observado por el cliente o usuario.

9.  **Describa con un gráfico la arquitectura Java EE**

> ![](Z:\Escritorio\imagenes\javaee.jpg){width="5.565324803149606in" height="3.727273622047244in"}

10. **Explique cuáles son los contenedores, componentes y servicios de Java EE**

-   Los contenedores hacen referencia a las plataformas que contienen los componentes web, los tipos de contenedores son:

    -   Contenedor Web.

    -   Contenedor de negocio.

-   Los componentes, son unidades autónomas de software que forman parte de las aplicaciones java EE, se dividen en tipos, como:

    -   Componente cliente:

        -   Cliente AWT.

        -   Swing.

        -   Applet.

        -   Navegador Web.

    -   Componentes Web:

        -   Servlet

        -   JSP y JSF.

    -   Componente de negocio:

        -   EJB.

-   Los servicios, son aquellos que esta conjuntamente con los contenedores de Java EE, existen los siguientes servicios:

    -   De directorio, para la indexación y búsqueda de componentes, recursos.

    -   De despliegue, para personalizar los componentes y recursos.

    -   De transaccionalidad, ejecutar varias acciones en una misma unidad de transaccionalidad.

    -   De seguridad, autentificar y autorizar a los usuarios de la aplicación.

    -   De acceso a datos, facilita el ingreso a la Base de Datos.

    -   De conectividad, fácil acceso a los distintos EIS.

    -   De mensajería, para la fácil comunicación entre los componentes, aplicaciones o EIS.

> Un entorno de ejecución debe implementar y soportar:

-   Todos los tipos de componentes.

-   Todos los tipos de contenedores.

-   Todos los servicios

11. **Investigue los métodos más utilizados de las clases [HttpServlet]{.underline}, [HttpServletRequest]{.underline} y [HttpServletResponse]{.underline}, y para cada uno de los métodos muestre un ejemplo.**

-   Métodos de HttpServlet:

    -   HTTP GET

        -   Limitación: Cuantos datos son pasados como parte del URL → Uso de HTTP POST.

        -   Ejemplo.

![](Z:\Escritorio\imagenes\httpget.png){width="5.174324146981627in" height="1.6233770778652667in"}

-   HTTP POST

    -   Permite al cliente enviar datos al servidor

        -   Pasar más información que una petición HTTP GET

    -   ![](Z:\Escritorio\imagenes\httppost.png){width="4.565216535433071in" height="1.8629024496937883in"}Ejemplo.

-   doGet() y doPost()

    -   Sobre escribir métodos doGet() y doPost().

![](Z:\Escritorio\imagenes\do.png){width="5.233766404199475in" height="1.874329615048119in"}

-   Metodos de HttpServletRequest

    -   **HttpServletRequest.getHeader()**

        -   Método que recupera el contenido de la cabecera HTTP cuyo nombre coincida con el pasado por parámetro.

        -   Ejemplo.

> String sIP = request.getHeader(\"X-FORWARDED-FOR\");

-   **HttpServletRequest.getSession()**

    -   Método que nos devuelve una referencia a la sesión HttpSession asociada a la petición actual.

> protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {
>
> HttpSession session = request.getSession();
>
> session.setMaxInactiveInterval(20\*60);
>
> }

-   Otros métodos:

    -   **HttpServletRequest.getAuthType()**

    -   **HttpServletRequest.getContextPath()**

    -   **HttpServletRequest.getCookies()**

    -   **HttpServletRequest.getDateHeader()**

    -   **HttpServletRequest.getHeaderNames()**

    -   **HttpServletRequest.getHeaders()**

    -   **HttpServletRequest.getIntHeader()**

    -   **HttpServletRequest.getMethod()**

    -   **HttpServletRequest.getPathInfo()**

    -   **HttpServletRequest.getPathTranslated()**

    -   **HttpServletRequest.getQueryString()**

    -   **HttpServletRequest.getRemoteUser()**

    -   **HttpServletRequest.getRequestedSessionId()**

    -   **HttpServletRequest.getRequestURI()**

    -   **HttpServletRequest.getRequestURL()**

    -   **HttpServletRequest.getServletPath()**

    -   **HttpServletRequest.getUserPrincipal()**

    -   **HttpServletRequest.isRequestedSessionIdFromCookie()**

    -   **HttpServletRequest.isRequestedSessionIdFromUrl()**

    -   **HttpServletRequest.isRequestedSessionIdFromURL()**

    -   **HttpServletRequest.isRequestedSessionIdValid()**

    -   **HttpServletRequest.isUserInRole()**

<!-- -->

-   Métodos de HttpServletResponse

    -   Interface que extiende la interface ServletResponse para proporcionar la funcionalidad de respuesta HTTP.

    -   **HttpServletResponse.sendRedirect()**

        -   se puede utilizar para redirigir la respuesta a otro recurso, puede ser un archivo servlet, jsp o html.

        -   **Ejemplo**

> \<%
>
> response.sendRedirect(\"[[http://www.lineadecodigo.com/]{.underline}](http://www.lineadecodigo.com/)\");
>
> \%\>

-   **Otros métodos:**

    -   **HttpServletResponse.addCookie()**

    -   **HttpServletResponse.addHeader()**

    -   **HttpServletResponse.addIntHeader()**

    -   **HttpServletResponse.containsHeader()**

    -   **HttpServletResponse.encodeRedirectURL()**

    -   **HttpServletResponse.encodeURL()**

    -   **HttpServletResponse.sendError()**

    -   **HttpServletResponse.setDateHeader()**

    -   **HttpServletResponse.setHeader()**

    -   **HttpServletResponse.setIntHeader()**

    -   **HttpServletResponse.setStatus()**
