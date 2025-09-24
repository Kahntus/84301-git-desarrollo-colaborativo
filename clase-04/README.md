# Clase 04 - Git desarrollo colaborativo

## Git Stash

* Existe dentro de git
* No se puede subir al remoot
* Trabaja con una estructura de pila
![fifo-lifo] (_ref/image.png)

## Listar los stashes
´´´´sh
git stash list
´´´´

## Creando un stash

´´´´´sh
git stash -m "mensaje descriptivo"
´´´´

## Ver contenido del stash

´´´´sh
git stash show <identificador del stash>
git stash show 0
git stash show stash{0}
´´´´

## Recuperar el stash

´´´´sh
git stash pop # Recuperar el último stash realizado y si no hay conflicto lo borra.
´´´´

## Aplicar un stash en particular

´´´´sh
git stash aplly 1 # stash@{1}
git stash aplly 2 # stash@{2}
´´´´

## Eliminar un stash en particular

´´´´´sh
git stash drop # Borra el stash de arriba de todo
git stash drop 1 # stash@{1}
git stash drop 1 # stash@{2}


# Git resets
Me permite deshacer commmits. Hay 3 tipos

## GIT RESET SOFT
Me permite deshacer uno o varios commits y los cambios lo arroja al staging area (SA)

´´´´sh
git reset --soft <hash>
´´´´

## GIT RESET MIXED (default)
Me permite deshacer uno o varios commits y los cambios los arroja al working directory (WD)

´´´´´sh
git reset <hash>
git reset --mixed <hash>
´´´´

## GIT RESET HARD
Me permite deshacer uno o varios commits y los cambios los descarta (CUIDADO PIERDO LOS CAMBIOS SOBRE LOS ARCHIVOS)

´´´´sh
git reset --hard <hash>
´´´´