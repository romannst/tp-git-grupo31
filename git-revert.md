# git revert

Deshace los cambios de un commit creando uno nuevo con los cambios opuestos,
sin eliminar el commit original del historial. Esto lo hace seguro para usar
cuando ya subimos cambios al repositorio remoto.

**Sintaxis:**

```
git revert <id-del-commit>
```

**Ejemplo:**

Queremos deshacer el último commit:

```
git revert abc1234
```

Git va a crear un nuevo commit que revierte exactamente lo que hizo `abc1234`,
dejando el historial intacto.
