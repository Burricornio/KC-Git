# Ejercicio Git

Se deberá crear un repositorio y realizar una serie de operaciones **desde la consola de
comandos** sobre el mismo para posteriormente subir el repositorio a Github.

Se deberá entregar a través del formulario de prácticas indicando la URL del repositorio. En el
repositorio, deberá existir un archivo readme.md con las respuestas a las siguientes preguntas:

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

    **git reset --hard HEAD~1**: Utilizo la directiva --hard para modificar el working copy

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

  1. **git reflog**: Para seguir el rastro de los commits (Hash) y situarnos en el anterior

  2. **git checkout identificadorCommit**: Entramos en *Detached HEAD* (Nuestro HEAD apunta a un commit) 

  3. **git checkout -b nombreRamaTemporal**: Creo una nueva rama temporal para poder guardar el commit

  4. **git checkout styled**: Cambio a la rama styled.

  5. **git merge nombreRamaTemporal**: Absorvemos la rama temporal.

  6. **git branch -D nombreRamaTemporal**: Elimino rama temporal.

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

    Nos dice que la rama ya está al día porque styled es hija de la rama master.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
    
    **Sí causa un conflicto**. Debido a que hemos modificado las mismas líneas en el archivo git-nuestro.md.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

    No genera ningun conflicto. Al estar en línea no hay ningun problema. El archivo git.nuestro.md es reemplazado por el contnido que tiene en la rama styled.

- ¿Qué comando o comandos utilizaste en el paso 25?

    Creo un alias global: **git config --global alias.graph 'log --graph --decorate --oneline'**

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

    Sí podría ser fast forward porque no hay ramificaciones (estan en línea).

- ¿Qué comando o comandos utilizaste en el paso 27?

    **git reset HEAD~1**: Para volver hacía atrás.

- ¿Qué comando o comandos utilizaste en el paso 28?

    **git checkout -- git-nuestro.md**: Para descartar los cambios.

- ¿Qué comando o comandos utilizaste en el paso 29?

    **git branch -D title**

- ¿Qué comando o comandos utilizaste en el paso 30?

    1. **git reflog**: Listar movimientos.

    2. **git checkout numeroCommit** en el que añadimos el titulo: Para situarnos en el momento en que creamos el titulo.

    3. **git checkout -b rama-temporal**: Creamos una rama temporal.

    4. **git branch master**: Nos movemos a master.

    5. **git merge rama-temporal**: Master absorve a temporal.

    6. **git branch -D rama-temporal**: Elimino la rama temporal

- ¿Qué comando o comandos usaste en el paso 32?

    1. **git log**: Para localizar el HASH del commit inicial

    2. **git checkout numeroCommit** : Nos situamos en el commit inicial.

- ¿Qué comando o comandos usaste en el punto 33?

    1. **git reflog**: Listamos los movimientos.

    2. **git checkout numeroCommit**: Me desplazo a cada commit.

    3. **git tag x**: Ponemos nobre a cada etiqueta.

    4. Nos movemos entre tags con **git checkout numeroCommit**