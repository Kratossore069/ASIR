# IIS Avanzada

El primer paso es ir a la configuración de nuestra IIS en Windows 2012 Server y agregar un sitio web nuevo.

![](./img/5.png)

Una vez completado, tendremos el sitio de nuestra página web.

![](./img/6.png)

En **Documento predeterminado** eliminamos todos los archivos por defecto para crear el nuestro.

![](./img/7.png)

![](./img/8.png)

Una vez hecho lo anterior podemos observar que tenemos una carpeta con nuestra configuración guardada.

![](./img/1.png)

Yendo a **DNS** podemos resolver nombres para que nuestra página web aparezca con un nombre en vez de con una dirección IP.

![](./img/2.png)

Creamos un archivo AAA para constar nuestro sitio.

![](./img/3.png)

Igualmente creamos otro archivo CNAME con la dirección de nuestro sitio web.

![](./img/4.png)

A continuación, necesitamos firmas SSL. Para ello, vamos a descargarnos de Internet una herramienta sencilla que más tarde usaremos en nuestro sitio web.

![](./img/9.png)

Una vez descargado procedemos a instalarlo.

![](./img/10.png)

Una vez instalado, volvemos a nuestra página en el IIS y **Configuración de SSL**.

![](./img/11.png)

En la siguiente pantalla insertamos nuestro SSL ya creado anteriormente y listo.

![](./img/12.png)
