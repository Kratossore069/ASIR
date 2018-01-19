# Servicio de Correo Electrónico

*En esta práctica vamos a configurar un servicio de email.*

Máquina virtual a usar: Windows12Server

## Instalando SMTP

Vamos a `Agregar roles y características` y lo instalamos desde ahí.

![](./img/1.png)

Habiéndolo instalado ahora vamos a configurarlo. Buscamos *IIS* en nuestro PC y nos llevará a esta ventana.

![](./img/2.png)

![](./img/3.png)

Configuramos como en la imagen de manera que establecemos la dirección IP de nuestra máquina a la dirección del servidor.

![](./img/4.png)

Pulsamos en `Acceso` y seguimos los pasos `Conexión` -> `Solo la lista a continuación` -> `Añadir` -> Establecemos la IP que deseemos. Esto sirve para limitar el acceso solo a mi ordenador.

![](./img/5.png)

Vamos a establecer un dominio externo. Si no queremos hacerlo lo dejamos como está. Pulsamos en `Entrega`.

![](./img/6.png)

Ahora establecemos algunas opciones en el cortafuegos. Hacemos una búsqueda de `Firewall`.

![](./img/7.png)

![](./img/8.png)

Por último le añadimos un nombre a la regla.

![](./img/9.png)

Cerramos el cortafuegos, reiniciamos y vamos a `Servicios` -> `Protocolo simple de transferencia` -> `Botón derecho y propiedades.`

![](./img/13.png)

Detenemos e iniciamos el servicio y le pulsamos en automático y ya tenemos nuestro servicio SMTP listo.

![](./img/14.png)

## Probar el servicio.

Una vez instalado el SMTP vamos a probar cómo funciona el servicio de correo. Para ello, he descargado el `Mozilla Thunderbird` que es un servicio de mensajería.

![](./img/15.png)

En nuestro correo le damos botón derecho y observamos nuestro servidor de salida.

![](./img/16.png)

![](./img/17.png)

Probaremos a enviar un mensaje a ver si funcionan todas nuestras configuraciones.

![](./img/18.png)

![](./img/19.png)

Y vemos que el mensaje llega.

![](./img/20.png)
