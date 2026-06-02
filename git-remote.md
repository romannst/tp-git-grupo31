# git remote

El comando `git remote` se usa para gestionar las conexiones a repositorios remotos.
Un remoto es simplemente un repositorio alojado en otro lugar, como GitHub.

## git remote -v 

Muestra los nombres y las URLs de los repositorios remotos vinculados al proyecto local,
tanto para fetch como para push.

**Sintaxis:**

```
git remote -v
```

**Ejemplo de salida:**

```
origin  https://github.com/usuario/repo.git (fetch)
origin  https://github.com/usuario/repo.git (push)
```

`origin` es el nombre que Git asigna por defecto al remoto cuando clonamos un repositorio.
El `-v` viene de *verbose*, que significa "mostrar con detalle".