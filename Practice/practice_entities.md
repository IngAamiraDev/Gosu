# Práctica Entidades PCF's

## Directorio Extensions
- Es el que contiene todas las entidades modificables de la plataforma
- Es modificable
- Contiene las entidades modificables
- Siempre que se hable de extensión estamos modicando el comportamiento o añadiendo información a las entidades
- Entidades `.eti` => Tipos de entidades de información, son las más comunes
- Entidades `.etx` => Entidades de extensión, resultado de una que se amplió el comportamiento
- Typelist `.ttx` => Typelist que han extendido su compartamiento
- Typelist `.tti` => Typelist de información, normalente son los que se crean inicialmente
- Typelist `.tix` => Typelist internos de extensión

## Directorio Metadata
- Es el que contiene todas las entidades lectura/edición de la plataforma
- No se puede modificar
- Contiene entidades propias del Core de la plataforma

## Criterios a tener en cuenta al crear una nueva Entidad
Extension>Entity>New Entity

Entity:
- Las entidades nuevas se deben nombrar con el sufijo `_Ext`

Entity Type:
- entity => Crear Entidades por defecto
- subtype => Crear subtipos de una entidad padre
- viewEntity => Crear vistas de una entidad. Se crea a partir de otra entidad, se puede filtrar campos. Las vistas no son persistibles
- nonPersistentEntity => Son temporales, no se persisten en BD. Los datos se mantienen en memoria, solo se mantienen en tiempo de ejecución y se eliminan al reiniciar
- delegate => Definir una interface y la clase que implementa los métodos de esa interface

Esc:
- Descripción en caso de ser necesario

Table:
- Nombre de la tabla que se va a represantar en la BD

Type:
- No todos se deben usar
- Algunos son de uso general
- Otros, en cambio, son de uso interno de la plataforma
- Solo usar los tipos:
    - Editable    => Permite almacenar la versión de una entidad
    - Versionable => Permite que la entidad mantenga un Id para versionar los cambios
    - Retireable  => Permite mantener todo los registros en BD. En caso de eliminar un registro lo hace a nivel lógico, manteniendolo en BD. Es el más usado

SubType (Atributos):
- Extendable => Nos indica que si se marca como "false" no se puede modificar. (Viene por defecto "true")
- Exportable => Es un atributo deprecado
- Final      => No se puede hacer subtipos de esta entidad

## Ejemplo PCF
![NewVehicle](/Practice/imgs/newVehicle.png)

## Ejemplo dle render en el front
![View Front](/Practice/imgs/viewFront.png)

## Gosu Scratchpad
![Gosu Scratchpad](/Practice/imgs/gosuScratchpad.png)