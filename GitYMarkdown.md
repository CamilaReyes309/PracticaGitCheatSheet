# **GIT Y MARKDOWN**

## ***Indice:***
<br>

### - **GIT**

1. ¿Qué es Git?

2. ¿Qué es un sistema de control de versiones?

3. ¿Para qué sirve Git?

4. Características de Git

5. Diferentes estados de un fichero Git

6. Comandos basicos de Git


### - **MARKDOWN**

1. ¿Qué es Markdown?

2. ¿Para qué sirve Markdown?

<br>

---

<br>

## **GIT**

<br>

 ## **1. ¿Qué es Git?** 

Git es un sistema de control de versiones distribuido, diseñado por Linus Torvalds. Está pensando en la eficiencia y la confiabilidad del mantenimiento de versiones de aplicaciones cuando estas tienen un gran número de archivos de código fuente.

<br>

![git](https://www.solucionex.com/sites/default/files/categorias_post/git.jpg)

<br>

## **2. ¿Qué es un sistema de control de versiones?**

El SCV o VCS (por sus siglas en inglés) es un sistema que registra los cambios realizados sobre un archivo o conjunto de archivos a lo largo del tiempo, de modo que puedas llevar el historial del ciclo de vida de un proyecto, comparar cambios a lo largo del tiempo, ver quién los realizó o revertir el proyecto entero a un estado anterior.

Cualquier tipo de archivo que se encuentre en un ordenador puede ponerse bajo control de versiones.

<br>

<br>

## **3. ¿Para qué sirve Git?**

Con Git se obtiene una mayor eficiencia usando archivos de texto plano(Markdown), ya que con archivos binarios no puede guardar solo los cambios, sino que debe volver a grabar el archivo completo ante cada modificación, por mínima que sea, lo que hace que incremente demasiado el tamaño del repositorio.

<br>

## **4. Caracteristicas de Git:**

- Git almacena la información como un conjunto de archivos.

- No existen cambios, corrupción en archivos o cualquier alteración sin que Git lo sepa.

- Casi todo en Git es local. Es difícil que se necesiten recursos o información externos, basta con los recursos locales con los que cuenta.

- Git cuenta con 3 estados en los que es posible localizar archivos: Staged, Modified y Committed.

<br>

## **5. Diferentes estados de un fichero Git:**

<br>

![areas](https://git-scm.com/book/en/v2/images/areas.png)

<br>

- *Existen tres tipos de estado de un fichero Git:*

- Secciones principales de un proyecto Git:

  - **Confirmado:** significa que los datos están almacenados de manera segura en tu base de datos local. 
  
  - **Modificado:** significa que has modificado el archivo pero todavía no lo has confirmado a tu base de datos. 
  
  - **Preparado:** significa que has marcado un archivo modificado en su versión actual para que vaya en tu próxima confirmación.

Esto nos lleva a las tres secciones principales de un proyecto de Git: El directorio de Git (Git directory), el directorio de trabajo (working directory), y el área de preparación (staging area).


<br>

## **6. Comandos basicos de Git**

<br>

![comandos de git](https://www.freecodecamp.org/espanol/news/content/images/size/w2000/2022/05/comandos-GIT.png)

<br>

### ***1. Git clone:*** 

    *  Git clone es un comando para descargar el código fuente existente desde un repositorio remoto (como Github, por ejemplo). En otras palabras, Git clone básicamente hace una copia idéntica de la última versión de un proyecto en un repositorio y la guarda en su computadora.

<br>

- **SINTAXIS:**
~~~
git clone https://name-of-the-repository-link
~~~



### ***2. Git branch:***

    * Las ramas son muy importantes en el mundo de git. Mediante el uso de ramas, varios desarrolladores pueden trabajar en paralelo en el mismo proyecto simultáneamente. Se puede usar el comando git branch para crear, enumerar y eliminar ramas. Podemos usar el comando git branch para crear, enumerar y eliminar ramas. 

<br>

- **SINTAXIS:**

- Creando una nueva rama:

~~~
git branch <branch-name>
~~~

- Este comando creará una rama localmente. Para insertar la nueva rama en el repositorio remoto, debes usar el siguiente comando:
~~~
git push -u <remote> <branch-name>
~~~

- Para ver las ramas:

~~~
git branch or git branch --list
~~~

- Para borrar las ramas:

~~~
git branch -d <branch-name>
~~~

### ***3. Git checkout:***

    * Este es también uno de los comandos Git más utilizados. Para trabajar en una rama, primero debe cambiarse a ella. Git checkout se usa principalmente para cambiar de una rama a otra. También podemos usarlo para verificar archivos y confirmaciones.

<br>

- **SINTAXIS:**

~~~
git checkout <name-of-your-branch>
~~~

- Hay algunos pasos que debes seguir para cambiar con éxito entre ramas:  

Los cambios en tu rama actual deben confirmarse o guardarse antes de cambiar.
La rama que deseas verificar debe existir en tu local.
También hay un comando de acceso directo que te permite crear y cambiar a una rama al mismo tiempo:

~~~
git checkout -b <name-of-your-branch>
~~~

### ***4. Git status:***

    * El comando de estado de Git brinda toda la información necesaria sobre la rama actual.

<br>

- **SINTAXIS:**

~~~
git status
~~~

- Puede recopilar información acerca de:  

    - Si la rama actual está actualizada.    
    - Si hay algo que necesita un commit, un add, o borrarse.  
    - Si hay archivos preparados, sin preparar o sin seguimiento    
    - Si hay archivos creados, modificados o eliminados


### ***5. Git add:***

    * Cuando se crea, modifica o elimina un archivo, estos cambios ocurriren en el local y no se incluirán en la próxima confirmación (a menos que se cambien las configuraciones).

Se necesita usar el comando git add para incluir los cambios de un archivo(s) en nuestro próximo commit.

<br>

- **SINTAXIS:**

- Para agregar un solo archivo:

~~~
git add <file>
~~~

 - Para añadir todo de una vez:

~~~
git add -A
~~~

### ***6. Git commit:***

    * Este es quizás el comando más utilizado de Git. Una vez que se llega a cierto punto en el desarrollo, queremos guardar nuestros cambios (tal vez después de una tarea o problema específico).

    Git commit es como establecer un punto de control en el proceso de desarrollo al que puede volver más tarde si es necesario. También necesitamos escribir un mensaje corto para explicar lo que hemos desarrollado o cambiado en el código fuente.

<br>

- **SINTAXIS:**

~~~
git commit -m "commit message"
~~~

Importante: Git commit guarda tus cambios solo localmente.

### ***7. Git push:***

    * Después de confirmar los cambios (con git commit), lo siguiente que hay que hacer es enviar estos cambios al servidor remoto. Git push sube tus confirmaciones al repositorio remoto.

<br>

- **SINTAXIS:**

~~~
git push <remote> <branch-name>
~~~

- Sin embargo, si tu rama se creó recientemente, también debes cargar la rama con el siguiente comando:

~~~
git push --set-upstream <remote> <name-of-your-branch>
~~~

- O bien:

~~~
git push -u origin <branch_name>
~~~

<u>*Importante: Git push solo carga los cambios que están confirmados.*</u>

### ***8. Git pull:***

    * El comando git pull se usa para obtener actualizaciones del repositorio remoto. Este comando es una combinación de git fetch y git merge, lo que significa que, cuando se usa git pull, se obtienen las actualizaciones del repositorio remoto (git fetch) e inmediatamente aplica los últimos cambios en su local (git merge). (En simples palabras, sirve para traer el repositorio remoto a tu repositorio local).

<br>

- **SINTAXIS:**

~~~
git pull <remote>
~~~

*<u>Esta operación puede causar conflictos que debes resolver manualmente.</u>*

### ***9. Git revert:***

    * Este se utiliza para deshacer los cambios que hemos hecho. Hay varias formas de deshacer los cambios, de forma local o remota (depende de lo que necesitemos), pero se deben usar estos comandos con cuidado para evitar eliminaciones no deseadas.

<br>

- **SINTAXIS:**

- Para ver el historial de confirmaciones, primero debemos usar git log -- oneline:

- Luego, solo necesitamos especificar el código hash junto a nuestro commit que nos gustaría deshacer:

~~~
git revert 3321844
~~~

- Después de esto, verás una pantalla como la siguiente: simplemente presiona shift + q para salir.

![git revert1](https://www.freecodecamp.org/espanol/news/content/images/2022/05/image-5.png)

- El comando Git revert deshará la confirmación dada, pero creará una nueva confirmación sin eliminar la anterior:

![git revert2](https://www.freecodecamp.org/espanol/news/content/images/2022/05/image-5.png)

### ***10. Git merge:***

    * La herramienta git merge se utiliza para fusionar uno o más ramas dentro de la rama que tienes activa. 

    Git merge básicamente integra su rama de características (feature branch) con todas sus confirmaciones en la rama dev (o master). Es importante recordar que primero se debe estar en la rama específica que se desea fusionar con la rama de características.

<br>

- **SINTAXIS:**

- Por ejemplo, cuando desees fusionar tu rama de características en la rama dev:

    - Primero debes cambiar a la rama dev:

~~~
git checkout dev
~~~

    - Antes de hacer la fusión, debes actualizar la rama de desarrollo local:

~~~
git fetch
~~~

    - Finalmente, puedes hacer la fusión:

~~~
git merge <branch-name>
~~~

*<u>Sugerencia: asegúrate que tu rama de desarrollo tenga la última versión antes de fusionar las ramas, de lo contrario, puede enfrentar conflictos u otros problemas no deseados.</u>*

<br>

---

<br>

## **MARKDOWN**

<br>

![MARKDOWN](https://geekytheory.com/content/images/size/w2000/2014/03/markdown.png)

<br>

## **1. ¿Qué es Markdown?**

Markdown nació como herramienta de conversión de texto plano a HTML. Markdown es un lenguaje simple que se utiliza para crear texto enriquecido (por ejemplo, HTML) con un editor de texto sin formato. Te permite darle un formato básico al texto, utilizando símbolos conocidos y accesibles en todos los teclados.

<br>

## **2. ¿Para qué sirve Markdown?**

es un lenguaje de marcado sencillo que sirve para agregar formato, vínculos e imágenes con facilidad al texto simple. Este método te permitirá añadir formatos tales como negritas, cursivas o enlaces, utilizando simplemente texto plano, lo que hará de tu escritura algo más simple y eficiente al evitar distracciones.
