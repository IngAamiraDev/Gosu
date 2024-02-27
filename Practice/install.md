# Pasos para la instalación:

Se recomienda usar [7-zip](https://www.7-zip.org/download.html) para descomprimir las carpetas Descargar

1. Descargar y descomprimir `Apache-ant` en C:\
2. Descargar y descomprimir `jdk-1.7.0_80` en C:\apps\java
3. Crear las variables de entorno para el Java y el ANT: 
    - Nombre de la variable: JAVA_HOME
        - Valor de la variable: C:\apps\java\jdk-1.7.0_80
    - Nombre de la variable: ANT_HOME
        - Valor de la variable: C:\apache-ant-1.8.2
4. Añadir al Path, deberan quedar de la siguiente manera al inicio del valor de la variable:
    %JAVA_HOME%\bin;%ANT_HOME%\bin
5. Descargar y descomprimir el `IDE de Guidewire` y descomprimir en la carpeta C:\Guidewire
6. Descargar y descomprimir `u01` en C:\
7. Lanzar el estudio desde una consola de windows en C:\Guidewire\ContactManagerTrainingApp\bin con el comando gwXX studio 
    (Reemplazar `xx` por `ta` para Training, `cc` para ClaimsCenter, `pc` para PolicyCenter, `bc` para BillingCenter y `ab` para ContactManager)
8. Realizar la configuración básica si es necesario, representada en las fotos de recursos.
9. Correr el servidor
10. Lanzar la app desde el navegador con la siguiente ruta: http://localhost:8280/ab/ContactManager.do
    usr: su 
    pwd: gw