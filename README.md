##### SMX2_M12.2_Síntesis_Fase4_A06_Aitor_Mahyen_Joan

## Índice

#### 1. Clasificación IP's
#### 2. ¿Qué IP 's se utilizan para servidores y qué IP' s para puertas de enlace?
#### 3. Funcionalidad de las máscaras de red y cómo se calculan según la clasificación de IP 's
#### 4. VLAN (qué es y para qué sirve, configuración en Packet Tracer)
#### 5. Configuración de red en máquinas virtuales. Diferentes configuraciones de los adaptadores de red.
#### 6. Configuración de red en Windows.
#### 7. Configuración de red en Linux (en Debian y Ubuntu 24.04)



## *1. Clasificación IP's*

#### Sabemos clasificar las *IP’s privadas VS públicas* 


- Las IP's públicas son las que pueden salir a Internet. 

|Clases |IP'S/M |
|----------|:----------:|
|A |29.15.10.5/8|
|B |133.11.24.3/16|
|C|192.186.15.5/24|


- IP’s privadas son las que se usan en casa, oficinas, empresas etc y no se pueden salir a Internet. 

|Clases |IP'S/M |
|----------|:----------:|
|A |10.X.X.X|
|B |172.16.X.X a 173.31.X.X |
|C|192.168.X.X|


#### Sabemos clasificar las *IP’s especiales o reservadas*


- **Id red:** son IP’s que identifican a un conjunto de hosts y tiene todos los bits a 0

**Ejemplo:** 

|Clases |IP'S/M |
|----------|:----------:|
|A |112.0.0.0/8|
|B |130.92.0.0/16|
|C|192.30.15.0/24|


- **IP 's de broadcast:** son IP's que se utilizan en el destino de paquetes para que los recogen todos los dispositivos de red. Y tiene todos los bits de hosts a 1

**Ejemplo:**

|Clases |IP'S/M |
|----------|:----------:|
|A |112.255.255.255/8|
|B |130.7.255.255/16|
|C|192.7.7.255/24|


#### Sabemos clasificarlas el protocolo *IPv4* que permite un número limitado de direcciones únicas y dentro de IPv4, las direcciones IP se dividen en clases que son:


- **Clase A:** Son direcciones que empiezan por *(0-127)* y se utilizan para redes muy grandes, es decir, grandes empresas o proveedores de servicios de Internet que necesitan muchas direcciones IP.
- **Clase B:** Son direcciones que empiezan por *(128-191)* y se utilizan para redes medianas como universidades o grandes organizaciones que requieren una gran cantidad de direcciones IP.
- **Clase C:** Son direcciones que empiezan por *(192-223)* y se utilizan para redes pequeñas, es decir, pequeñas empresas que necesitan una cantidad limitada de direcciones IP.
- **Clase D:** Son direcciones que empiezan por *(224-239)* y se utilizan para multicast para enviar datos a varios destinatarios (grupos) al mismo tiempo
- **Clase E:** Son direcciones que empiezan por *(240-255)* y están reservadas para investigación y desarrollo, no se utilizan en redes comunes.

## *2. Que IP's se utilizan para servidores y cuales IPs para puertas de enlace*

- Sabemos que los servidores utilizan IPs altas, cómo pueden ser 248,250 etc. Aparte de que éstas IPs deben ser estàticas.

- Sabemos que las IPs de puerta de enlace acaban en X.X.X.1


## *3. Funcionalidad de la máscaras de red y cómo se calculan según la clasificación de IP's*

- Las máscaras de red que son de número 255, y se ponen dependiendo de la clase de IP:

|Clases |IP'S/M |
|----------|:----------:|
|A |X.X.X.255|
|B |X.X.255.255|
|C|X.255.255.255|


## *4. VLAN (qué es y para qué sirve, configuración en Packet Tracer)*


- VLAN: Virtual Local Area Network, son ordenadores en un mismo dominio de una LAN para comunicarse sólo entre ellos. 

![VLAN](https://github.com/MahyenQ/SMX2_M12.2_S-ntesi_Fase4_A06_Aitor_Mahyen_Joan/blob/main/VLAN.jpg.png)

## *5. Configuración de red en máquinas virtuales. Diferentes configuraciones de los adaptadores de red*

- Sabemos configurar los 4 diferentes tipos de adaptadores que son red NAT, NAT y adaptador puente.


## *6. Configuración de redes de Windows*

- Sabemos configurar las IP de manera estática y dinámica. Principalmente en interfaz gráfica, identificar qué adaptador se está usando y que IP, máscara y gateway o DNS está asociado a esa IP.

- Sabemos mirar la MAC de nuestro adaptador de red, ipconfig /all

## *7.  Configuración de red en Linux (en Debian y Ubuntu 22.04)*

- Sabemos usar la configuración en netplan (Debian) y net-tool (ubuntu después de la 16.07) mediante comandos y también cambiar tanto la IP como la máscara, gateway y DNS asociado.





