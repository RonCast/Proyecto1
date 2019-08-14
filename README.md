# Proyecto1
EmergentesII
## Sistemas Empresariales ##
----------------

 1. Explique que son los sistemas empresariales
    

> Un sistema empresarial es un sistema central de la organización, que garantiza que la información que se pueda transmitir a través de todas las funciones empresariales, y todos los niveles de gestión, para soportar la operación y administracion de una empresa.

2.  Describa cuales son las caracteristicas más importantes de una aplicación empresarial.

>  - Es un sistema global, todos sus elementos se relacionan entre si.
Se trata de un sistema autoregulado.
Es un sistema abierto con contacto con su entorno.
Se divide en subsistema 1, subsistema de operaciones 2, subsistema financiero, 3. Subsistema de administracion.

3.  Justifique y proponga cinco (5) instituciones que requeririan aplicaciones de mision critica, Justifique su respuesta.

> 1ra Institucion
    Entidades de desarrollo, Diaconia
    Debe tener una aplicacion de mision critica ya que aparte de manejar bases de datos, cuentas y dinero, debe poseer la seguridad suficiente par evitar la perdida o robo de datos.
    2da Institucion
    Ministerio de Educacion
    Una institucion tan grande requiere una aplicacion de mision critica porque maneja bases de datos extenssas, y necesita responder a consultas de manera rapida y simple,
    3ra Institucion
    Supermercado BigSur
    Esta entidad, realiza cobros por internet, posee tarjetas inteligentes que es un beneficio de descuentos para sus clientes, para ello necesita de una aplicacion de mision critica, para asegurar que los cobros y descuentos sean correctos, y una identificacion de productos rapida.
    4ta Institucion
    Planifica
    Una institucion de Fondos de Inversion, que calcula inversiones y las gestiona mediante software, asi que necesita una aplicacion de misio critica para sus estudios, proyecciones, calculos y el buen manejo de calculo en sus operaciones.
    5ta Institucion
    Gestora publica de la seguridad social a largo plazo.
    Una administradora de Fondos de peciones, que requiere una solida gestion, soportar operaciones basadas en estadisticas y manejo de diner externo.
    
4.  Explique cuales son las diferencias entre escalabilidad horizontal y escalabilidad vertical.

> A pesar de que escalamiento vertical no soporta de forma natural la alta disponibilidad, sí que es posible habilitarla mediante una estrategia llamada Failover, la cual consiste en que cuando el servidor falla, mediante hardware se redireccionan las peticiones a un servidor secundario que es un espejo del principal, este servidor normalmente se encuentra en stand by, y solo se habilita cuando el primario falla, de la misma manera, cuando el primario se recupera, el secundario vuelve a pasar a stand by. En cambio por otra parte, la escalabilidad horizontal ya utiliza de forma natural el Failover, ya que al haber varios nodos, es posible pasar la carga al resto de nodos activos en caso de que uno falle. Ahora bien, esto no garantiza una alta disponibilidad total, ya que si el servidor primario falla puede tumbar todo el cluster, por lo que también se suele utilizar un ambiente espejo del cluster para garantizar la alta disponibilidad. Cabe mencionar que esto solo lo hacen empresas gigantes, ya que administrar dos cluster completos es un verdadero reto. 

5.  Que es un servidor Web y que es un servidor de aplicaciones

>   SERVIDOR WEB
El servidor web responde a solicitudes provenientes de más de una conexión a la vez, pero no puede procesar múltiples solicitudes simultáneas en paralelo. La idea de utilizar subprocesos para mejorar la velocidad de cómputo simplemente no funciona con servidores web

>   SERVIDOR DE APLICACIONES
Los servidores de aplicaciones, por otro lado, admiten subprocesos múltiples junto con varias otras características como la agrupación de aislamiento, la agrupación de conexiones, el equilibrio de carga, la agrupación en clústeres, etc.

 1.  Con un grafico explique como funciona el protocolo HTTP
        ![enter image description here][1]


 2.  Explique los elementos importantes de REQUEST en HTTP
>   Pase en el parámetro contenido el cuerpo (body) de la petición. Los datos pasados en este parámetro dependen del método HTTP de la petición.
Puede enviar datos de tipo texto, BLOB, imagen u objeto. Cuando el content-type no se especifica, se utilizan los siguientes tipos:

    *   para los textos: texto/plano - UTF8
    *   para los BLOBs: aplicación/byte-stream
    *   para las imágenes: tipo MIME conocido (best for Web).
    *   para los objetos C_OBJECT: aplicación/json
    
    
 3.  Explique los elementos importantes de RESPONSE en HTTP
    >   HTTP se basa en un modelo solicitud / respuesta, de modo que hay dos tipos de mensajes HTTP: la solicitud y la respuesta. El navegador abre una conexión a un servidor y realiza una solicitud. El servidor procesa la solicitud del cliente y devuelve una respuesta. La figura siguiente ilustra este proceso.
