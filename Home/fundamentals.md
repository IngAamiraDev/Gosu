# GOSU FUNDAMENTALS

## Tabla de Contenido

1. [GOSU FUNDAMENTALS](#gosu-fundamentals)
   - [GUIDEWIRE](#guidewire)
   - [Guidewire InsuranceSuite](#guidewire-insurancesuite)
     - [PolicyCenter](#policycenter)
     - [ClaimCenter](#claimcenter)
     - [BillingCenter](#billingcenter)
     - [InsuranceSuite](#insurancesuite)
   - [ARQUITECTURA](#arquitectura)
   - [MODELO DE DATOS](#modelo-de-datos)
   - [ENTIDADES](#entidades)
   - [SUBTIPOS](#subtipos)
   - [TYPELIST](#typelist)
   - [LENGUAJE GOSU](#lenguaje-gosu)
     - [Diferencias entre Gosu y Java](#diferencias-entre-gosu-y-java)
     - [Declaración de funciones y variables](#declaración-de-funciones-y-variables)
     - [Diferencias en los flujos de control](#diferencias-en-los-flujos-de-control)
     - [Características propias del Lenguaje](#características-propias-del-lenguaje)
   - [ENHANCEMENT](#enhancement)
     - [Ejemplo Enhancement](#ejemplo-enhancement)
   - [REGLAS DE NEGOCIO](#reglas-de-negocio)
     - [Ejemplos Reglas de Negocio](#ejemplos-reglas-de-negocio)
   - [GOSU QUERIES](#gosu-queries)
     - [Ejemplo Gosu Queries](#ejemplo-gosu-queries)
   - [INTERFAZ GRÁFICA DE USUARIO](#interfaz-gráfica-de-usuario)
     - [Jerarquía de Elementos PCF](#jerarquía-de-elementos-pcf)
     - [Ejemplos de Elementos PCF](#ejemplos-de-elementos-pcf)
     - [Reutilizar Contenedores](#reutilizar-contenedores)
   - [ENTITY NAMES](#entity-names)
   - [GLOBALIZACIÓN](#globalización)
     - [Internacionalización](#internacionalización)
   - [SEGURIDAD](#seguridad)
   - [SCRIPT PARAMETERS](#script-parameters)
   - [INTEGRACIONES](#integraciones)
     - [Puntos de Integración](#puntos-de-integración)
     - [Puntos de Integración por Plataforma](#puntos-de-integración-por-plataforma)
     - [Tecnologías de Integración](#tecnologías-de-integración)
     - [Mecanismos de Integración](#mecanismos-de-integración)
2. [RECURSOS ADICIONALES](#recursos-adicionales)


## GUIDEWIRE
Guidewire es una empresa de tecnología líder en el sector de seguros que ofrece soluciones de software para compañías de seguros de propiedad y accidentes. Fundada en 2001 y con sede en San Mateo, California, Guidewire proporciona una plataforma integral conocida como Guidewire InsurancePlatform, que consta de varios productos diseñados para ayudar a las aseguradoras a gestionar todas las facetas de su negocio.

La plataforma Guidewire InsurancePlatform abarca áreas clave como la suscripción de pólizas, la gestión de reclamaciones, la facturación y la gestión de seguros. Sus productos principales incluyen PolicyCenter, ClaimCenter y BillingCenter, que están diseñados para facilitar la emisión y administración de pólizas, la gestión de reclamaciones y el proceso de facturación, respectivamente. Estos productos están integrados para proporcionar a las aseguradoras una solución completa y coherente para gestionar sus operaciones.

Guidewire se ha convertido en un socio confiable para numerosas aseguradoras en todo el mundo, brindando soluciones innovadoras que les permiten adaptarse a un mercado en constante cambio y ofrecer un servicio excepcional a sus clientes. Además de sus productos principales, Guidewire también ofrece servicios de consultoría y soporte para ayudar a las aseguradoras a implementar y optimizar sus soluciones de software.

### Guidewire InsuranceSuite

#### PolicyCenter
- **Descripción:** 
    - Emitir, modificar y mantener información de las condiciones de las pólizas en todo el ciclo de vida.
    - Compatible con todo el ciclo de vida de la póliza.
- **Procesos Principales:**
    - Subscripción
    - Validación
    - Cotización
    - Emisión
    - Mantenimiento
    - Cambios
    - Renovación

#### ClaimCenter
- **Descripción:** 
    - Administrar procesos de reclamaciones frente a una póliza.
    - Compatible con el ciclo de vida de la reclamación de extremo a extremo.
- **Procesos Principales:**
    - Registro de siniestros
    - Segmentación/Asignación
    - Investigación/Evaluación
    - Reservas/Pagos/Recuperos
    - Litigios/Negociaciones
    - Cierre

#### BillingCenter
- **Descripción:**
    - Emitir y hacer seguimiento al plan de pagos de todos los cargos que genera una póliza.
    - Compatible con todo el ciclo de facturación.
- **Procesos Principales:**
    - Instrucción de facturación
    - Programación
    - Comisiones
    - Cálculos de facturación
    - Servicios al asegurado
    - Pagos
    - Cierre


## ARQUITECTURA
![Arquitectura](/Home/Imgs/arquitectura.png)

## MODELO DE DATOS
![Modelo de Datos](/Home/Imgs/modelo_datos.png)

## ENTIDADES
![Entidades](/Home/Imgs/entidades.png)

- Foreign Key: Relaciones uno a uno
- Array Key: Relaciones uno a muchos
- TypeKey: Relaciones entidad con lista de valores definidos

## SUBTIPOS
![Subtipos](/Home/Imgs/subtipos.png)

- Hereda campos, funciones o propiedades de una entidad padre

## TYPELIST
![Typelist](/Home/Imgs/typelist.png)

- Lista de tipos
- Puede tener campos físicos y virtuales

## LENGUAJE GOSU
![Lenguaje Gosu](/Home/Imgs/lenguaje_gosu.png)

- Creado por Guidewire
- Corre en la máquina virtual de Java
- Orientado a objetos
- Escritura estática
- Se ejecuta secuencial, imperativo
- Expresiones en bloque (lambda)
- Tipos de datos genéricos
- Sistemas de datos extensibles
- Case sensitive
- && (And)
- || (Or)

### Diferencias entre Gosu y Java
![Diferencias](/Home/Imgs/diferencias.png)

### Diferencias operadores lógicos
![Diferencias 2](/Home/Imgs/diferencias_logicos.png)

### Diferencias en los flujos de control
![Diferencias 3](/Home/Imgs/diferencias_flujos.png)

### Declaración de funciones y variables
![Declaraciones](/Home/Imgs/declaraciones.png)

### Características propias del Lenguaje
![Características](/Home/Imgs/caracteristicas_propias.png)

## ENHANCEMENT
![Enhancement](/Home/Imgs/enhancement.png)

- Funciones para mejorar los comportamientos de clases o entidades

### Ejemplo Enhancement
![Ejemplo Enhancement](/Home/Imgs/enhancement.png)

## REGLAS DE NEGOCIO
![Reglas de Negocio](/Home/Imgs/reglas_negocio.png)

- Están presentes en todas las plataformas.
- Las reglas de Negocio no se pueden testear. Se debe migrar a una clase o a un Enhancement para poder testear.
- Tienen una jerarquía, y estas dependen de su ejecución.

### Ejemplos Reglas de Negocio
![Ejemplo Reglas de Negocio](/Home/Imgs/ejm_reglas_negocio.png)

## GOSU QUERIES
![Gosu Queries](/Home/Imgs/gosu_queries.png)

- Permite crear consultas SQL orientadas a objetos
- La construcción de TU es algo complejo, se vuelve tedioso el testeo de queries

### Ejemplo Gosu Queries
![Ejemplo Gosu Queries](/Home/Imgs/ejm_gosu_queries.png)

- No se puede aplicar Right Order Join o Full Order Join

## INTERFAZ GRÁFICA DE USUARIO
![Interfaz de Usuario](/Home/Imgs/interfaz_usuario.png)

- Framework: PCF (Page Configuration File)
- Archivos XML

### Jerarquía de Elementos PCF
![Jerarquía PCF](/Home/Imgs/jerarquia_pcf.png)

- Widget: Renderizan en el navegador html
- Location: Navegar de un elemento a otro. Controlar la navegación dentro de la app

### Ejemplos de Elementos PCF
![Ejemplo PCF](/Home/Imgs/ejm_pcf.png)

![Ejemplo PCF 2](/Home/Imgs/ejm_pcf_2.png)

### Reutilizar Contenedores
![Reutilizar Contenedores](/Home/Imgs/reutilizar_contenedores.png)

## ENTITY NAMES
![Entity Names](/Home/Imgs/entity_names.png)

## GLOBALIZACIÓN

### Internacionalización
![Internacionalización](/Home/Imgs/internacionalizacion.png)

- Cada idioma debe tener claves y valores para cada elemento configurado

## SEGURIDAD
![Seguridad](/Home/Imgs/seguridad.png)

- Los roles son agrupadores de permisos
- Es importante definir con el equipo de negocio el tipo de rol/usuario toda vez que se requiera construir alguna pantalla

## SCRIPT PARAMETERS
![Script Parameters](/Home/Imgs/script_parameters.png)

## INTEGRACIONES
![Integraciones](/Home/Imgs/integraciones.png)

### Puntos de Integración
![Puntos de Integración](/Home/Imgs/puntos_integracion.png)

### Puntos de Integración por Plataforma
![Puntos de Integración por Plataforma](/Home/Imgs/puntos_integracion_plataforma.png)

### Tecnologías de Integración
![Tecnologías de Integración](/Home/Imgs/tecnologias_integracion.png)

- Se utilizan para intercambiar información
- FTP
- Unidades de red
- Bidireccional
- Comunicaciones Síncronas

### Mecanismos de Integración
![Mecanismos de Integración](/Home/Imgs/mecanismos_integracion.png)

- Componentes dentro de la plataforma que permiten hacer uso de la integración

## Recursos Adicionales
- [Capacitación Guidewire](https://iascol.sharepoint.com/sites/CapacitacionGuidewire/SitePages/TrainingHome.aspx?e=4%3A19eb02b624df4c7fba03d0f6b18e00ae&web=1&at=9&cid=62f9cb85-604e-4a28-af48-089885b52eb8)