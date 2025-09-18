# Clase 01 - Git Desarrollador Colaborativo

## Página de git


## Configuración inicial
Esta configuración se hace una sola vez. Y es para indicarle a git con que nombre y correo se van a firmar los commits creados

´´´´sh
git config --global user.name "Eduardo Colque"
git config --global user.mail eduardocolque04@gmail.com
´´´´

## Verificar la configuración del usuario
´´´´ sh
git config --get-regexp user 
´´´´

## Listar configuraciones
´´´´sh
git config --list
´´´´

## Para editar las configuraciones
´´´´sh
git config --global -e
´´´´

## Para crear un repositorio de git
´´´´sh
git init
´´´´

## En el caso de que no haya colocado en la instalación main
´´´´sh
git config --global init-defaultBranch

## Ver loc commits generado (Timeline de commits)
´´´´sh
git log # versión larga
git log --oneline # versión corta
´´´´

