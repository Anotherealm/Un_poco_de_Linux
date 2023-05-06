=================================================================================================

=================================================================================================

## Componentes de red

- ISP : Proveedor de servicios de internet, tanto para compañías como hogares.

- Router : Los routers permiten que cada dispositivo de una red pueda conectarse a Internet.
	   Permite la conexión vía cables o inalámbrica.

- WAN : Red de Área Amplia, es una red que abarca todo desde un router y otra red amplía, como 
Internet.

- WLAN : Red de Área Local Inalámbrica, red entre un router y cualquier dispositivo 
inalámbrico.

- LAN : Red de Área Local, red entre un router y cualquier dispositivo que se conecté vía 
cables.

- Hosts : Cada máquina dentro de una red se le conoce como "host".

Los datos e información que son transmitidos entre redes se les conoce como **paquetes**.

=================================================================================================

## Modelo OSI (Open Systems Interconnection)

: Es un *modelo teórico* de redes.
Este modelo divide los pasos que recorre un paquetes (información), en 7 niveles o capas.

=================================================================================================

## Modelo TCP/IP

: Modelo implementado de redes. Utiliza el conjunto de protocolos TCP/IP. Especifíca como los 
datos deben recopilarse, direccionarse, transmitirse y enrutarse a través de una red.

### CAPAS DEL MODELO TCP/IP

- **Aplicación**
: Capa superior del modelo OSI. Determina cómo un navegador web interactúa con los servicios de 
la capa de transporte para ver los datos que se envían y reciben

	- HTTP (Hypertext Transfer Protocol): Utilizado por las páginas webs en Internet.
	- SMTP (Simple Mail Transfer Protocol) : Transmisión de correo electrónico.

- **Transporte**
: Indica como los datos serán transferidos, incluyendo la verificación de puertos, la 
integridad de los datos y la entrega de paquetes.

	- TCP (Transmission Control Protocol) : Proporciona entrega confiable de datos
	- UDP (User Datagram Protocol) : Entrega de datos no confiable

- **Red**
: Esta capa especifíca como se mueven los paquetes entre hosts y a través de redes.

	- IP (Internet Protocol) : Ayuda a enrutar paquetes de un equipo a otro.
	- ICMP (Internet Control Message Protocol) : Entrega información acerca del envío o 
			                             recepción de paquetes de red, conexión, 
						     debugging.

- **Acceso a red**
: Esta capa especifíca como enviar datos a través de piezas físicas de hardware, como 
transferencia a través de Ethernet, fibra, etc.

=================================================================================================

## Direcciones de red

Para identificar los hosts emisores y los hosts receptores, es necesario direcciones que 
permitan identificar su ubicación en la red. Los dispositivos utilizan direcciones MACs y 
direcciones IPs para identificarse.

#### Dirección **MAC**
: Es un identificador único que se utiliza como dirección de hardware. Esta dirección es única 
y nunca cambia.
Para poder conectarse a Intenet, los equipos necesitan un dispositivo llamado **Tarjeta de 
interfaz de red** (NIC). La dirección MAC es el identificador único asignado a esa NIC.

Cada fabricante de terjeta de interfaz posee un identificador, correspondiente al 
"**Identificador único Organizacional**" (OUI). En una dirección MAC, el OUI es indicado en los 
primeros 3 bytes. El resto de bytes indican el dispositivo.

#### Dirección **IP**
: Son utilizadas para identificar un equipo en una red. No dependen de hardware. Existen dos 
tipos, IPv4 IPv6. También existen las direcciones IPs Públicas y Privadas.

#### Hostnames
: Otra forma de identificar un equipo en la red es por medio del hostname. Hostnames son una 
forma leible de dirección IP. Por ejemplo, en vez de recordar la dirección IP 192.168.1.14, 
puede ser recordado como myhost.com


==========================================================================================

