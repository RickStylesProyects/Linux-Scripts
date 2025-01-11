# Script-en-Bash-de-un-Menu

## Resumen

Hemos desarrollado un script en Bash que proporciona un menú interactivo para realizar varias tareas como listar usuarios y grupos, mostrar terminales activas, y obtener información detallada sobre usuarios específicos. Además, valida la existencia de usuarios y grupos para asegurar la precisión de las operaciones. Esta documentación detalla el código y los pasos necesarios para ejecutar y comprender el script.

## Introducción

El propósito de esta práctica es familiarizarse con la creación de scripts en Bash y el uso de comandos del sistema para gestionar usuarios y grupos a travez de un menú interactivo.

## Objetivos

### Objetivo General
Desarrollar un script en Bash que proporcione un menú interactivo para realizar tareas administrativas en el sistema operativo Linux.

### Objetivos Específicos
- Listar los usuarios existentes en el sistema.
- Listar todos los grupos existentes en el sistema.
- Listar las terminales disponibles en el sistema.
- Validar la existencia de usuarios y grupos.
- Mostrar información detallada sobre usuarios específicos.
##Desarrollo
###Shebang
#!/bin/bash
Esta linea es un shebang y se encarga de indicar al sistema que el script debe ser ejecutado usando un interprete de bash.

###Bucle Principal
while :
do
    clear
    echo "==================================================================================="
    echo "                                     * Menú*                                       "
    echo "==================================================================================="
    echo "1. Listar los usuarios existentes en el sistema"
    echo "2. Listar todos los grupos existen en el sistema"
    echo "3. Listar las terminales disponibles en el sistema"
    echo "4. Elija un usuario o ingrese el nombre de usuario y muestre a qué grupos pertenece"
    echo "5. Elija un grupo o ingrese el nombre de grupo y muestre los usuarios pertenecientes"
    echo "6. Mostrar toda la información disponible respecto a un usuario"
    echo "7. Salir"
    echo "========================="
    echo -n "Elige una opción [1-7]: "

    read opcion

while : inicial un bucle infinito con su comando : siempre retorna verdadero hasta que encuentre un break o exit.
clear limpiar la pantalla al inicio de cada bucle esto evitara que tengamos una terminal llena siempre
echo se encarga imprimir el menu en pantalla con las opciones disponibles.
read opcion aqui se lee una entrada del usurio y la almacena en la variable opcion.

Vamos a crear una funcion para verificar la existencia de un usuario en especifico.
