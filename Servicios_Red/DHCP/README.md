# Configuración de DHCP en Linux

En este informe vamos a instalar y configurar un servicio DHCP en un sistema operativo Linux Ubuntu.

- Lo primero que haremos será ir a nuestra terminal y ejecutar el comando `sudo apt-get install isc-dhcp-server`

![1](./img/1.png)

- Una vez terminada la instalación iremos a `/etc/dhcp/dhcpd.conf`

![2](./img/2.png)

- Entramos en ese archivo e insertamos la información de nuestra IP,  máscara y el rango de IPs que va a escoger para los equipos.

![3](./img/3.png)
