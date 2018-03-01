# Práctica GIT - Respuestas

### Grosu, Maria Alisia 2DA

--

**1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?**

`git reset --hard HEAD~1`

He utilizado este comando para ir un paso hacia atrás y deshacer el último commit, perdiendo lo que había en el working copy y el staging area también queda vacío.
--
**2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

`git reflog`
`git reset 5a601c5`
En este caso he utilizado dos comandos, en primer lugar "git reflog" para ver todos los cambios que se han hecho en el repositorio, con la ayuda de este historial he saltado con git reset y el indentificador al paso que había deshecho. Con `git checkout <HASH>` también se puede cambiar de rama.
--
**3. El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**
`git branch`
`git merge master`
En primer lugar, he comprobado que estoy en la rama "styled" que es la que va a absorber a "master" y en segundo lugar he heho el merge con fast-forward porque es lineal y he vuelto a hacer el commit para resolver el conflicto.
--
**4. El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**
`git branch`
`git merge htmlify`
Styled es la rama que absorbe a htmlify, por eso he comprobado primero que estoy en la rama styled y luego he hehco el merge fast-forward con la rama master que luego me ha causado un conflicto y lo he resuelto con `git merge --abort`, de esta manera me he quedado con el contenido de la rama styled.
--
**5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**
`git branch`
`git checkout master`
`git merge master`
Me he cambiado a la rama master para absorber a styled y se realiza el merge sin conflictos con "fast-forward".
--
**6. ¿Qué comando o comandos utilizaste en el paso 25?**
`git log --graph`
--
**7. El merge del paso 26, ¿Podría ser fast-forward? ¿Por qué?**
`git branch`
`git merge --no-ff title`
Si el merge fuese fast-forward el punetro de master se desplazaria al commit de title, pero en este caso title esta en su commit y el HEAD y master se desplazan al commit de la unión.
--
**8. ¿Qué comando o comandos utilizaste en el paso 27?**
`git reset HEAD~1`
Deshacemos el merge sin perder los cambios del working copy.
--
**9. ¿Qué comando o comandos utilizaste en el paso 28?**
`git checkout don-quijote.md`
--
**10. ¿Qué comando o comandos utilizaste en el paso 29?**
`git branch -D title`
--
**11. ¿Qué comando o comandos utilizaste en el paso 30?**
`git reflog`
`git chekout (identificador)`
--
**12. ¿Qué comando o comandos usaste en el paso 32?**
`git reflog`
`git reset (identificador)`
--
**13. ¿Qué comando o comandos usaste en el punto 33?**
`git reflog`
`git reset 51a0b8a`
--

