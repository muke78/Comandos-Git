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

- Es un comando que sirve para ver todo el historial de cambios dentro de git, nos recupera todo aunque se hayan quitado o se hayan modificado con su hash el conteo de HEAD y en donde cual commit estamos, al aplicar el comando `reset` con el hash que sacamos de `reflog` podemos restablecer todo el proyecto a un punto en especifico donde el proyecto se encuentre estable

```bash
    git reflog
```
