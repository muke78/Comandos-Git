# Configuracion de alias

- Se ocupa para poder cambiar el git status solo por git s

```bash
    git config --global alias.s status --short
```

- Se ocupa para poder cambiar el git log por git lg y dar mas detalles de lo que se ha subido como la firma del hasheo, en que tiempo se hizo el ultimo commit, nombre del cambio y que autor

```bash
    git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"
```
