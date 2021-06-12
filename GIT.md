# GIT


## Congifuración Git 

### Tu identidad

Configurar dentro de un proyecto especifico 
```
git config user.email 'eleazar-00@hotmail.com'

git config user.name 'Eleazar Curiel Monjaraz'
```
Configuración de manera Global
```
git config --global user.email 'eleazar-00@hotmail.com'

git config --global user.name 'Eleazar Curiel Monjaraz'
```

### Comprobar configuración

```
git config --list 
```

```
user.name=eleazar.curiel
user.email=eleazar.curiel@famsa.com
core.repositoryformatversion=0
core.filemode=true
core.bare=false
core.logallrefupdates=true
remote.origin.url=https://github.com/IngCuriel/BackEndJava.git
remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
branch.main.remote=origin
branch.main.merge=refs/heads/main
user.email=eleazar-00@hotmail.com
user.name=Eleazar Curiel Monjaraz
```

> Puede que veas claves repetidas ya que git lee la claves de distintos archivos. (/etc/gitconfig y ~/.gitconfig, por ejemplo).
> Por lo tanto git toma el último valor de la clave.

```
 git config user.name
Eleazar Curiel Monjaraz
```
