# Comandos Básicos

- `git --version`: Muestra la versión de Git instalada en el sistema.
- `git help`: Muestra la ayuda para los comandos completos y con alias (--, -).

# Configuración Inicial de Git

- `git config --global user.name "Erick Muke"`
- `git config --global user.email "muke7881@gmail.com"`
- `git config --global -e`: Muestra la configuración establecida del nombre y correo.
- `git config --global init.defaultBranch <name>`: Cambia el nombre de la rama por defecto.

# Gestión de Repositorios

- `git status`: Ve el estado del nuevo repositorio, la rama actual, archivos y commits.
- `git add`: Prepara todos los archivos para hacer un commit.
- `git reset <nombre_del_archivo>`: Quita los archivos que no se desean incluir en el commit.
- `git commit -m "Primer commit"`: Sube los cambios, registrando un mensaje descriptivo.
- `git init`: Crea el repositorio local, y se crea una carpeta .git para que git pueda llevar un rastro de todo lo que hacemos
- `git log`: Verifica los cambios realizados, incluyendo autor y fecha.
- `git checkout -- .`: Reconstruye el proyecto al estado del último commit.
- `git push origin <Nombre de la rama>`: Sirve para cargar los commits que se hicieron al repositorio en Github.
