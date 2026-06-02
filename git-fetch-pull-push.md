# git fetch, git pull y git push

Estos tres comandos se usan para sincronizar el repositorio local con el repositorio remoto.

## git fetch

Descarga los cambios del repositorio remoto pero no los aplica a los archivos de trabajo.
Los cambios quedan guardados internamente en Git, listos para revisarlos antes de integrarlos.

**Sintaxis:**

```
git fetch origin
```

**Ejemplo:**

Queremos ver qué cambios subieron nuestros compañeros sin modificar nuestros archivos todavía:

```
git fetch origin
```

Para integrar esos cambios después, habría que hacer un `git merge`.

## git pull

Descarga los cambios del repositorio remoto y los aplica directamente a los archivos de trabajo.
Es equivalente a hacer un `git fetch` seguido de un `git merge`.

**Sintaxis:**

```
git pull origin <rama>
```

**Ejemplo:**

Queremos traer y aplicar los últimos cambios de la rama main:

```
git pull origin main
```

## git push

Sube los commits realizados en el repositorio local al repositorio remoto.
Solo se pueden subir cambios que ya fueron confirmados con `git commit`.

**Sintaxis:**

```
git push origin <rama>
```

**Ejemplo:**

Subimos los commits de nuestra rama al repositorio remoto en GitHub:

```
git push origin alumno4_rama
```