>   La línea de salida de una petición HTTP se conoce como línea de la petición. Siempre es la primera línea del mensaje de solicitud y contiene tres campos:
• Un método HTTP
• Un identificador universal de recursos (URI)
• Una versión del protocolo HTTP

 4.  Describa con un grafico la arqiuitectura Java EE
    ![enter image description here][2]


  [1]: #file:f53cd7cd-0b8d-bff5-7c73-203990bb5b37
  [2]: #file:03f06479-4313-1fce-10f8-2350110b5e71
  

 5. Explique cuales son los contenedores, componentes y servidores de Java EE
>   Java EE hace que las aplicaciones sean fáciles de escribir porque la lógica de negocio se divide en componentes reutilizables y adicionalmente se cuenta con un servidor de aplicaciones que proporciona servicios en la forma de contenedor para los diferentes tipos de componentes, debido a esto no se tiene que desarrollar estos servicios, sino enfocarse en el desarrollo, es por eso que define los siguientes contenedores.
    1.  Contenedor EJB: Maneja la ejecución de los enterprise beans.
    2.  Contenedor Web: Maneja la ejecución de las paginas web, servlets y algunos componentes ejb para las aplicaciones Java EE.
    3.  Contenedor de aplicación cliente: Maneja la ejecución de la aplicación cliente no necesita un servidor de aplicaciones.
    4.  Contenedor Applet: Maneja la ejecución de applets, no necesita servidor de aplicaciones, consiste en un browser y el plugin web de java.\
>   Los componentes son:
        1.  Las Aplicaciones cliente y los applets hijo Componentes Que se ejecutan en el cliente. Java Servlet, hijo JavaServerFaces y JavaServerPages Componentes Web Que se ejecutan en el Servidor. Enterprise JavaBeans (EJB) hijo Componentes de Negocio Que se ejecutan en el Servidor.
        2.  JAVA EE: Es una colección de especificaciones que definen una infraestructura para desarrollar aplicaciones distribuidas multicapa.
        3.  El servidor y el cliente pueden incluir componentes JavaBeans para administrar el flujo de datos entre una aplicación cliente o un applet y componentes que se ejecutan en el servidor JEE o entre componentes de 
servidor y BD
>   Servidores
    Hasta el 2019 se conocel los siguientes servidores que trabajan con Java EE
    *   Eclipse Glassfish
    *   Oracle Weblogic
    *   IBM Websphere
    *   Red Hat WildFly (JBoss)
    *   Payara
    *   Apache TomEE

11. Investigue los metodos mas utilizados de las clases **HttpServlet, HttpServletRequest y HttpServletResponse**, y para cada uno de los metodos muestre un ejemplo.
       **HttpServlet**
    * public abstract interface Servlet: Todos los servlets implementan este interfaz directamente o extendiendo una clase que lo implemente como HttpServlet. Entre sus métodos están:
    
*   init(ServletConfig config): Es el método utilizado para crear una nueva instancia del servlet (análogo al constructor). Ver el ciclo de vida. Este método puede ser sobreescrito para realizar tareas como crear una conexión a una BD que se mantendrá mientras el servlet se mantenga cargado y puede ser utilizada por cada petición. ServletConfig contiene los parámetros de inicialización que entrega el servidor al servlet.
*   getServletConfig(): Retorna la configuración dada para la inicialización del servlet.
*   service(ServletRequest req, ServletResponse res): Este método es el que se llama cuando se recibe una petición de un cliente y en su implementación normal para HTTP verifica el tipo de solicitud GET, POST, etc. y la redirige a los métodos respectivos. En general no es necesario reimplementar este método.
*   destroy(): Este método es llamado por el servidor para indicar que el servlet será destruido. Es llamado sólo una vez y uno debe encargarse de esperar por posibles peticiones en curso.

**HttpServletRequest**
*   public abstract interface HttpServletRequest extends ServletRequest: Permite obtener del cliente la información que es dependiente del protocolo, en este caso HTTP. Entre sus métodos están:

*   getHeader(String name): Permite obtener el valor de los Headers de HTTP con que fue llamado el servlet.
*   getCookies(): Retorna un arreglo que contiene todas las cookies que el cliente envía al servlet.
*   getSession(): Retorna la sesión en la cual se encuentra el cliente.


**HttpServletResponse**
*   public abstract interface HttpServletResponse extends ServletResponse: Permite enviar al cliente respuestas específicas del protocolo HTTP.

*   addCookie(Cookie cookie): Para definir nuevas cookies en el cliente.
*   setHeader(String name, String value): Para definir un header HTTP a enviar al cliente.
*   sendRedirect(String location): Envía un mensaje al cliente para redireccionar la respuesta a la dirección señalada.
