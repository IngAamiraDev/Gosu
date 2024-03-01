# Taller Practico - Creación cola para la mensajería

## Temario
- Creación cola para la mensajería
- Creación de plugin para enviar y recibir mensajes

## Prerequisitos
- [Erlang](https://www.erlang.org/)
- [Rabbit](https://rabbitmq-website.pages.dev/)

## Conceptos Mensajería

### Mensajería
![Mensajeria](/Practice/imgs/mensajeria.png)

### Indetificación de las tablas de Mansajería
![TablasMansajeria](/Practice/imgs/tablas_mensajeria.png)

### Etapas de la Mensajeria
![EtapasMensajeria](/Practice/imgs/etapas_mensajeria.png)

### Ejemplo Módulo CORE Mensajería
![CoreoMensajeria](/Practice/imgs/core_mensajeria.png)

### Componentes de la Mensajería
![ComponentesMensajeria](/Practice/imgs/componentes_mensajeria.png)

## Archivo Conf Colas de Mensajes
- Path: configuration>config>messaging>messaging-config.xml
- Se define el Id de la cola
- Se definie los diferentes elementos para las configuraciones (Transport, Request, ReplayPlgin)

Ejemplo:

![ConfMensajeria](/Practice/imgs/conf_mensajeria.png)

## Conf Plugin Request Mensajeria
- Path: configuration>config>pluging>registry
- Se encarga de construir el menaje
- Defginir interface `AMQPMessageRequest.gs`

Ejemplo:

![ConfRequestMensajeria](/Practice/imgs/conf_request_mensajeria.png)

## Conf Plugin Transport Mensajeria
- Path: configuration>config>pluging>registry
- Se encarga de poner información del mensaje completo en el Broker. (Transportar el mensaje)
- Implementa la clase `AMQPMessageTransport.gs`

Ejemplo:

![TransportMensajeria](/Practice/imgs/transport_mensajeria.png)

## EvenFired
![EvenFired](/Practice/imgs/even_fired.png)

## InboundMessageProcess
![InboundMessageProcess](/Practice/imgs/inbound_message_process.png)