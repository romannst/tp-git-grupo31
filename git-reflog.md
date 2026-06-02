# git reflog

Muestra un historial completo de todos los movimientos realizados en el repositorio local,
incluyendo commits, merges, resets y cambios de rama. A diferencia de `git log`, el reflog
registra todo lo que ocurrió, hasta commits que fueron eliminados o que
ya no aparecen en el historial normal.
Es útil para recuperar contenido que fue borrado accidentalmente.

**Sintaxis:**

```
git reflog
```

**Ejemplo de salida:**

```
7576b23 (HEAD -> gianfranco_tarulli) HEAD@{0}: commit: docs: Agrego explicacion de git revert
d6bd9cd HEAD@{1}: commit: docs: Agrego explicacion de git fetch, git pull y git push
ab070c2 HEAD@{2}: commit: docs: Agrego explicacion de git remote -v
```

Cada línea muestra el id del commit, la posición en el historial y la acción realizada.

**Ejemplo de uso para recuperar un commit eliminado:**

Si borramos un commit con `git reset` y queremos recuperarlo, buscamos su id en el
reflog y usamos `git checkout` para volver a él:

```
git reflog
git checkout abc1234
```