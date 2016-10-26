- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
	git reset --hard HEAD~1
    este comando deshace el ultimo commit realizado y limpia el working copy

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
	git reflog
        este comando permite buscar el commit al que necesito regresas
    git reset --hard f40aacd
        este comando me permite rehacer al commit que necesito

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
	Realizar el merge no causo conflicto
    git branch
          master
        * styled
    git merge master
        Already up-to-date.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
	SI causo conflictos ya que el contenido del archivo de las dos ramas es diferente

    CONFLICTO(contenido): conflicto de fusión en git-nuestro.md
    Automatic merge failed; fix conflicts and then commit the result.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
	NO causo conflictos, se realizo un fast forward
    git checkout master
        Switched to branch 'master'
        eduardo@eduardo-NV55C:$ git branch
          htmlify
        * master
          styled
    git merge styled
        Updating c11f99e..dca991f
        Fast-forward
        git-nuestro.md | 19 +++++++++----------
        1 file changed, 9 insertions(+), 10 deletions(-)

- ¿Qué comando o comandos utilizaste en el paso 25?

git graph

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

	Si, ya que el HEAD actual es un ancestro del commit que se esta
	tratando de hacer merge

- ¿Qué comando o comandos utilizaste en el paso 27?

	git reset --soft HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 28?

	git reset HEAD git-nuestro.md

- ¿Qué comando o comandos utilizaste en el paso 29?

	git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30?

	git reflog
        este comando permite buscar el paso que se realizo el merge
    git checkout 12222d9
        regresar al merge solicitado

- ¿Qué comando o comandos usaste en el paso 32?

	git log
        este comando permite buscar el commit inicial
    git checkout c11f99efd6a0915b47b63c5b070df1600a4dcd1d
        regresar al commit inicial

- ¿Qué comando o comandos usaste en el punto 33?

	git reflog
        este comando permite buscar el commit del titulo final
    git checkout 5042e9b
        volver al commit del titulo final