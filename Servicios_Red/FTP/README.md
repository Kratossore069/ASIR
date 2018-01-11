# FTP

*En esta práctica vamos a configurar el servicio FTP tanto en Windows Server como en Linux.*

## Windows - MV Windows12Server

Procederemos a instalar el FTP con IIS.



## Linux - MV UbuntuServer

Instalamos el **vsftpd**.

![](./img/1.png)

El fichero de configuración está en **/etc**.

![](./img/2.png)

Ahora, crearemos un nuevo usuario de FTP.

![](./img/3.png)

Le proporcionamos una clave.

![](./img/4.png)

A continuación, unos ejemplos de comandos de FTP en Linux.

![](./img/5.png)

![](./img/6.png)

El archivo `/etc/ftpusers` contiene una lista de los usuarios del sistema a los que se deniega el acceso mediante ftp.

![](./img/7.png)

El archivo `/var/log/vsftpd.log` registra la información sobre las conexiones ftp establecidas.

Ahora vamos a:

#### Enjaular usuarios

Hacemos una copia de seguridad del fichero de configuración.

![](./img/8.png)

Ahora vamos a `/etc/vsftpd.conf` y añadimos la siguiente configuración al final del archivo.

![](./img/9.png)

A continuación, creamos el fichero siguiente y ponemos nuestro usuario para que quede enjaulado.

![](./img/10.png)

Reiniciamos el servicio.

![](./img/11.png)

Ya tendríamos nuestro usuario registrado.

#### Usuarios anónimos.

Si se realiza una conexión anónima, se tiene acceso a la carpeta `/srv/ftp` que será compartida para todos los accesos anónimos.

Creamos un fichero en esta carpeta.

![](./img/12.png)

Editamos el archivo de configuración para permitir el acceso a usuarios anónimos.

![](./img/13.png)

Reiniciamos el servicio y listo.

![](./img/14.png)
