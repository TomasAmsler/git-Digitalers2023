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
