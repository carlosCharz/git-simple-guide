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
