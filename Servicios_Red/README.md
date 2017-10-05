# Administración de un servidor DHCP
En esta práctica vamos a monitorizar un servicio DHCP en una máquina Windows Server 2012.

- Lo primero que debemos hacer es instalar el servicio DHCP.

![1](./img/1.png)

- Cuando termine la instalación ir a `Herramientas -> Servidor DHCP`

![2](./img/2.png)

- Creamos un nuevo ámbito e insertamos el rango de IPs que vamos a dar a los demás equipos.

![3](./img/3.png)

- Ahora vamos a agregar rangos de IP que no se vayan a colocar a los equipos ya que están reservados.

![3](./img/4.png)

- Tenemos que insertar una puerta de enlace que en este caso será `172.18.0.1`

![3](./img/5.png)

- Insertamos el DNS en su defecto `8.8.4.4`

![3](./img/6.png)

- Con el uĺtimo paso aceptamos y terminamos el primer ámbito.

![3](./img/7.png)

- Como método de análisis de IP, ejecutamos el comando `ipconfig`

![3](./img/8.png)

- Crearemos un segundo ámbito cuya información sea complementaria con el anterior.

![3](./img/9.png)

- En el paso anterior deberíamos insertar unas direcciones distintas por que nos pueden dar problemas. Aceptamos y creamos el segundo ámbito.

![3](./img/10.png)

- Como último paso, debemos crear un súper ámbito que una los dos ámbitos anteriores.

![3](./img/11.png)

- Aceptamos y ya tenemos nuestro súper ámbito.

![3](./img/12.png)
