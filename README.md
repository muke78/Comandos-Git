# Comandos Básicos

- Muestra la versión de Git instalada en el sistema.

```bash
    git --version
```

- Muestra la ayuda para los comandos completos y con alias (--, -).

```bash
    git help
```

# Configuración Inicial de Git

```bash
    git config --global user.name "Erick Muke"
    git config --global user.email "muke7881@gmail.com"
```

- Muestra la configuración establecida del nombre y correo los alias que tienes, los cores, y el nombre de la rama por defecto

```bash
    git config --global -e
```

- Cambia el nombre de la rama por defecto.

```bash
    git config --global init.defaultBranch <name>
```

- Para convertir los finales de línea a LF en todos los sistemas operativos

```bash
    git config --global core.autocrlf input
```

# Gestión de Repositorios

- Ve el estado del nuevo repositorio, la rama actual, archivos y commits.

```bash
    git status
```

- Verifica los cambios realizados, incluyendo autor y fecha.

```bash
    git log
```

- Reconstruye el proyecto al estado del último commit.

```bash
    git checkout -- .
```

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

# Gestion de ramas

- Cambia el nombre a la rama de master a main

```bash
    git branch -m master main
```

# Configuracion de alias

- Se ocupa para poder cambiar el git status solo por git s

```bash
    git config --global alias.s status --short
```

- Se ocupa para poder cambiar el git log por git lg y dar mas detalles de lo que se ha subido como la firma del hasheo, en que tiempo se hizo el ultimo commit, nombre del cambio y que autor

```bash
    git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"
```
