# Creación de servidor web.

En nuestra máquina virtual **Windows 2012 Server** vamos a instalar los elementos necesarios para hacer de ella un servicio de hosting hecho a mano.

php 5.3.9 nts x86.msi

mysql 5.7.20.msi

phpmyadmin 4.0.10.20.zip

**PHP - Instalación**

*http://windows.php.net/downloads/releases/archives/*

![](./img/1.png)

*Es importante descargarse la versión nts.*

![](./img/2.png)

![](./img/3.png)

![](./img/4.png)

![](./img/5.png)

*En este momento hay un fallo por que debemos configurar el CGI de la siguiente manera.*

![](./img/6.png)

*Volvemos a la instalación normal.*

![](./img/7.png)

![](./img/8.png)

**Alojamos el PHP en nuestro servidor.**

No vamos a necesitar instalar IIS ya que en **Windows 2012 Server** con ir a `Agregar roles y servicios -> IIS` ya lo instalamos.

Nos creamos un sitio.

![](./img/9.png)

![](./img/10.png)

Vamos a DNS.

![](./img/11.png)

![](./img/12.png)

![](./img/13.png)

![](./img/14.png)

![](./img/15.png)

![](./img/16.png)

![](./img/17.png)

![](./img/18.png)

Hecho esto no nos aparecerá nuestro sitio web. Debemos ir a **cmd** e insertar este comando.

![](./img/19.png)

Vamos a nuestra carpeta en la que está alojado nuestro sitio web.

![](./img/20.png)

Vemos que funciona cuando accedemos a un navegador.

![](./img/21.png)

**Instalación de MySQL**

Es importante instalar primero **.NET Framework 4.0**.

![](./img/22.png)

![](./img/23.png)

![](./img/24.png)

![](./img/25.png)

**Instalación de PHPMyAdmin**

![](./img/26.png)

Una vez descargado debemos crear un nuevo sitio específico para PHPMyAdmin.

![](./img/27.png)

![](./img/28.png)

*Copiamos y pegamos el fichero de phpmyadmin en esta carpeta.*

![](./img/29.png)
