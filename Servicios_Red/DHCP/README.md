# Configuración de DHCP en Linux

En este informe vamos a instalar y configurar un servicio DHCP en un sistema operativo Linux Ubuntu.

- Lo primero que haremos será ir a nuestra terminal y ejecutar el comando `sudo apt-get install isc-dhcp-server`

![1](./img/1.png)

- Antes de continuar con el DHCP, debemos ir a nuestra configuración de red y poner una IP estática. `/etc/network/interfaces`

![4](./img/7.png)

- Podemos reiniciar aunque también podemos usar un comando para reiniciar la conexión desde la terminal `sudo /etc/init.d/networking restart`

![5](./img/8.png)

- Una vez terminadas las configuraciones iremos a `/etc/dhcp/dhcpd.conf`

![2](./img/2.png)

- Entramos en ese archivo e insertamos la información de nuestra IP,  máscara y el rango de IPs que va a escoger para los equipos.

![3](./img/3.png)

- Existe la posibilidad de que, al intentar encender el servicio, nos de un problema. `sudo service isc-dhcp-server status`

![6](./img/6.png)
