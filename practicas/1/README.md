# Práctica 1: Introducción a Git y GitHub
````
Entrega: 25/03/2019
````
El objetivo de esta práctica es comprender el flujo de desarrollo utilizando Git y GitHub. 

## Cuenta de usuario
Si aún no tienes una cuenta de usuario accede a https://github.com para crearla.

## Ambiente de trabajo
El repositorio oficial del curso es https://github.com/Miguelp-rez/Linux y para poder agregar sus entregas deberán crear una copia de este en su espacio personal (un fork).  

## ¿Cómo utilizar un fork?
Comunmente, los forks se utilizan para proponer cambios al proyecto de alguien más o como punto inicial para desarrollar una nueva idea.

Cuando alguien desea solucionar un error del proyecto de alguien más, usualmente realiza los siguientes pasos:
1. Hacer fork al repositorio
2. Corregir el error
3. Hacer un pull request al desarrollador del proyecto
Si el desarrollador del proyecto está de acuerdo con la solución propuesta, podría incluirla en el repositorio original.

En este curso se seguirá un esquema similar para agregar las entregas:
1. Hacer fork al repositorio
2. Realizar la tarea
3. Hacer un pull request

## ¿Cómo realizar un fork?
Acceder al repositorio oficial y dar click en el botón "Fork", ubicado arriba a la derecha. Con esto tendrán una copia 'remota' del repositorio en su cuenta de GitHub, el siguiente paso es hacer una copia 'local' en sus computadoras.
En la copia creada presionar el botón verde "Clone or download" y copiar la URL.
Las instrucciones a partir de este punto asumen que se tiene git instalado y que se estáa utilizando una interfaz de línea de comandos. Existen interfaces gráficas y son libres de usarlas si así lo desean.
1. Abre una terminal
2. Dírigite al directorio donde se almacenará la copia
2. Escribe 'git clone' y pega la URL copiada anteriormente. Se verá similar a esto, sustituyendo USERNAME por tu nombre de usuario
```
git clone https://github.com/USERNAME/Linux.git
```
3. Presiona enter para crear tu copia local

## Actividad
Dirigirse al directorio "practicas/1"
```
cd practicas/1
```
Crear una carpeta con el siguiente formato \[ApellidoPaternoNombre\]. Ejemplo: 
```
mkdir EscutiaJuan
```
Nota: sustituyan Escutia por su apellido paterno y Juan por su nombre
Dirigirse al directorio creado
```
cd EscutiaJuan
```
Crear un archivo llamado "Prueba.txt" y escriban en él su nombre completo seguido de su nombre de usuario.
Cuando hayan terminado agreguen sus cambios a git.
```
git add *
```
Confirmen sus cambios
```
git commit -m "Inserte un comentario"
```
Suban sus cambios a su repositorio
```
git push
```

## Pull request
Un pull request es una petición para que el desarrollador del proyecto original acepte tus cambios. Para entregar la práctica o cualquier otra actividad deberán acceder su repositorio en GitHub y dar click en el botón "New pull request". Se mostrarán las diferencias entre el repositorio oficial y su copia. Si les parece correcto, seleccionar el botón verde "Create pull request".

Describe los cambios que hiciste, confirma tu mensaje y GitHub te mostrará que la solicitud ha sido creada.

## Sincronización con el repositorio original
Cuando se hace fork de un proyecto, se puede configurar Git para trear cambios del repositorio original.
```
git remote add --track master Miguelp-rez git://github.com/Miguelp-rez/Linux
```
Esto significa, agrega una fuente remota en la dirección mencionada, siguiendo la rama master, y dale localmente el nombre Miguelp-rez.

Ejecutar la siguiente instrucción para traer cambios del repositorio original. Es recomendable realizar esta acción antes de empezar a trabajar en la copia local.
```
git pull Miguelp-rez master
```






