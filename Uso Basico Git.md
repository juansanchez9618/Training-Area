---


---

<h1 id="manual-de-uso-basico-de-git">Manual de uso Basico de Git</h1>
<p><strong>Índice</strong></p>
<ol>
<li><a href="#id1">Clonar repositorio</a></li>
<li><a href="#id2">Subir un cambio con Git</a></li>
<li><a href="#id3">Como Hacer un Merge</a></li>
<li><a href="#id4">Como subir los cambios a un repositorio en la nube</a></li>
</ol>
<p>En este manual encontraran los aspectos basicos para iniciar el uso de Git</p>
<h2 id="clonar-repositorioa-nameid1a">Clonar repositorio<a></a></h2>
<ul>
<li><strong>Paso 1</strong></li>
</ul>
<p>Se necesita la URL del repositorio que se desea clonar</p>
<ul>
<li><strong>Paso 2</strong></li>
</ul>
<p>Creamos una carpeta que será donde copiará el repositorio</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Clonar1.png" alt="Clonar   repositorio 1"></p>
<ul>
<li>
<p><strong>Paso 3</strong><br>
Copiamos la URL donde está alojado el repositorio</p>
<pre><code>         En ejemplo será uno  en Github
</code></pre>
</li>
</ul>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Clonar2.png" alt="Clonar   repositorio 2"></p>
<ul>
<li><strong>Paso 4</strong></li>
</ul>
<p>Damos Clic derecho en la carpeta creada y seleccionamos la opción <strong>Git Bash Here</strong></p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Clonar3.png" alt="Clonar   repositorio 3"></p>
<p>Nos abrirá el editor de Git<br>
<img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Clonar4.png" alt="Clonar   repositorio 4"></p>
<ul>
<li><strong>Paso  5</strong></li>
</ul>
<p>Usamos el comando:</p>
<p><strong>Git clone</strong> y la URL del repositorio</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Clonar5.png" alt="Clonar   repositorio 5"></p>
<p>Cargara la información del repositorio</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Clonar6.png" alt="Clonar   repositorio 6"></p>
<ul>
<li><strong>Paso 6</strong><br>
En la carpeta creada veremos los archivos descargados localmente del repositorio</li>
</ul>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Clonar7.png" alt="Clonar   repositorio 7"></p>
<p>De esta forma quedaran los archivos guardados localmente para hacer uso de ellos.</p>
<h2 id="subir-un-cambio-con-gita-nameid2a">Subir un cambio con Git<a></a></h2>
<ul>
<li><strong>Paso 1</strong><br>
Abrimos el proyecto</li>
</ul>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Cambio1.png" alt="Cambios 1"></p>
<p>Iniciamos el proyecto con</p>
<p><strong>Git init</strong></p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Cambio2.png" alt="Cambios 2"></p>
<ul>
<li><strong>Paso 2</strong></li>
</ul>
<p>Realizamos los cambios o modificaciones en el proyecto</p>
<p>Al visualizar el explorador de soluciones tenemos cambios que no se han agregado</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Cambio3.png" alt="Cambios 3"></p>
<ul>
<li><strong>Paso 3</strong></li>
</ul>
<p>Usamos el comando <strong>git status</strong></p>
<p>Para validar que elementos nuevos encuentra</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Cambio4.png" alt="Cambios 4"></p>
<p>Se veran resaltados en rojo las modificaciones o archivos nuevos que encuentra pero no se han guardado.</p>
<ul>
<li><strong>Paso 4</strong></li>
</ul>
<p>Agregamos los archivos para subir repositorio con el comando <strong>git add -A</strong></p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Cambio5.png" alt="Cambios 5"></p>
<p>Usamos el comando <strong>git status</strong></p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Cambio6.png" alt="Cambios 6"></p>
<p>Se veran reflejados los cambios listos para agregarlos al repositorio.</p>
<ul>
<li><strong>Paso 5</strong></li>
</ul>
<p>Para subir los cambios usaremos el comados <strong>git commit -m "Descripción"</strong></p>
<p>En la descripción debemos especificar que cambios se estan subiendo</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Cambio7.png" alt="Cambios 7"></p>
<p>Validaremos en el explorador de soluciones que el cambio se realizo correctamente</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/Cambio8.png" alt="Cambios 8"></p>
<p>De esta forma tendremos el cambio o modificación guardado en el repositorio localmente.</p>
<h2 id="como-hacer-un-mergea-nameid3a">Como Hacer un Merge<a></a></h2>
<ul>
<li><strong>Paso 1</strong></li>
</ul>
<p>Iniciamos el proyecto usando el comando <strong>git init</strong></p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/merge1.png" alt="merge 1"></p>
<ul>
<li><strong>Paso 2</strong></li>
</ul>
<p>Debemos crear una rama que será donde realicemos los cambios para luego realizar el merge a la rama principal llamada <strong>Master</strong></p>
<p>Usamos el comando <strong>git branch "nombre"</strong></p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/merge2.png" alt="merge 2"></p>
<ul>
<li><strong>Paso 3</strong></li>
</ul>
<p>Despues de crear la nueva rama, vamos a posicionarnos en ella</p>
<p>Usamos el comando <strong>git checkout "nombre de la rama"</strong></p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/merge3.png" alt="merge 3"></p>
<p>En la ruta veremos que estamos en la rama <strong>pruebamerge</strong> o usamos el comando <strong>git branch</strong></p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/merge4.png" alt="merge 4"></p>
<p>En verde nos resaltara la rama donde estamos posicionados.</p>
<ul>
<li><strong>Paso 4</strong></li>
</ul>
<p>Una vez hecho esto procedemos a realizar nuestros cambios o modificaciones en algún archivo del repositorio o crear uno nuevo.</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/merge5.png" alt="merge 5"></p>
<ul>
<li><strong>Paso 5</strong></li>
</ul>
<p>Con los cambios realizados los alistaremos para agregarlos al repositorio</p>
<p>Usamos el comando <strong>git add -A</strong></p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/merge6.png" alt="merge 6"></p>
<p>A continuación cargaremos los cambios al repositorio en la rama creada</p>
<p>Usamos el comando <strong>git commit -m "Descripción"</strong></p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/merge7.png" alt="merge 7"></p>
<p>Despues de haber realizado el commit, volveremos a la rama <strong>Master</strong> para unificar los cambios</p>
<ul>
<li><strong>Paso 6</strong></li>
</ul>
<p>Usamos el comando <strong>git checkout master</strong> para volver a la rama principal</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/merge8.png" alt="merge 8"></p>
<p>Estando en la rama principal usamos el comado <strong>git merge pruebamerge</strong> para realizar la union.</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/merge9.png" alt="merge 9"></p>
<p>veremos los cambios guardados en la rama principal.</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/merge10.png" alt="merge 10"></p>
<h2 id="como-subir-los-cambios-a-un-repositorio-en-la-nubea-nameid4a">Como subir los cambios a un repositorio en la nube<a></a></h2>
<p>Debemos tener un repositorio en la nube donde haremos el push</p>
<ul>
<li><strong>Paso 1</strong></li>
</ul>
<p>Iniciar el proyecto</p>
<p>Usamos el comandos <strong>Git init</strong></p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/merge1.png" alt="push 1"></p>
<ul>
<li><strong>Paso 2</strong></li>
</ul>
<p>Debemos tener commits realizados</p>
<p>Para subir los cambios, primero debemo crear una conexión con el repositorio</p>
<p>Usamos el comandos <strong>git remote add origin <a href="https://github.com/juansanchez9618/Prueba-TP.git">https://github.com/juansanchez9618/Prueba-TP.git</a></strong></p>
<p>Es necesario la URL donde esta esta el repositorio en la nube, en este ejemplo utilizaremos uno de prueba</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/push2.png" alt="push 2"></p>
<ul>
<li><strong>Paso 3</strong></li>
</ul>
<p>Ya tenemos la union al repositorio, ahora solicitaremos subir los cambios a dicho repositorio.</p>
<p>Usamos el comandos <strong>git push -u origin master</strong></p>
<p>La primera vez nos solicitara las credenciales del repositorio.</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/push6.png" alt="push 3"></p>
<p>Despues de confirmar las credenciales empezara a subir la información al repositorio.</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/push4.png" alt="push 4"></p>
<p>Una vez finalice podemos validar en github o donde tengamos el repositorio que ya estan los cambios.</p>
<p><img src="https://raw.githubusercontent.com/juansanchez9618/Training-Area/master/Capturas/push5.png" alt="push 5"></p>
<ul>
<li><strong>Paso 4</strong></li>
</ul>
<p>Ya como tenemos la conexión del repositorio local con github cuando tengamos cambios que subir.</p>
<p>Usamos el comando <strong>git push</strong></p>
<hr>

