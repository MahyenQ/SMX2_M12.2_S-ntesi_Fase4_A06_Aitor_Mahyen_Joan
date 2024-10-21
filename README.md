##### SMX2_M12.2_Síntesis_Fase4_A06_Aitor_Mahyen_Joan

# Actividad 6 Redes 

## Índice

#### 1. Clasificación IP's
#### 2. ¿Qué IP 's se utilizan para servidores y qué IP' s para puertas de enlace?
#### 3. Funcionalidad de las máscaras de red y cómo se calculan según la clasificación de IP 's
#### 4. VLAN (qué es y para qué sirve, configuración en Packet Tracer)
#### 5. Configuración de red en máquinas virtuales. Diferentes configuraciones de los adaptadores de red.
#### 6. Configuración de red en Windows.
#### 7. Configuración de red en Linux (en Debian y Ubuntu 24.04)



## *1. Clasificación IP's*

### Sabemos clasificar las *IP’s privadas VS públicas* 


- Las IP's públicas son las que pueden salir a Internet y son direcciones únicas que identifican a nuestro dispositivo en Internet. Cuando nos conectamos a Internet, nuestro proveedor de servicios de Internet (ISP) nos asigna una IP pública. Esta dirección permite que otros dispositivos y servidores en Internet nos encuentren y se comuniquen con nosotros. 

**Algunos puntos clave:**

1. Identificación: Cada dispositivo que se conecta a Internet necesita una IP pública para ser identificado. Sin ella, no podríamos enviar ni recibir información. 
2. Comunicación: Cuando visitamos un sitio web, nuestra IP pública es la que se muestra al servidor del sitio lo le permite saber a dónde enviar la información que solicitamos.
3. Acceso: Las IPs públicas son necesarias para acceder a servicios en línea, como correos electrónicos, redes sociales y páginas web.
4. Interacción: Si queremos que otros dispositivos, como un servidor de juegos o una cámara de seguridad, se conecten a nuestra red, entonces necesitamos configurar nuestra IP pública para que puedan hacerlo.

### Sabemos clasificarlas el protocolo IPv4 que permite un número limitado de direcciones únicas y dentro de IPv4, las direcciones IP se dividen en clases que son:

- **Clase A**: se utilizan para redes muy grandes, es decir, grandes empresas o proveedores de servicios de Internet que necesitan muchas direcciones IP.
- **Clase B**: se utilizan para redes medianas como universidades o grandes organizaciones que requieren una gran cantidad de direcciones IP.
- **Clase C**: se utilizan para redes pequeñas, es decir, pequeñas empresas que necesitan una cantidad limitada de direcciones IP.
- **Clase D**: se utilizan para multicast para enviar datos a varios destinatarios (grupos) al mismo tiempo
- **Clase E**: están reservadas para investigación y desarrollo, no se utilizan en redes comunes.

|Clases |Empiezan por |IP'S/M|
|----------|:----------:|:----------:|
|A |0 a 127|29.15.10.5/8|
|B |128 a 191|133.11.24.3/16|
|C|192 a 223|192.186.15.5/24|
|D|224 a 239|224.220.225.238|
|E|240 a 255|240.241.250.253|


- Las IPs privadas son direcciones que se utilizan en redes locales, como en casas, oficinas o empresas. Estas direcciones son diferentes de las IPs públicas, que son las que se usan para conectarse a Internet.

**Por ejemplo**: si tenemos varios dispositivos en nuestra casa, como nuestra computadora, el teléfono y la impresora, cada uno tendrá una dirección IP privada para poder comunicarse entre ellos.

Las IPs privadas no pueden salir a Internet directamente. En cambio, cuando queremos acceder a Internet, nuestro router utiliza una IP pública para comunicarse con el mundo exterior. Así que, aunque nuestros dispositivos tengan IPs privadas, pueden navegar por Internet gracias a esa IP pública que el router tiene.


|Clases |IP'S/M |
|----------|:----------:|
|A |10.X.X.X|
|B |172.16.X.X a 173.31.X.X |
|C|192.168.X.X|


### Sabemos clasificar las *IP’s especiales o reservadas*


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

## *2. Que IP's se utilizan para servidores y cuales IPs para puertas de enlace*

- Sabemos que los servidores utilizan IPs altas, cómo pueden ser 248,250 etc. Aparte de que éstas IPs deben ser estàticas.

- Sabemos que las IPs de puerta de enlace acaban en X.X.X.1


## *3. Funcionalidad de la máscaras de red y cómo se calculan según la clasificación de IP's*

- Las máscaras de red hace saber a demás dispositivos que parte de la IP es, que son de número 255, y se ponen dependiendo de la clase de IP:

|Clases |IP'S/M |
|----------|:----------:|
|A |X.X.X.255|
|B |X.X.255.255|
|C|X.255.255.255|


## *4. VLAN (qué es y para qué sirve, configuración en Packet Tracer)*


- VLAN: Virtual Local Area Network, son ordenadores en un mismo dominio de una LAN para comunicarse solamente entre ellos, dando igual donde este su posición.

**Ejemplo:**

![VLAN](https://github.com/MahyenQ/SMX2_M12.2_S-ntesi_Fase4_A06_Aitor_Mahyen_Joan/blob/main/VLAN.jpg.png)

## *5. Configuración de red en máquinas virtuales. Diferentes configuraciones de los adaptadores de red*

- Sabemos configurar los 4 diferentes tipos de adaptadores que son red NAT, NAT y adaptador puente.


## *6. Configuración de redes de Windows*

- Sabemos configurar las IP de manera estática y dinámica. Principalmente en interfaz gráfica, identificar qué adaptador se está usando y que IP, máscara y gateway o DNS está asociado a esa IP.

- Sabemos mirar la MAC de nuestro adaptador de red, ipconfig /all

## *7.  Configuración de red en Linux (en Debian y Ubuntu 22.04)*

- Sabemos usar la configuración en netplan (Debian) y net-tool (ubuntu después de la 16.07) mediante comandos y también cambiar tanto la IP como la máscara, gateway y DNS asociado.





