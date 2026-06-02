# git add, git rm y git mv

Estos tres comandos gestionan el staging area.

## git add

Agrega un archivo que haya sido modificado al staging area.

**Ejemplo:**

git add index.html

## git rm

Elimina un archivo del proyecto y le avisa a Git que deje de trackearlo.

**Ejemplo:**

git rm archivo-viejo.txt

## git mv

Renombra o mueve un archivo dentro del proyecto, registrando el cambio.

**Ejemplos:**

*Renombra:* 
git mv pagina.html index.html

*Mueve:* 
git mv index.html carpeta/index.html

*Renombra y mueve:* 
git mv pagina.html carpeta/index.html