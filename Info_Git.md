# Git Info

## Documentacion y ligas
1. Readme.md: [Documentación](https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

## Configuración
### Obtener version
```
git --version
```
### Información de configuracion del git
```
git config --list
git config --list --show-origin
```
### Asignar nombre y correo
```
git config --global user.name "nombre"
git config --global user.email "email@outlook.com"
```

## Primeros pasos, cargar nuevo proyecto
1. __Iniciar git:__
    * git init
2. __Agregar todos los archivos__
    * git add .
3. __Hacer commit__
    * git commit -m "Primer commit"
4. __Agregar a repositorio remoto__
    * git remote add origin https://github.com/victor000001/Info.git
5. __Elegir la rama__
* __con rama master__ 
    * git push --set-upstream origin master
* __en otra rama__
    * git branch -M nueva_rama
    * git push -u origin main

## Comandos
### Crea un nuevo repositorio en la carpeta
```
git init
```
### Agrega un archivo o todos los archivos modificados al staging, 
```
git add archivo.txt
git add .
```
### Agregar cambios del staging al repositorio local
```
git commit -m "version_1"
```
### Estatus de la base de datos
```
git status
```
### Mostrar historico de cambios
```
git show archivo.txt 
```
### Historia entera de los commits o un archivo
```
git log
git log --stat
git log archivo.txt
```
### Regresa un archivo a un commit especifico o la ultima version de la rama
```
git checkout id_del_commit archivo.txt
git checkout master archivo.txt
```
### Volver a una version especifica de un commit (AVISO se borran los demas commits)
```
git reset id_del_commit --hard
```
### Elminar un archivo (va a seguir existiendo en el historial de git)
```
git rm --force
```
### Clonar el repositorio remoto de una rama
```
git clone -b master https://github.com/victor000001/Info.git
```
### Subir a repositorio remoto
```
git push
```
### Descargar de repositorio remoto
```
git pull
```
### Informacion del archivo
```
cat archivo.txt
```
### Obtenemos los cambios entre dos commits especificos
```
git diff
git diff id_del_commit id_del_commit
```

## Flujos
### Actualizar archivos
```
git add .
git commit -m "Merge develop"
git push
```
### Recuperar ultimo commit
```
git checkout -- .
```
### Ramas
```
git branch
git branch -r
```
### Merge
```
git remote update origin
git branch -a
git merge remotes/origin/qAssurance
```
### Cherry-pick Pasar commit especifico (no merge)
```
git cherry-pick codigo_del_commit
```
### Nueva rama con los cambios actuales hasta hacer commit y push sube la rama remota
```
git checkout -b origin/Ajuste-Promociones
```

## GitBash
### Obtener ruta
```
pwd
```
### Home del disco
```
cd /
```
### Lista archivos
ls -al prueba