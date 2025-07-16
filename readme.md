# PASOS LABORATORIO GIT

## 1. CREACION DE LOS FICHEROS

- Lo primero que se ha realizado es la creación del fichero 
    **readme.md**
- Luego he inicializado el repositorio en la ruta con el siguiente comando

```bash
    git init
```
- Inicializado el repositorio en local he creado un nuevo repositorio en Git Hub para poder enlazarlo con el repositorio local y poder subir los cambios 

```bash
    git remote add origin git@github.com:DavidRiveraArtero/LaboratorioGiclst.git
```

- Una vez terminado el paso anterior guardé mis datos en local con los comandos
```bash
   git add .
   git commit -m "fichero readme.md"
```

- Después de esto cree el fichero index.html y volví a guardar los cambios en local.
```bash
   git add .
   git commit -m "Creado el fichero index.html
```

- Creado estos 2 ficheros hice mi push para guardar los cambios en Git Hub 

```bash
    git push --set-upstream origin main
```

## 2. CREACIÓN DE RAMAS

- Para crear la rama y cambiar a esta, use el siguiente comando
```bash
    git branch development
    git checkout development
```

- Una vez en esta rama realizamos un cambio en el fichero index.html

- Terminado el cambio ejecutaremos los siguientes comando para guardar todos los cambios y subirlos a Git Hub

```bash
    git commit -am "Cambiado el título de index.html"
    git push -u origin development 
```

## 3. MERGE

- Cambiamos a la rama **main**
```bash
    git checkout main
```

- Para aplicar los cambios realizados en la rama development ejecutamos este comando
```bash
    git merge development    
```

- Por último subiremos los cambios a Git Hub
```bash
    git push 
```