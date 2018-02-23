# Instalación y configuración de un servidor multimedia - Smooth Streaming

MV: **Windows12Server**

En esta práctica vamos a instalar un servicio multimedia de streaming.

## Servicios de multimedia 4.1 de IIS.

Lo primero que debemos hacer es instalar los servicios de IIS.

![](./img/13.png)

## Smooth Streaming Player

Vamos al moodle del instituto y descargamos de ahí el programa.

![](./img/14.png)

Nos queda un archivo en el escritorio.

![](./img/15.png)

Nos quedan estos archivos.

![](./img/16.png)

En esos archivos hay un HTML que es necesario configurar para la transmisión del vídeo que deseamos.

![](./img/17.png)

![](./img/18.png)

Necesitamos copiar los archivos que hemos visto antes y copiarlos en el DNS que tenemos que crear para nuestro servicio multimedia.

![](./img/19.png)

Debemos descargar los vídeos de la práctica.

![](./img/20.png)

Creamos dos sitios web en el IIS de elefante y conejo.

![](./img/21.png)

![](./img/22.png)

Cambiamos el archivo HTML de uno de los vídeos para que salga nuestro archivo especificado. Antes de esto, hemos copiado y pegado los archivos del media player en las carpetas convenientes.

![](./img/23.png)

## Expression Encoder

Vamos a instalar el servicio llamado Expression Encoder para usar sus preferencias.

![](./img/1.png)

![](./img/2.png)

## IIS Media

Nuestro siguiente paso serái ir a la página oficial de IIS para descargarnos el programa que también nos servirá para nuestro proyecto. https://www.iis.net/downloads/category/serve-media

![](./img/3.png)

Usaremos este programa.

![](./img/4.png)

Bajamos en la página e instalamos x64 ó x86 según nuestro ordenador.

![](./img/5.png)

## Microsoft Silverlight

Para poder usar estas herramientas debemos instalar el Microsoft Silverlight. https://www.microsoft.com/getsilverlight/get-started/install/default?reason=unsupportedbrowser&_helpmsg=FirefoxObsoleteForSL#sysreq

![](./img/8.png)

![](./img/9.png)

![](./img/10.png)

## Volviendo al IIS.

Entramos en el IIS y vemos que se han añadido programas.

![](./img/11.png)

Podemos ver sus características y opciones.

![](./img/12.png)
