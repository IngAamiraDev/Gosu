# Taller Práctico - Creación y Exposición de Servicios Soap

## Temarios
- Lista de notas
- Campos obligatorios
- Propiedad implementsEntity
- Permisos(Usuarios y seguridad)
- Consumo externo, creación y exposición de servicios Soap

## Reglas de validación
![Reglas Validación](/Practice/imgs/reglas_validacion.png)

## Permisos(Usuarios y seguridad)
- Se debe configurar roles para configurar los permisos de cada usuario
- canEdit  => perm.System.(tipo_permiso)
- canVisit => perm.System.(tipo_permiso)

## Servicios Web SOAP
Configuration>gsrc>sura

- Crear el nombre del paquete
- Dentro del paquete crear el Webservice Collection => Permte configurar los recursos para el uso de servicios externos

### Consumir Servicio Web
![Consumir Servicio Web](/Practice/imgs/consumir_servicio_web.png)


### Exponer Servicio Web
![Exponer Servicio Web](/Practice/imgs/exponer_servicio_web.png)

Anotaciones:
- `@WsiWebService`   => Para exponer el servicios web
- `@WsiPermissions`  => Para configurar los tipos de permisos
- `@WsiAvailability` => Para mantener la disponibilidad del servicio (MAINTENANCE)