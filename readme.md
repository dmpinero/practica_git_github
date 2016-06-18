- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
Comandos
--------
  git reset --hard HEAD~1

Comentarios
-----------
  Se utiliza el comando git reset para deshacer un commit.
  Con el modificador --hard se indica que no se quiera conservar el contenido de
  lo que esté actualmente en el área de trabajo (working copy).
  Con HEAD~1 indicamos que queremos que el puntero HEAD apunte al commit anterior
  (~1) al actual.
  Además el staging area queda vacío.

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
Comandos
--------
  git reflog
  git reset --hard "código_SHA_del_commit"

Comentarios
-----------
  git reflog permite conocer el historial de commits realizados.
  Una vez localizado el commit deseado (mirando los comentarios del commit) se
  ejecuta git reset --hard "código_SHA_del_commit" (git reset --hard d352e20) en
  mi caso. Con esto se consigue git apunte al commit deseado.

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
No, porque la rama styled ya contenía a la rama master. De hecho no se realizó
ningún commit.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Sí causó conflicto, porque el contenido del archivo git-nuestro.md en las ramas
styled y htmlify es distinto en las mismas líneas del archivo.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
- ¿Qué comando o comandos utilizaste en el paso 25?
- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
- ¿Qué comando o comandos utilizaste en el paso 27?
- ¿Qué comando o comandos utilizaste en el paso 28?
- ¿Qué comando o comandos utilizaste en el paso 29?
- ¿Qué comando o comandos utilizaste en el paso 30?
- ¿Qué comando o comandos usaste en el paso 32?
- ¿Qué comando o comandos usaste en el punto 33?

Comandos
--------
Comentarios
-----------
