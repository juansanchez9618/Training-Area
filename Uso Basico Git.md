#                Manual de uso Basico de Git


**Índice**   
1. [Clonar Repositorio](#Clonar-Repositorio)
2. [Subir un cambio con Git](#Subir-un-cambio-con-Git)
3. [Como Hacer un Merge](#Como-Hacer-un-Merge)
4. [Como subir los cambios a un repositorio en la nube](#Como-subir-los-cambios-a-un-repositorio-en-la-nube)








En este manual encontraran los aspectos básicos para iniciar el uso de Git.



## Clonar Repositorio

+ **Paso 1**

Se necesita la URL del repositorio que se desea clonar.

+ **Paso 2**

Creamos una carpeta que será donde copiará el repositorio.

![Clonar   repositorio 1](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Clonar1.png)

+ **Paso 3** 
Copiamos la URL donde está alojado el repositorio.

               En ejemplo será uno  en Github

![Clonar   repositorio 2](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Clonar2.png)


+ **Paso 4**

Damos Clic derecho en la carpeta creada y seleccionamos la opción **Git Bash Here**

![Clonar   repositorio 3](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Clonar3.png)


Nos abrirá el editor de Git. 

![Clonar   repositorio 4](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Clonar4.png)


+ **Paso  5**

Usamos el comando:

**Git clone** y la URL del repositorio.

![Clonar   repositorio 5](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Clonar5.png)

Cargara la información del repositorio.

![Clonar   repositorio 6](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Clonar6.png)


+ **Paso 6**
En la carpeta creada veremos los archivos descargados localmente del repositorio.

![Clonar   repositorio 7](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Clonar7.png)


De esta forma quedaran los archivos guardados localmente para hacer uso de ellos.



## Subir un cambio con Git

+ **Paso 1**
Abrimos el proyecto. 

![Cambios 1](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Cambio1.png)

Iniciamos el proyecto con

 **Git init**

![Cambios 2](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Cambio2.png)

+ **Paso 2**


Realizamos los cambios o modificaciones en el proyecto.

Al visualizar el explorador de soluciones tenemos cambios que no se han agregado.


![Cambios 3](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Cambio3.png)


+ **Paso 3**

Usamos el comando **git status**

Para validar que elementos nuevos encuentra. 

![Cambios 4](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Cambio4.png)

Se veran resaltados en rojo las modificaciones o archivos nuevos que encuentra pero no se han guardado.

+ **Paso 4**

Agregamos los archivos para subir repositorio con el comando **git add -A**

![Cambios 5](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Cambio5.png)

Usamos el comando **git status**

![Cambios 6](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Cambio6.png)

Se verán reflejados los cambios listos para agregarlos al repositorio.

+ **Paso 5**

Para subir los cambios usaremos el comado **git commit -m "Descripción"**

En la descripción debemos especificar que cambios se están subiendo.

![Cambios 7](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Cambio7.png)


Validaremos en el explorador de soluciones que el cambio se realizo correctamente. 


![Cambios 8](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/Cambio8.png)

De esta forma tendremos el cambio o modificación guardado en el repositorio localmente.






## Como Hacer un Merge


+ **Paso 1**

Iniciamos el proyecto usando el comando **git init**

![merge 1](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/merge1.png)




+ **Paso 2**

Debemos crear una rama que será donde realicemos los cambios para luego realizar el merge a la rama principal llamada **Master**

Usamos el comando **git branch "nombre"**

![merge 2](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/merge2.png)


+ **Paso 3**

Después de crear la nueva rama, vamos a posicionarnos en ella.


Usamos el comando **git checkout "nombre de la rama"**

![merge 3](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/merge3.png)

En la ruta veremos que estamos en la rama **pruebamerge** o usamos el comando **git branch**


![merge 4](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/merge4.png)

En verde nos resaltara la rama donde estamos posicionados.


+ **Paso 4**

Una vez hecho esto procedemos a realizar nuestros cambios o modificaciones en algún archivo del repositorio o crear uno nuevo.

![merge 5](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/merge5.png)
+ **Paso 5**

Con los cambios realizados los preparamos para agregarlos al repositorio.

Usamos el comando **git add -A**

![merge 6](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/merge6.png)
A continuación cargaremos los cambios al repositorio en la rama creada

Usamos el comando **git commit -m "Descripción"**

![merge 7](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/merge7.png)

Después de haber realizado el commit, volveremos a la rama **Master** para unificar los cambios.

+ **Paso 6**

Usamos el comando **git checkout master** para volver a la rama principal.

![merge 8](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/merge8.png)

Estando en la rama principal usamos el comando **git merge pruebamerge** para realizar la unión.


![merge 9](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/merge9.png)

veremos los cambios guardados en la rama principal.

![merge 10](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/merge10.png)




## Como subir los cambios a un repositorio en la nube

Debemos tener un repositorio en la nube donde haremos el push.

+ **Paso 1**

Iniciar el proyecto.


Usamos el comando **Git init**

![push 1](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/merge1.png)

+ **Paso 2**

Debemos tener commits realizados.

Para subir los cambios, primero debemos crear una conexión con el repositorio.

Usamos el comandos **git remote add origin https://github.com/juansanchez9618/Prueba-TP.git**

Es necesario la URL donde esta esta el repositorio en la nube, en este ejemplo utilizaremos uno de prueba.

![push 2](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/push2.png)

+ **Paso 3**

Ya tenemos la unión al repositorio, ahora solicitaremos subir los cambios a dicho repositorio.

Usamos el comando **git push -u origin master**

La primera vez nos solicitara las credenciales del repositorio.


![push 3](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/push6.png)



Después de confirmar las credenciales empezara a subir la información al repositorio.


![push 4](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/push4.png)


Una vez finalice podemos validar en github o donde tengamos el repositorio que ya están los cambios.

![push 5](https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Material/Capturas/push5.png)


+ **Paso 4**

Ya como tenemos la conexión del repositorio local con github cuando tengamos cambios que subir.

Usamos el comando **git push**

____________________

