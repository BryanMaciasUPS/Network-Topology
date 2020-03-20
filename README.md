# Topología de Red Etapa Turín Urb. Milann en PKT

Diseñe esta topología de red para la urbanización Milann, la etapa Turín; 
planteadas unas limitaciones para el desarrollo del proyecto. 
Como tema principal se dio el direccionamiento de red. Me pareció un trabajo productivo porque nos plantea 
libre elección de la urbanización que vamos a realizar su direccionamiento de red.
Presentando ciertos detalles al desarrollar el trabajo, como limitaciones en el uso de conexión a internet, etc. 

## Mapa Satelital

![a](../master/etapa_turin.jpeg)

**Urbanizacion:** Milann Etapa Turin (Maps)

## Planteamiento del Proyecto
En el documento guía, se planteó elegir una urbanización de la ciudad de Guayaquil, 
siguiendo ciertas indicaciones: 
“Cada grupo deberá escoger una urbanización (mediante google maps) y una dirección de red de clase B. 
Luego en base al número de casas y manzanas realizar un adecuado direccionamiento de red 
que evite que el broadcast de una manzana afecte a otra (subredes y vlans)”.
Teniendo esto en cuenta, diseñe la red de la urbanización, contabilizando el número de manzanas y casas en la misma;
ubicando 4 pc conectadas a un mismo switch en cada manzana.
Dado que son 11 manzanas, la Etapa Turín necesito de 44 pc, 
conectados a cada switch correspondiente e interconectados todos a su vez a un router como salida a internet:

* Mz 1(Vlan 5): 153.19.0.17
* Mz 2(Vlan 10): 153.19.0.33
* Mz 3(Vlan 15): 153.19.0.65
* Mz 4(Vlan 20): 153.19.0.129
* Mz 5(Vlan 25): 153.19.0.225
* Mz 6(Vlan 30): 153.19.1.0
* Mz 7(Vlan 35): 153.19.1.17
* Mz 8(Vlan 40): 153.19.1.33
* Mz 9(Vlan 45): 153.19.1.65
* Mz 10(Vlan 50): 153.19.1.129
* Mz 11(Vlan 55): 153.19.1.225
Todos los Switchs están interconectados con sus respectivas manzanas y entre sí, 
teniendo una única conexión a internet.

## Limitaciones en el Desarrollo
Para comodidad del trabajo, se planteó y desarrollo la simulación de la topología en el programa Cisco Packet Tracer, 
por mayor seguridad y manejo optimo; conociendo en número de dispositivos que se iban a emplear, 
siguiendo los detalles que se los especificaron.
Se formuló que seleccioné un método para el direccionamiento de la red que hayamos desarrollado,
elegí el método de router-on-a-stick (“es una de los métodos más comunes para hacer el enrutamiento inter-VLAN. 
Consiste en crear sub interfaces en una sola interface física de un router; 
tenemos con esta configuración la posibilidad de utilizar una sola interface para enrutar los paquetes de varias VLAN 
que viajan a través del puerto trunk de un switch conectado a esa interface”).

## Ejecutar PKT
Instalar [Cisco Packet Tracer](https://www.netacad.com/es/courses/packet-tracer) descargar el proyecto [Urbanizacion Milann Etapa Turin.pkt](../master/Urbanizacion%20Millan%20Etapa%20Turin.pkt),
ejecutarlo y ver el funcionamiento adecuado.
