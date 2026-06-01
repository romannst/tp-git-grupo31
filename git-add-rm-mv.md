# git add, git rm y git mv

Estos tres comandos se usan para gestionar archivos dentro del staging area, que es la zona intermedia donde se preparan los cambios antes de confirmarlos con un commit.

## git add

Le indica a Git qué archivos queremos incluir en el próximo commit.
Cuando modificamos un archivo, Git detecta el cambio pero no lo incluye automáticamente, primero hay que agregarlo al staging area.

**Sintaxis:**
git add <archivo>   <-- agrega un archivo específico
git add .           <-- agrega todos los archivos modificados

**Ejemplo:**
Modificamos el archivo index.html y queremos incluirlo en el próximo commit:
git add index.html

## git rm

Elimina un archivo del proyecto y le avisa a Git que deje de trackearlo.
Si borramos un archivo manualmente sin usar este comando, Git lo detecta como un cambio sin stagear y hay que agregarlo igual.

**Sintaxis:**
git rm <archivo>

**Ejemplo:**
git rm archivo-viejo.txt

## git mv

Renombra o mueve un archivo dentro del proyecto, registrando el cambio
en Git automáticamente. Si lo hacemos a mano, Git lo interpreta como
que borramos un archivo y creamos uno nuevo, perdiendo el historial.

**Sintaxis:**
git mv <nombre-actual> <nombre-nuevo>

**Ejemplo: Renombra**
git mv pagina.html index.html

**Ejemplo: Mueve**
git mv index.html carpeta/index.html

**Ejemplo: Renombra y mueve**
git mv pagina.html carpeta/index.html