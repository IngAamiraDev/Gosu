# Taller Practico - Consumo externo, creación y exposición de servicios JsonRPC Tipo Rest

# Servicios Tipo Rest
- Path: configuration>gsrc>company>ab>edge
- Crear un nuevo paquete para almacenar los métodos
- Crear la clase que contine los métodos a exponer
- Crear paquetes internos para agrupar los DTO (Request y Response)
- Dentro de la clase principal implementar el método `IRpcHandler`
- Etiquetar la clase principal con `@JsonRpcMethod`
- Crear otro paquete para implementar la lógica
    - Definir una interface con la delcaración del método abstracto
    - Crear clase que implemente la interface

Ejemplo Conf Inicial:

![Ejemplo Conf Inicial](/Practice/imgs/paquetes_rest.png)


## Paquete `contact.properties`
- Archivo de localización de los recursos 
- Se puede usa para definir el camino de la clase handler
- Path: configuration>config>portal>capabilities
- Definir el llamado del handler

Ejemplo `contact.properties`:

![Ejemplo contact.properties](/Practice/imgs/paquete_contact_properties.png)