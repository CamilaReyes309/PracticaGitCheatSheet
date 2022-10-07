# GIT Y MARKDOWN

Indice
GIT

¿Qué es Git?
¿Qué es un sistema de control de versiones?
¿Para qué sirve Git?
Características de Git
Diferentes estados de un fichero Git
10 Comandos basicos de Git
MARKDOWN
¿Qué es Markdown?
¿Para qué sirve Markdown?


GIT

Git es un sistema de control de versiones distribuido, diseñado por Linus Torvalds. Está pensando en la eficiencia y la confiabilidad del mantenimiento de versiones de aplicaciones cuando estas tienen un gran número de archivos de código fuente.

¿Qué es un sistema de control de versiones?

El SCV o VCS (por sus siglas en inglés) es un sistema que registra los cambios realizados sobre un archivo o conjunto de archivos a lo largo del tiempo, de modo que puedas llevar el historial del ciclo de vida de un proyecto, comparar cambios a lo largo del tiempo, ver quién los realizó o revertir el proyecto entero a un estado anterior.

Cualquier tipo de archivo que se encuentre en un ordenador puede ponerse bajo control de versiones.


¿Para qué sirve Git?

Con Git se obtiene una mayor eficiencia usando archivos de texto plano(Markdown), ya que con archivos binarios no puede guardar solo los cambios, sino que debe volver a grabar el archivo completo ante cada modificación, por mínima que sea, lo que hace que incremente demasiado el tamaño del repositorio.

Caracteristicas de Git

Git almacena la información como un conjunto de archivos.

No existen cambios, corrupción en archivos o cualquier alteración sin que Git lo sepa.

Casi todo en Git es local. Es difícil que se necesiten recursos o información externos, basta con los recursos locales con los que cuenta.

Git cuenta con 3 estados en los que es posible localizar archivos: Staged, Modified y Committed.

Diferentes estados de un fichero Git:

Existen tres tipos de estado de un fichero Git:

Secciones principales de un proyecto Git
Confirmado: tenemos un fichero con el que hemos estado trabajando, hemos aprobado todos sus cambios y va en una nueva revisión, es decir, una especie de paquete dónde van todos los cambios.
Modificado: estamos trabajando en el directorio de trabajo (o working directory) y consideramos que ese cambio debe de ir en una revisión, en esa especie de paquete, para formar la revisión.
Preparado: hemos marcado un archivo para que vaya una revisión.

Fundamentalmente, un proyecto Git se estructura en tres partes o tres cajas:

El área del working directory, que es dónde vamos a tener todos nuestros ficheros, dónde estamos trabajando constantemente.
El staging area, que es donde van los archivos que estamos modificando y que aceptamos para que vayan en una futura revisión.
El área de commit o el git directory, que es dónde se almacenan la revisión completa. A lo largo de nuestro curso de Git, se explicará cómo podemos movernos a lo largo de esos tres estados, para qué sirven y por qué suponen una ventaja.

10 Comandos basicos de Git

1. Git clone
Git clone es un comando para descargar el código fuente existente desde un repositorio remoto (como Github, por ejemplo). En otras palabras, Git clone básicamente hace una copia idéntica de la última versión de un proyecto en un repositorio y la guarda en su computadora.

2. Git branch
Las ramas son muy importantes en el mundo de git. Mediante el uso de ramas, varios desarrolladores pueden trabajar en paralelo en el mismo proyecto simultáneamente. Se puede usar el comando git branch para crear, enumerar y eliminar ramas. 

3. Git checkout
Este es también uno de los comandos Git más utilizados. Para trabajar en una rama, primero debe cambiarse a ella. Git checkout se usa principalmente para cambiar de una rama a otra. También podemos usarlo para verificar archivos y confirmaciones.

4. Git status
El comando de estado de Git brinda toda la información necesaria sobre la rama actual.

git status
Puede recopilar información acerca de:  

Si la rama actual está actualizada.    
Si hay algo que necesita un commit, un add, o borrarse.  
Si hay archivos preparados, sin preparar o sin seguimiento    
Si hay archivos creados, modificados o eliminados

5. Git add
Cuando se crea, modifica o elimina un archivo, estos cambios ocurriren en el local y no se incluirán en la próxima confirmación (a menos que se cambien las configuraciones).

Se necesita usar el comando git add para incluir los cambios de un archivo(s) en nuestro próximo commit.

6. Git commit
Este es quizás el comando más utilizado de Git. Una vez que se llega a cierto punto en el desarrollo, queremos guardar nuestros cambios (tal vez después de una tarea o problema específico).

Git commit es como establecer un punto de control en el proceso de desarrollo al que puede volver más tarde si es necesario. También necesitamos escribir un mensaje corto para explicar lo que hemos desarrollado o cambiado en el código fuente.

git commit -m "commit message"
Importante: Git commit guarda tus cambios solo localmente.

7. Git push
Después de confirmar los cambios (con git commit), lo siguiente que hay que hacer es enviar estos cambios al servidor remoto. Git push sube tus confirmaciones al repositorio remoto.


8. Git pull
El comando git pull se usa para obtener actualizaciones del repositorio remoto. Este comando es una combinación de git fetch y git merge, lo que significa que, cuando se usa git pull, se obtienen las actualizaciones del repositorio remoto (git fetch) e inmediatamente aplica los últimos cambios en su local (git merge). (En simples palabras, sirve para traer el repositorio remoto a tu repositorio local).


9. Git revert
Este se utiliza para deshacer los cambios que hemos hecho. Hay varias formas de deshacer los cambios, de forma local o remota (depende de lo que necesitemos), pero se deben usar estos comandos con cuidado para evitar eliminaciones no deseadas.

10. Git merge
La herramienta git merge se utiliza para fusionar uno o más ramas dentro de la rama que tienes activa. 

Git merge básicamente integra su rama de características (feature branch) con todas sus confirmaciones en la rama dev (o master). Es importante recordar que primero se debe estar en la rama específica que se desea fusionar con la rama de características.

MARKDOWN

¿Qué es Markdown?

Markdown nació como herramienta de conversión de texto plano a HTML. Markdown es un lenguaje simple que se utiliza para crear texto enriquecido (por ejemplo, HTML) con un editor de texto sin formato. Te permite darle un formato básico al texto, utilizando símbolos conocidos y accesibles en todos los teclados.

¿Para qué sirve Markdown?

es un lenguaje de marcado sencillo que sirve para agregar formato, vínculos e imágenes con facilidad al texto simple. Este método te permitirá añadir formatos tales como negritas, cursivas o enlaces, utilizando simplemente texto plano, lo que hará de tu escritura algo más simple y eficiente al evitar distracciones.

