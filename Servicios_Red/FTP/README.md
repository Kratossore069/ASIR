# FTP

*En esta práctica vamos a configurar el servicio FTP tanto en Windows Server como en Linux.*

## Windows - MV Windows12Server

Procederemos a instalar el FTP con IIS.

Vamos a `Agregar roles y características`.

![](./img/a.png)

![](./img/b.png)

Después de instalarlo, vamos a IIS y seguimos estos pasos.

![](./img/c.png)

![](./img/d.png)

![](./img/e.png)

*En el paso siguiente hay que estar seguro de que existe la configuración correcta en el DNS.*

![](./img/f.png)

En la siguiente imagen se tilda la opción `Básica` por que interesa que los usuarios se conecten con su usuario y contraseña y no de manera anónima.

![](./img/g.png)

Ahora vamos a **configurar los valores predeterminados de FTP**.

![](./img/h.png)

En el panel de `Acciones` pulsamos en `Establecer valores predeterminados`.

![](./img/i.png)

Establecemos un usuario para conectarnos.

![](./img/j.png)

![](./img/k.png)

![](./img/l.png)

Ahora vamos a **configurar la compatibilidad con el firewall de FTP**. Para ello, volvemos al IIS.

![](./img/m.png)

![](./img/n.png)

Accedemos a `Compatibilidad con el firewall`.

Usamos el intervalo 0-0 para usar los puertos predeterminados y la IP del firewall externo de Windows.

![](./img/ñ.png)

#### Configuramos el aislamiento de usuario.

Volvemos al IIS. Configuramos los usuarios.

![](./img/o.png)

#### Configurar las opciones de exploración de directorios.

`Filtrado de solicitudes`.

![](./img/p.png)

![](./img/registro1.png)

![](./img/registro2.png)

![](./img/mensajes1.png)

![](./img/mensajes2.png)

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
