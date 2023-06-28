  # Clase 06 - Git Intro

## Configuracion inicial.
''' sh
git config --global user.name "Tomas Amsler"
git config --global user.email "amslertomas@hotmail.com"

## Verificando la configuracion inicial:

'''sh
git config --get-regexp user
'''

## Inicializando un repositorio de GIT (Creando de GIT)

'''sh
git init
'''
## Areas del repositorio

3 Areas:

* Working Directory (WD): Directorio de trabajo donde se van agregando o quitando archivos durante el desarrollo.
* Area de control de cambios (Staging Area (SA)): Area de control de cambios. Area temporal/intermedia (separa los archivos y despues guardarlos).
* Locar Repo (LR): Una caja donde voy guardando las fotos que vaya sacando.

## Estado de los archivos

* untracked: (Archivos que no tienen seguimiento) estan en el working directory pero GIT no le da seguimiento todavía.
* unmodified: Archivo que GIT ya esta siguiendo y con respecto al WD, no fueron modificados.
* modiefied: Archivos que se encuentran en el repositorio (seguidos por GIT) pero difieren con lo que se encuentra en el area de trabajo (WD).
* stateg: Archivos que estan en el area temporal/intermedia.

## ¿Como chequeo en que area estan los archivos?

'''sh
git status
'''
¡IMPORTANTE! TENGO LA CARPETA EN ESTE CASO, TENIA QUE PONER GIT/README.md 

'''sh
git commit -m "agrego el readme"
'''
con ese comando agrego la modificacion.

## Para confirmar los cambios de un archivo (WD => SA)

'''sh
git add <nombre-archivo>
fit add README.md
gid add README.md css/estilos.css
git add . # Con el punto (.) o el asterisco (*) agrego todos los archivos que estan (UnTRACKED, MODIFIED) al area intermedia o stanging area (SA)
'''

## Para hacer un commit [Sacar foto] (SA => LR)

'''sh
git commit -m "Mensaje explicando que guarde en esa foto"
git commit -m "Agrego el readme.md"
'''

## Para ver los commits que estan dentro el repositorio locar (Local REPO)

'''sh
git log
git log --oneline
'''

'''sh
git diff sirve para ver los cambios que hice en el archivo.
Con la tecla "Q" hace que salga de ver las modificaciones.
Por ejemplo en este caso seria el readme que yo guarde en el local repo.
'''

## Si quiero ver los cambios entre el WD y LR

'''sh
git diff
NOT: si se me bloquea la consola. Tengo que apretar la tecla q (quit).
'''

'''sh
git restore (lo que se haya borrado, ejemplo index.html)
para poder restaurar cualquier archivo eliminado

'''