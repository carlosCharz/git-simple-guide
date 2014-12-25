GIT - Una simple guía
================

Una simple guía para comenzar a entender los comandos más conocidos de GIT. Porque la memoria muchas veces me falla y solo necesito una revisión rápida.

Basado en [# just a simple guide for getting started with git. no deep shit ;)](http://rogerdudler.github.io/git-guide/)

##### Nuevo repositorio

```git
git init
```

##### Crear un archivo

```git
touch README.md
```

##### Checkout un repositorio

```git
git clone /ruta/al/repositorio
git clone usuario@host://ruta/al/repositorio
```


##### Add

```git
git add <filename>
git add *
```

##### Commit

```git
git commit -m "Mensaje del commit"
```

##### Push

```git
git remote add origin https://ruta/al/repositorio
git push -u origin master //También puede apuntar a un branch, se reemplaza master por el nombre del branch
```
* Ej: git remote add origin https://github.com/carlosCharz/git-simple-guide.git


##### Branch

```git
git checkout -b branch_name  //Para crear un branch
git checkout master  //Para hacer un switch al master
git branch -d branch_name  //Para eliminar un branch
git push origin branch_name  //Para hacer push de nuestros cambios al branch
```

##### Pull (Actualizar)

```git
git pull
```


##### Pull (Actualizar)

```git
git pull
```


##### Merge

```git
git merge branch_name  //Puede ser el master también
```


##### Conflictos en Merge

```git
git add file_name  //Para agregar manualmente los archivos
git diff <source_branch> <target_branch>  //Para previsualizar los cambios
```


##### Tagging

```git
git tag 1.0.0 162e1d63ff  //Normalmente se coloca los primeros 10 caracteres del primer commit
```


##### Log (Historia del Repositorio)

```git
git log
git log --author=carlos
git log --pretty=oneline
git log --name-status  //Para ver los archivos que cambiaron
git log --help
```


##### Reemplazar cambios locales

```git
git checkout <commit>
git checkout <commit> <filename>
git checkout --<filename>
```


##### Reemplazar todos los cambios locales (commits)

```git
git fetch origin
git reset --hard origin/master
```


##### Revert (genera un nuevo commit que deshace todos los cambios introducidos en un commit)

```git
git revert commit
```


##### Reset (Deshacer cambios de manera permanente) NO HACER RESET DE LA HISTORIA PUBLICA

```git
git reset HEAD
git reset --hard HEAD~2
git reset --hard
```


##### Clean

```git
git clean -n  //Dry run
git clean -f  //Force
```


##### Useful hints

```git
gitk //Para usar gui
git config color.ui true
git config format.pretty oneline
git add -i  //Para hacer un adding interactivo
git config --global user.name <nombre>
git config --gloobal user.email <email>
git status
```
