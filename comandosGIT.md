# Primeros comandos GIT

* git --version --> Observamos la version de GIT que tenemos instalada.
* git help --> Importante ya que nos muestra la ayuda que nos ofece GIT.
* git clone --> Clona un repositorio en un nuevo directorio.
* git init --> Crea un nuevo repositorio y lo inicializa
* git add --> prepara los archivos para subirlos 
* git mv --> Mueve o cambia el nombre de algún archivo o directorio.
* git config --global user.name user.email "Santiago Carrillo" --> Realizar configuración global para agregar nombre
* git config --global -e --> Para observar los cambios con el usuario y correo electronico
* tecla Esc + :wq! Para salir del comando de arriba


## cd 

Siginifica change Directory (Cambio de directorio o carpeta )


## GIT init

Este comando nos permite inicializar mi repositorio 

git config --global init.defaultBranch <Name> --> Esto nos permite hacer la configuracion de manera opcional para que despues de que se inicialice un repositorio este tenga un nombre que le asignemos por defecto

## Git status

Este comando nos va a dar información sobre los commit, sobre la rama donde nos encontramos trabajando y nos muestra que archivos sufieron algún cambio o modificación

## Git add .

nos permite actualizar el estado de los datos nuevos dentro del repositorio

## Git reset .Directorio o carpeta

Esto nos sirve para remover un archivo que no queremos agregar para hacer el commit.

## Git commit -message "nombre que queramos"

El comando git commit captura una instantánea (Como tipo de fotografía) de los cambios preparados en ese momento del proyecto. Las instantáneas confirmadas pueden considerarse como versiones "seguras" de un proyecto: Git no las cambiará nunca a no ser que se lo pidas expresamente.

## Git push 

Este comando nos va a permitir subir todos los cambios realizados a nuestro repositorio de manera de remota.

## Git checkout -- .

Este comando le dice a Git que reconstruya el proyecto a como lo dejamos en el ultimo commit, solo de los archivos que se le esta dando seguimiento por GIT, o sea aquellos que ya hayan tenido su Git add .

## Git branch

Este comando nos va a permitir saber en que rama estamos trabajando



# Hacer dos pasos en 1 (add . + git commit -m "")

Para ejecutar los dos comandos a la vez y ahorrarnos un poco de tiempo al momento de actualizar los cambios utilizamos el comando

**git commit -am "la descripcion que queramos"**


Este comando solo funciona si ya le estamos dando seguimiento a nuestro archivo si este aparece con u de untrack entonces no funcionara, posiblemente si añada todos los archivos con excepción de los archivos que tengan untrack

# Git log

Es una herramienta básica de Git para explorar el historial del repositorio. Este comando se usa cuando necesitas buscar una versión concreta de un proyecto o saber los cambios que se introducirán mediante la fusión en una rama de función.

# Subir varios archivos seleccionados a la vez para un solo commit

Para subir varios archivos de un mismo tipo utlizamos el comando

**git add *.html** En este caso estariamos agregando todos los archivos de tipo html

Si queremos especificar un directorio en especifico del cual querramos agragar archivos a seguimiento lo hacemos de la siguiente manera

**git add js/*.js** En este caso entramos a la carpeta llamada js y agregamos los archivos .js que esten ahí dentro. 



**npm run build-mf**
Generar compilado para subir a producción