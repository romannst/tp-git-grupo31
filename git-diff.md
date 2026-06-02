# git diff

Permite comparar los estados del código, mostrando exactamente qué líneas fueron
agregadas o modificadas (en verde) y cuáles fueron eliminadas (en rojo).
A diferencia de `git status`, que solo indica qué archivos cambiaron, `git diff`
muestra el contenido exacto de los cambios.

**Sintaxis:**

```
git diff
```

**Ejemplo de salida:**

```
- Esta línea fue eliminada
+ Esta línea fue agregada
```

**Variantes útiles:**

```
git diff                  # muestra cambios que todavía no fueron agregados al staging area
git diff --staged         # muestra cambios que ya están en el staging area
git diff <rama1> <rama2>  # compara dos ramas entre sí
```

**Ejemplo:**

Modificamos un archivo y queremos ver qué cambió antes de hacer el commit:

```
git diff index.html
```