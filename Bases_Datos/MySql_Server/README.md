## INSTALACIÓN DE MYSQL COMMUNITY SOBRE WINDOWS

- Comenzaremos instalando el MySL Community en modo Developer en nuestra MV con Windows 7

![1](./img/img1.PNG)

- Lo descargaremos de la página oficial. En este momento pueden surgir algunos problemas con paquetes adicionales que debemos descargar a parte para que todo funcione a la perfección.

![1](./img/img2.PNG)

- En la imagen de arriba podemos observar una página que nos servirá para instalar el Visual C++ que se consigue de esta página https://support.microsoft.com/en-us/help/3179560/update-for-visual-c-2013-and-visual-c-redistributable-package

![1](./img/img3.PNG)

- Otro paquete que deberemos instalarnos será el .NET Framework que lo buscaremos también en la página oficial. https://www.microsoft.com/es-es/download/details.aspx?id=17851

![1](./img/img4.PNG)

- Y lo instalamos.

![1](./img/img5.PNG)

- También existe la probabilidad de que se necesite instalar el Python para continuar con la instalación óptima del MySQL.

![1](./img/img7.PNG)

- Una vez instalado esto último podemos comenzar con la instalación del MySQL.

![1](./img/img10.PNG)

- `Es importante para esta práctica ponerlo en "Developer"`

![1](./img/img6.PNG)

![1](./img/img8.PNG)

- `Esta ventana de aquí arriba es importante por que hay que chequear todas las celdas que hay debido a que no debe fallar nada`.

![1](./img/img9.PNG)

- `La segunda ventana es similar a la anterior. Hay que probar e instalar todos los componentes.`

Una vez instalado el programa saldrá en la barra de `Inicio` un archivo donde tenemos instalado el MySQL llamado `MySQL Server → Command Line Client`. Esta será la ventana donde nosotros trabajaremos.

![1](./img/img12.PNG)

- Accediendo a la ventana `Servicios` a partir del menú `Inicio` podemos observar que nuestro MySQL está habilitado.

![1](./img/img11.PNG)

- Los archivos se encuentran en la carpeta `AppData` de nuestro ordenador.

![1](./img/mysql2.PNG)

- Instalamos el `MySQL WorkBench` en el cliente.

![1](./img/mysql4.PNG)

- Ahora procederemos a instalar el `XAMPP` para relacionar el servidor con el cliente.

![1](./img/img13.PNG)

- En este paso intentaremos entrar en phpMyadmin pero tendremos un error así que hay que configurar como en el ejemplo de la página https://tech.enekochan.com/es/2015/02/06/solucionar-configuration-pmadb-not-ok-en-phpmyadmin/  un archivo dentro de xampp llamado `config.inc.php`

![1](./img/img14.PNG)
