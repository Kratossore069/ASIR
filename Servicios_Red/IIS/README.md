# Internet Information Server.

Empezaremos agregando roles de servidor para instalar **IIS**.

![](./img/1.png)

![](./img/2.png)

Una vez instalado el IIS, haremos una prueba de localhost para visualizar la página por defecto.

![](./img/3.png)

Hacemos una prueba desde la máquina cliente hasta la dirección IP del servidor y vemos que está operativa.

![](./img/4.png)

Podemos observar que, desde la máquina cliente, dirigiéndonos a **localhost** no entramos en la página. Esto es por que aún no está configurado de manera que el servidor no ofrece resolución de nombres.

![](./img/5.png)

Una vez hecho el paso anterior e interactuando con los archivos en **C:\\inetpub\wwwroot** hemos hecho un cambio en la página principal de nuestro archivo.

![](./img/6.png)

Crearemos una carpeta en este destino en el que irán imágenes y cambiaremos un poco la página como hemos visto antes.

![](./img/7.png)

Ahora crearemos un sitio web nuevo desde **Administrador de IIS**.

![](./img/8.png)

![](./img/9.png)

![](./img/10.png)

![](./img/11.png)

Podemos observar que la página creada anteriormente funciona.

![](./img/12.png)

En la siguiente imagen podemos obervar la ruta en la que está registrado nuestro sitio web.

![](./img/13.png)

Ahora procederemos a crear un subdominio.

![](./img/14.png)

![](./img/15.png)
