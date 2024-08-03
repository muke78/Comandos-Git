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

```bash
    git config core.autocrlf true
```