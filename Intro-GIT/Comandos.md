# GIT

## Intro

- Sistema de control de versiones
- Guarda todos los cambios en un proyecto
- Colaborar con multiples desarrolladores
- Revertir cambios hechos en un proyecto

## Áreas de git

- Working directory -> Directorio actual
- Staging area -> Estado intermedio
- Repository -> Directorio final

- Working directory --> git add --> Staging area
- Staging area --> git commit --> Repository

## Comandos básicos

- git init
- git add \<file>
- git status
- git commit
- git push
- git pull
- git clone

## Añadir todos los archivos al Staging area

- git add .

## Configuración 

- git config --global user.email "contacto@gmail.com"
- git config --global user.name "cele:/"

## Snapshoots

- Un snapshoot es una "foto" actual del proyecto
- Un snapshoot es guardada al realizar un git commit
- Cada snapshoot se guarda con la fecha, el usuario que realiza algun cambios y que cambios se realizaron
- Cada snapshoot tiene además un hash que lo identifica, un numero larguisimo
- \<git log> para ver todos los cambios hechos en el tiempo

## Revertir cambios

- git checkout -- \<nombre-archivo.extension>
- Para cambios generados en el Working Directory
- git diff
- Ver que cambios se realizaron

## Archivo ignorador

- Si creamos un archivo llamado .gitignore
- Escribimos dentro el nombre de alguna carpeta o archivo
- Entonces esta carpeta/archivo sera ignorada por git
- En cada linea del .gitignore debemos escribir el nombre de cada uno de los archivos o carpetas que queremos ignorar

## git branch

- git branch: muestra el nombre de la rama donde estamos trabajando
- Si queremos realizar un gran cambio a nuestro proyecto crearemos una nueva rama
- git branch \<nueva-rama> --> creamos una nueva rama
- git chechout \<nueva-rama> --> usamos para movernos de rama en rama
- Dentro de esta nueva rama podemos crear cualquier cantidad de cambios y realizar snapshoots
- Pero cuando volvamos a la rama principal o la rama anterior todos esos cambios desaparecen

## GITHUB

- Repositorios remotos
- Podemos acceder a nuestros proyectos desde cualquier dispositivo y cualquier persona puede ver los códigos

## Crear un repositorio en github

- Si ya tenes un repositorio creado en tu computadora:
 - Crear un nuevo repositorio sin READ.ME
 - git remote origin \<direccion-del-repositorio-url>
 - git push -u origin \<nombre-rama>

## error remote origin already exist

- git remote rm origin

## READ.ME

- Archivo para leer de que se trata el proyecto
- Es una presentanción del proyecto
- Es de tipo mark-down

## git clone

- git clone \<url-del-codigo-de-un-repositorio-de-github>

## Uniendo dos ramas

- Estando en rama main
- git merge \<nueva-rama>
