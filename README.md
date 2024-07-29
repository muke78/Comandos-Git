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

- `git status`: Ve el estado del nuevo repositorio, la rama actual, archivos y commits.
- `git log`: Verifica los cambios realizados, incluyendo autor y fecha.
- `git checkout -- .`: Reconstruye el proyecto al estado del último commit.

# Gestion de Cambios

- `git add`: Prepara todos los archivos para hacer un commit.
- `git reset <nombre_del_archivo>`: Quita los archivos que no se desean incluir en el commit.
- `git push origin <Nombre de la rama>`: Sirve para cargar los commits que se hicieron al repositorio en Github.
- `git commit -m "Primer commit"`: Sube los cambios, registrando un mensaje descriptivo.
- `git init`: Crea el repositorio local, y se crea una carpeta .git para que git pueda llevar un rastro de todo lo que hacemos
- `git commit -am "Cambio que se ha hecho"`: Sirve para agregar los archivos mas aparte hacer el commit al mismo tiempo al poner -am
- `git add *.html/ *.tipo de archivo`: SOlo va a mandar los indices con el tipo de archivo solicitado para subirlo al stage
- `git add js/*.js`: Agrega todos los archivos con extension sobre el directorio indicado
- `git restore --staged *js`: Quita los archivos y los vuelve a bajar del stage para no tomar en cuenta esos archivos sobre el directorio indicado y la extension del archivo indicada

# Gestion de ramas

- `git branch -m master main`: Cambia el nombre a la rama de master a main

# Configuracion de alias

- `git config --global alias.s status --short`: Se ocupa para poder cambiar el git status solo por git s
- `git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"`: Se ocupa para poder cambiar el git log por git lg y mas especifico
