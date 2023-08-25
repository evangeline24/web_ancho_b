# web_ancho_banda
ASSR PROYECTO

Diagrama de la Base de Datos:

Tabla devices

Campos: id(int), name(varchar), ip_address(varchar), created_at(marca de tiempo)
id: Clave primaria autoincremental (int) que identifica de manera única un dispositivo.
name: El nombre del dispositivo (varchar).
ip_address: La dirección IP del dispositivo (varchar).
created_at: La marca de tiempo cuando se creó el registro (timestamp).

Tabla bandwidth_usage

Campos: id(int), device_id(int), bandwidth_usage(decimal), timestamp(marca de tiempo)
id: Clave primaria autoincremental (int) que identifica de manera única un registro de uso de ancho de banda.
device_id: Clave foránea (int) que se relaciona con el idde la tabla devices.
bandwidth_usage: El valor de uso de ancho de banda (decimal).
timestamp: La marca de tiempo cuando se registró el uso de ancho de banda (timestamp).

[![APP-WEB-ANCHO-DE-BANDA.png](https://i.postimg.cc/vmbfRY8p/APP-WEB-ANCHO-DE-BANDA.png)](https://postimg.cc/qNDzyd3L)

METODOLOGÍA

Paso 1: Configuración del Proyecto

Crea una carpeta para el proyecto y abrir una terminal en esa ubicación.
Inicializar un proyecto Node.js ejecutando npm init. 
Instale las dependencias necesarias:

expresspara crear el servidor.

socket.iopara la comunicación en tiempo real.

mongoosepara interactuar con MongoDB.

Otras bibliotecas según tus necesidades (por ejemplo, para gráficos o estilos).

Paso 2: Configuración del Servidor

Crea un archivo server.jspara tu servidor.
Configura Express y crea el servidor HTTP.
Configura Socket.io para comunicación en tiempo real.

Paso 3: Configuración de MongoDB

Configure la conexión a su base de datos MongoDB server.jsutilizando mongoose.
Define los esquemas y modelos necesarios para tus datos (por ejemplo, dispositivos y uso de ancho de banda).

Paso 4: Lógica de Monitoreo y Comunicación en Tiempo Real

Implementa la lógica para recopilar los datos de uso de ancho de banda y almacenarlos en la base de datos.
Utiliza WebSockets con Socket.io para enviar los datos de uso de ancho de banda a los clientes conectados en tiempo real.
Paso 5: Interfaz de Usuario

Crea las páginas HTML, CSS y JavaScript para tu interfaz de usuario.
Utilice JavaScript para establecer una conexión WebSocket con el servidor y recibir actualizaciones en tiempo real.
Paso 6: Despliegue

Despliega tu aplicación en un servidor en la nube o en tu propio servidor local.
Asegúrese de configurar MongoDB y otras dependencias en el entorno de producción.
