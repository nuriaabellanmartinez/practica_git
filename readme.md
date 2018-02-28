**-¿Qué comando utilizaste en el paso 11? ¿Por qué?**

< git reset --hard HEAD~1  >

Utilicé esta expresión porque si hubiese utilizado: < git reset HEAD~1 > no habría perdido los cambios en el working copy. Al escribir este comando más fuerte con el --hard sí se pierden. 


**-¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

Primero entré a consultar mis commits hasta el momento: < git reflog >
Después copié el código del commit que había deshecho y lo rehice incluyéndolo con el siguiente comando: < git reset --hard cd9adf6 >

Hice estos pasos porque consultar mi historial de commits con el reflog era el método pertinente para recuperar ese paso, copiando y pegando exactamente el punto al que quisiese volver. 

**-El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

No, pues la rama styled accede sin problemas a la rama master. <git merge master >


**-El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**

Sí, pues en las dos ramas hay un archivo don-quijote.md aunque con distintas modificaciones. 

**-El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**

No, pues el archivo don-quijote.md no había sufrido variaciones.

**-¿Qué comando o comandos utilizaste en el paso 25?**

< git graph >

**-El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

Sí, pues el archivo de la rama master no ha sido alterado. 

**-¿Qué comando o comandos utilizaste en el paso 27?**

< git reset HEAD~1 > para deshacer la orden anterior sin perder la información de working copy. 

**-¿Qué comando o comandos utilizaste en el paso 28?**

< git checkout -- don-quijote.md > para descartar los cambios realizados en el archivo. 

**-¿Qué comando o comandos utilizaste en el paso 29?**

< git branch -D title > desde otra rama, pues no podemos borrar la rama en la que estamos. 

**-¿Qué comando o comandos utilizaste en el paso 30?**

< git reflog > para coger el código del paso en el que deshice el merge. 

< git reset --hard 2c67177 > para retroceder en ese paso en el que se deshacía el merge. 
 > 

**-¿Qué comando o comandos usaste en el paso 32?**

< git reflog >para coger el código del primer commit.

< git checkout fae458c > para situarnos en ese paso.

**-¿Qué comando o comandos usaste en el punto 33?**

De nuevo utilicé: < git reflog > para copiar el código del paso en que añadimos título en el archivo don-quijote.md, seguido de < git checkout ddf7b50 > para retroceder hasta ese paso. 