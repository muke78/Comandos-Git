# Gestion de Cambios

- Prepara todos los archivos para hacer un commit.

```bash
    git add
```

- Quita los archivos que no se desean incluir en el commit.

```bash
    git reset <nombre_del_archivo>
```

- Sirve para cargar los commits que se hicieron al repositorio en Github.

```bash
    git push origin <Nombre de la rama>
```

- Sube los cambios, registrando un mensaje descriptivo.

```bash
    git commit -m "Primer commit"
```

- Crea el repositorio local, y se crea una carpeta .git para que git pueda llevar un rastro de todo lo que hacemos

```bash
    git init
```

- Sirve para agregar los archivos mas aparte hacer el commit al mismo tiempo al poner -am

```bash
    git commit -am "Cambio que se ha hecho"
```

- Solo va a mandar los indices con el tipo de archivo solicitado para subirlo al stage

```bash
    git add *.html/ *.tipo de archivo
```

- Agrega todos los archivos con extension sobre el directorio indicado

```bash
    git add js/*.js
```

- Quita los archivos y los vuelve a bajar del stage para no tomar en cuenta esos archivos sobre el directorio indicado y la extension del archivo indicada

```bash
    git restore --staged *js
```

- <span style="color: yellow;">Hace una comparador de cambios de lo que se cambio y lo que habia antes de subirlo al stage (funciona en codigos mas cortos)</span>

```bash
    git diff
```

- <span style="color: yellow"> Compara los cambios subidos al staged despues de hacer un `git add .`</span>

```bash
    git diff --staged
```

- Realiza el cambio del nombre del ultimo commit hecho

```bash
    git commit --amend -m "<Mensaje nuevo>"
```

- Sirve para que el ultimo commit que se hizo se pueda resetear y git lo quita del registro para subir los cambios que hicieron falta y se vuelvan a subir (`Esto no se recomienda cuando ya este en github, la mejor practica es un nuevo commit`) 

```bash
    git reset --soft HEAD^[numero de cambios anteriores]
```

```bash
    git reset --soft <"Hash de el segundo commit hecho">
```

- El `reset --soft` mantiene los cambios que se tienen
- El `reset  --mixed` saca los cambios del staged para que se puedan agregar de nuevo con `git add`
- El `reset --hard` saca los cambios del staged pero no guarda los cambios que se tenian anteriormente y regresa el codigo al punto original