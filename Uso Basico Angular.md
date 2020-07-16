#                Manual de uso B�sico de Node JS y Angular


## Como abrir y compilar el proyecto desde el Backend 

 + **Paso 1** 

Descargar repositorio donde está alojado el proyecto.

Imagen 1


Una vez con el repositorio guardado localmente procedemos con el inicio del proyecto.

+ **Paso 2**

**Nota** debemos estar en la ruta donde está la carpeta back-end

Imagen 2

Usar el comando cd y la carpeta a acceder que será back-end.


 + **Paso 3**

Descargar e Instalar librerías para la compilación del mismo , para ello usar el comando **npm i o npm install**

Imagen 3

Se mostrara los paquetes cargados.

Imagen 4

Debe aparecer un nuevo archivo llamado **node_modules** allí estarán las librerías descargadas. 

Imagen 5

Una vez termine de correr el comando estará listo el proyecto para su uso.

+ **Paso 5**

**Nota**: validar que en la carpeta back-end este el archivo .env ya que es el que contiene las rutas y usuarios de acceso necesarios para el proyecto.

IMagen 6

Usar el comando **node index.js** para compilar el proyecto, este deberá generar los datos de compilación en el respectivo puerto junto con la fecha y hora.


Imagen 7

Validar el acceso en el navegador, para ello desde cualquier navegador acceder a **localhost:4200** que es donde está alojado el proyecto.

Al acceder si todo funcionó correctamente nos debe aparecer el Log in.

De momento no va a funcionar el Log in ya que hace falta compilar el front.

Imagen 11

___ 



## Como abrir y compilar el proyecto desde el front


 + **Paso 1** 

Iniciar el proyecto en el front.

Ubicar la ruta donde está el front. 

IMagen 8


También es necesario descargar e instalar las librerías necesarias 

Usar el comando **nmp i** 

Imagen 9

Paso 2

Ahora para compilar el proyecto en el front usar el comando **nmp run ng serve**

IMagen 10


Deberá mostrar el mensaje **Compiled Successfully** donde confirma la compilación del front

Ahora que ya esta el back y el front compilados se tendra disponible el acceso al proyecto DisDev

Imagen 12

Usar las credenciales de CCMS

IMagen 13



Con los pasos anteriormente indicados se obtendrá la visibilidad del proyecto junto con algunas opciones de consultar SQL editar agregar y eliminar registros.



____


## Crear un Componente 


+ **Paso 1**


Para crear un componente es necesario estar en la ruta container dentro del front.

Imagen 14


+ **Paso 2**

Para crear un nuevo componente se necesita el comando npm run ng g c "nombre del componente" --skiptests

IMagen 15

Validar que se creó el componente dentro de la carpeta container.

Imagen 16

Adicional también se cargara  en la sección app.modules.ts quedando listo para ser usado en el proyecto.


+ **Paso 3**

Crear el contenido del componente, en este caso será un botón como ejemplo.

IMagen 17


Al momento de guardar se volverá a compilar , quedando el cambio en el front, ya con esto guardado debemos aplicar el cambio al back-end para que pueda ser un componente visible y usable.


 + **Paso 4**

Es necesario indicar donde debe mostrar el componente creado para ello ir al archivo **app-routing.module.ts**
Imagen 18

En este se le dirá que componente debe mostrar, en este momento se encuentra en *container/main* 

Imagen 19

Imagen 20

+ **Paso 5**


Ahora se añadirá otro hijo que llamara al componente que se ha creado.

      {
        path: 'trainingtest',  ----> "será el nombre"
        component:TrainingtestComponent,, ----> "Sera el componente que se ha creado"
        canActivate: [ValidateLoginGuard]
      },


Adicional se evidencia que se importó el componente.

Imagen 22


Ahora al guardar  automáticamente  volverá a compilar el proyecto.


Imagen 23