#Test Laravel 
###Creación de nuevo proyecto
Se creó la carpeta llamada test Laravel dentro de la carpeta de xampp, paso seguido se abrió la consola y se creó un nuevo proyecto en Laravel como se puede ver a continuación:

![](https://github.com/SLeonC05/Test-Laravel/blob/master/Img/img.PNG?raw=true)

Posteriormente luego de la descarga se abrió el editor de código y se puso a correr la terminal por medio del comando `php artisan serve`

![](https://github.com/SLeonC05/Test-Laravel/blob/master/Img/img2.PNG?raw=true)

Se ubicó la carpeta test, que contiene la carpeta feature y unit y los archivos de php createsApplication y testCase.

Posteriormente usamos el comando `./vendor/bin/phpunit` para la ejecución de pruebas unitarias 

El comando php artisan test nos muestra los métodos que han funcionado correctamente

![](https://github.com/SLeonC05/Test-Laravel/blob/master/Img/img3.PNG?raw=true)

Luego con el comando `php artisan make:test UserTest` se creó un archivo nuevo dentro de la capeta feature

Posteriormente verificamos que este nuevo archivo de test esté funcionando correctamente

Se abrió el archivo UserTest y se agrego la palabra “test” después del “/” 

![](https://github.com/SLeonC05/Test-Laravel/blob/master/Img/img4.PNG?raw=true)

Lo cual en el momento nos arroja un error al correr el comando el la terminal.

###Creando test unitarios 
Por medio del siguiente comando `php artisan make: test UserTest --unit`
 
Posteriormente se elimina la palabra “test”que se había agregado 

![](https://github.com/SLeonC05/Test-Laravel/blob/master/Img/Captura.PNG?raw=true)

Luego se vuelven a ejecutar las pruebas con el comando `php artisan test`
 

###Creando interfaces de usuario
Por medio del comando `composer require laravel/ui`

Posteriormente se crea una interfaz de autenticación reactiva, por medio del comando `php artisan ui react –auth`

Luego se instalan las dependencias por medio de los comandos `npm install && npm run dev `desde la consola

![](https://github.com/SLeonC05/Test-Laravel/blob/master/Img/img5.PNG?raw=true)

###Creando base de datos
Se ingresó a phpMyAdmin y se creó la base de datos llamada “testlaravel”
 
También se verifico en el archivo .env que el nombre de la base de datos sea el correcto

Posteriormente se realiza la migración a la base de datos por medio del comando php artisan migrate

Se ingresó al archivo UserTest de la carpeta Unit y se borró la función que se encontraba en él y se sustituyó por la siguiente:

![](https://github.com/SLeonC05/Test-Laravel/blob/master/Img/img6.PNG?raw=true)

También se modificó la ruta que tenía en la parte superior del archivo

![](https://github.com/SLeonC05/Test-Laravel/blob/master/Img/img8.PNG?raw=true)

Y se procedió a ejecutar las pruebas

También se añadió la función test_user_duplication la cual nos ayuda a que los datos de los usuarios no se repitan

![](https://github.com/SLeonC05/Test-Laravel/blob/master/Img/img7.PNG?raw=true)

Luego se realiza la prueba nuevamente con el comando `php artisan test`
 
