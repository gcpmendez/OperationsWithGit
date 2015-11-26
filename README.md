# GIT
```
.
                    _______ __________________
                    (  ____ \\__   __/\__   __/
                    | (    \/   ) (      ) (
                    | |         | |      | |
                    | | ____    | |      | |
                    | | \_  )   | |      | |
                    | (___) |___) (___   | |
                    (_______)\_______/   )_(
                                      Forever!
```

##   Agregando! | Adding!
```
git add .
```

##    Comiteando! | Commiting!

```
git commit -m "text"
```

##    Pusheando! | Pushing!


```
git push origin $actual_branch
```

##   Regresando! | Return!

> Volver a un commit anterior, descartando los cambios
 Return to a previous commit, discarding changes
```
git reset --HARD $SHA1
```


> Deshacer el último commit (sin haber hecho push)
```
git reset --soft HEAD~1
```
> Deshacer el último commit (habiendo hecho ya un push)
```
git revert HEAD
```


##   Eliminando! | Removing!

> Eliminar una rama local
```
git branch -d $branch
```
> Eliminar una rama remota
```
git push origin :$branch
```
> Eliminar las ramas remotas que ya no existan en origin (Ambos comandos hacen lo mismo)
> Ejecutar con --dry-run para ver los cambios que realizará
```
git fetch -p
git remote prune origin
```


##   Obtener! | Obtains!

> Ver y descargar Ramas remotas
```
git remote show origin
```
>  Si hay alguna rama de la cual no tengamos los datos aún
```
git fetch origin
```

> Obtener la rama remota
```
git checkout --track -b $rama origin/$rama
git checkout -t origin/$rama
```

>  mostrar todas las ramas
```
git branch -a
```


> ir a una rama remota
```
git checkout -b baremacion remotes/origin/baremacion
```




##   Trabajando con ramas! | Working with branch! 

> Crear una rama basada en el HEAD
```
git branch $branch# 
```

> Cambiar el nombre de una rama
```
git branch -m $nombre_rama_anterior $nombre_rama_nuevo
```


> Crear una nueva rama basada en el branch $other
```
git checkout -b $new_branch $other
```

## Fuentes
1. [rogerdudler git guide]( http://rogerdudler.github.io/git-guide/ "Guide")
