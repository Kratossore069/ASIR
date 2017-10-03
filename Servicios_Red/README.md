# Administración de un servidor DHCP
En esta práctica vamos a monitorizar un servicio DHCP en una máquina Windows Server 2012.

- Lo primero que debemos hacer es instalar el servicio DHCP.

![1](./img/1.png)

- Cuando termine la instalación ir a `Herramientas -> Servidor DHCP`

![2](./img/2.png)

- Creamos un nuevo ámbito e insertamos el rango de IPs que vamos a dar a los demás equipos.

![3](./img/3.png)

- En la imagen de arriba ponemos como primera la dirección IP de nuestra propia máquina hasta un número no muy alto como prueba de que funciona el servicio DHCP. Agregamos exclusiones a nuestro DHCP. Son direcciones que no tomarán los nuevos equipos. 

![4](./img/4.png)

- Ponemos una puerta de enlace para nuestras conexiones.

![5](./img/5.png)

- También tenemos que configurar el DNS.

![5](./img/6.png)

- Ya tenemos creado el primer ámbito con el DHCP configurado.

![5](./img/7.png)

- La siguiente imagen es de la máquina cliente que podemos observar que haciendo un `ipconfig` la dirección IP del cliente cambia.

![5](./img/8.png)

- A continuación, crearemos otro ámbito. Lo haremos con unas credenciales y una información parecida a la anterior.

![5](./img/9.png)
