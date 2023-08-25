# web_ancho_banda
ASSR PROYECTO
Diagrama de la Base de Datos:

tablasdevices

Campos: id(int), name(varchar), ip_address(varchar), created_at(marca de tiempo)
id: Clave primaria autoincremental (int) que identifica de manera única un dispositivo.
name: El nombre del dispositivo (varchar).
ip_address: La dirección IP del dispositivo (varchar).
created_at: La marca de tiempo cuando se creó el registro (timestamp).

tablasbandwidth_usage

Campos: id(int), device_id(int), bandwidth_usage(decimal), timestamp(marca de tiempo)
id: Clave primaria autoincremental (int) que identifica de manera única un registro de uso de ancho de banda.
device_id: Clave foránea (int) que se relaciona con el idde la tabla devices.
bandwidth_usage: El valor de uso de ancho de banda (decimal).
timestamp: La marca de tiempo cuando se registró el uso de ancho de banda (timestamp).

[![APP-WEB-ANCHO-DE-BANDA.png](https://i.postimg.cc/vmbfRY8p/APP-WEB-ANCHO-DE-BANDA.png)](https://postimg.cc/qNDzyd3L)


