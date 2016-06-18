**¿Qué comando utilizaste en el paso 11? ¿Por qué?**

git reset --hard HEAD~1

Se utiliza el comando git reset para deshacer un commit.
Con el modificador --hard se indica que no se quiera conservar el contenido de
lo que esté actualmente en el área de trabajo (working copy).
Con HEAD~1 indicamos que queremos que el puntero HEAD apunte al commit anterior
(~1) al actual.
Además el staging area queda vacío.

**¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

git reflog

git reset --hard "código_SHA_del_commit"

git reflog permite conocer el historial de commits realizados.
Una vez localizado el commit deseado (mirando los comentarios del commit) se
ejecuta git reset --hard "código_SHA_del_commit" (git reset --hard d352e20) en
mi caso. Con esto se consigue git apunte al commit deseado.

**El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

No causó conflicto porque la rama styled ya contenía a la rama master.

De hecho no se realizó ningún commit.

**El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**

Sí causó conflicto, porque el contenido del archivo git-nuestro.md en las ramas
styled y htmlify es distinto en las mismas líneas del archivo.

**El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**

No causó conflicto porque la rama styled estaba un commit más
adelantado que la rama master, por lo que pudo hacerse un fast-fordward y
mover el puntero HEAD y el puntero de la rama master desde el commit de la
rama master al commit de la rama styled.

**¿Qué comando o comandos utilizaste en el paso 25?**

git log --graph --decorate --pretty=oneline

**El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

Sí, porque master podría absorber a title moviendo el puntero head a la rama
title, que está un commit más avanzado.

**¿Qué comando o comandos utilizaste en el paso 27?**

git reset HEAD~1

**¿Qué comando o comandos utilizaste en el paso 28?**

git checkout -- git-nuestro.md

**¿Qué comando o comandos utilizaste en el paso 29?**

git branch -D title

**¿Qué comando o comandos utilizaste en el paso 30?**

git reflog para ver el historial de commits realizados

git reset --hard 5607f86 para posicionar el puntero HEAD en el commit en el que
realicé el merge de las ramas master y title

**¿Qué comando o comandos usaste en el paso 32?**

git reflog para ver el historial de commits realizados

git reset --hard 9f1f0be para posicionar el puntero HEAD en el commit inicial

**¿Qué comando o comandos usaste en el punto 33?**

git reflog para ver el historial de commits realizados

git reset --hard abbd726  para posicionar puntero el HEAD en el commit en el
que se puso un título al poema
