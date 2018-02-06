# Instalación y Configuración de un Servidor de Correo en Linux

Vamos a proceder a crear un servidor de correo como hicimos en Windows pero esta vez en Linux.

Máquinas a usar: **UbuntuCliente**

## Servicio de correo electrónico junto con SquirrelMail.

Primero debemos instalar el servicio apache para nuestra práctica.

![](./img/8.png)

Ahora tenemos que instalar el servidor DNS para luego configurarlo.

![](./img/9.png)

Configuramos el DNS.

![](./img/10.png)

Debemos crear un archivo para nuestro proyecto con el nombre dado anteriormente.

![](./img/11.png)

Insertamos valores en este archivo.

![](./img/12.png)

Reiniciamos el demonio para efectuar los cambios.

![](./img/13.png)

Ahora necesitamos un servicio de correo. *sudo apt-get install postfix* Y lo tomamos como **Sitio de Internet**. Además, le ponemos el nombre de nuestra página de correo.

![](./img/14.png)

Configuramos el siguiente archivo en la siguiente ruta para nuestro Postfix.

![](./img/15.png)

Reiniciamos el demonio de Postfix.

![](./img/16.png)

Procedemos a instalar un servidor de correo electrónico o mail. *sudo apt-get install courier-pop*. En la siguiente ventana le decimos que *No*.

![](./img/17.png)

Instalamos el courier-imap.

![](./img/18.png)

Ahora debemos instalar un mailx para enviar y recibir correo electrónico mediante la línea de comandos.

![](./img/19.png)

Instalamos una aplicación webmail como SquirrelMail.

![](./img/20.png)

Ahora lo configuramos yendo a **sudo squirrelmail-configure**. Nos saldrá una pantalla en la que debemos escribir **D e Intro** para avanzar y nos saldrá esta paǵina.

![](./img/21.png)

Escribimos **courier**.

![](./img/22.png)

Pulsamos **2 e Intro.**

![](./img/23.png)

Pulsamos **1 e Intro** dos veces e insertamos nuestro dominio de correo. Hecho esto pulsamos **Q** y **Enter** junto con **Y** para salvar los cambios.

![](./img/24.png)

Hacemos un enlace simbólico.

![](./img/25.png)

Reiniciamos el demonio.

![](./img/26.png)

Ahora accedemos a la url **www.correoweb.com/webmail** y ya tenemos nuestro correo instalado.

Y ya tenemos todo listo para enviar y recibir correos.
