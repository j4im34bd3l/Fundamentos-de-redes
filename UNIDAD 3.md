### ACTIVIDAD 3.1
Hacer una figura explicando porque van en pares
¿Qué capa de modelo OSI entra?
![[Diagrama 3.1.drawio.png]]
¿Por qué los puntos de intercambio reducen la latencia?
Los puntos de intercambio reducen la latencia porque dejan que ciertas redes se conecten y no necesitan mandar datos lejanos.
### GLOSARIO

**Capa física**

-Bit: Un 1 o un 0, siendo lo más pequeño de bit que puede entender la computadora.

-Señal: Es como viaja la información por el cable en ondas eléctricas.

-Ancho de banda: Es cuanta información puede pasar al mismo tiempo por el camino.

-Rendimiento (throughput): Es lo que pasa de datos en la práctica y no lo teórico.

-Latencia: Es lo que tarda en llegar un paquete de un lado a otro o el ping.

-Medio de transmisión: Es por dónde viaja la señal como la cable de red, la fibra, o el aire.


**Cables y medios**

-Par trenzado (UTP / STP): Son cables de red normales, el UTP no tiene protección extra y el STP sí contra las interferencias.

-Conector RJ-45: Es la pieza de plástico transparente que va en la punta del cable de red.

-Cable directo y cable cruzado: El directo conecta cosas diferentes como de computadora a switch y el cruzado conecta dos cosas iguales como de computadora a computadora.

-Fibra óptica: Es un cable de vidrio muy rápido que manda luz en lugar de electricidad.

-Fibra monomodo y multimodo: La monomodo es para distancias largas como un solo rayo de luz y la multimodo es para distancias más cortas como varios rayos.

-Interferencia electromagnética (EMI): Es cuando las ondas de los cables de luz o lo aparatos arruinan la señal de internet.

-Wi-Fi (IEEE 802.11): Es un conjunto de estándares internacionales que dan las características y el funcionamiento de las WLAN o Wi-Fi.

-Bandas de 2.4 GHz y 5 GHz: Son las dos frecuencias del Wi-Fi, la de 2.4 GHz llega más lejos pero es más lenta y la de 5 GHz es más rápida pero llega menos lejos.

-Bluetooth: Es una conexión corta para conexiones cercanas como audífonos o celulares.


**Señalización**

-Codificación: Es traducir los datos a un formato que se pueda mandar por el cable o por el aire.

-Señalización: Es como se mandan físicamente las señales como los voltajes, las luces, etc.

-Sincronización: Es que el emisor y el receptor estén bien coordinados en el tiempo para así no perder el hilo.

-Código Manchester: Es una forma de acomodar los ceros y unos con la señal para que la computadora no se pierda leyendo, donde cada bit de datos pone un nivel en su punto medio


**Ethernet y LAN**

-Ethernet (IEEE 802.3): Es la tecnología estándar dominante para la construcción de las redes de área local o LAN.

-Tarjeta de red (NIC): Es la Interfaz de un hardware que permite a un equipo el conectarse físicamente a una red de datos.

-Switch: Es un dispositivo de capa 2 que interconecta equipos en una LAN y segmenta el tráfico enviándolo solo al puerto de destino según su MAC.

-Hub: Es un dispositivo de hardware que conecta muchos equipos o nodos en una sola red LAN, que replica datos entrantes por todos sus puertos sin filtrar nada.

-Tabla de direcciones MAC: Es el registro interno o base de datosque utiliza el switch para asociar cada dirección física con su respectivo puerto.

-Dúplex (half y full): Half permite enviar y recibir datos al mismo tiempo, Full permite ambas acciones pero no de forma simultánea.

-Colisión: Es el choque de datos que pasa cuando dos de los dispositivos transmiten al mismo tiempo en un medio compartido.


**Direccionamiento**

-Dirección MAC: Es un identificador físico único de unos 48 bits grabado de fábrica en cada tarjeta de red.

-OUI: Son los primeros 3 bytes de la dirección MAC que permiten identificar al fabricante del dispositivo.

-Hexadecimal: Sistema numérico de base 16, como el 0 al 9 y de la A a la F, utilizado para escribir las direcciones MAC.

-Unicast: Es el tipo de trafico mas común de red dirigido de un único origen a un único destino.

-Multicast: Es un método de comunicación enviado desde una fuente hacia un grupo específico de receptores en la red.

-Broadcast: forma de comunicación dirigido de un paquete a todos los dispositivos dentro de la misma subred de forma sumiltanea.


**Enlace de datos**

-Trama (frame): La unidad de medida enviada en la capa 2, lista para ser encapsulada y enviada al medio físico.

-Encabezado y tráiler: Los bloques de información agregados al inicio y al final de la trama con información de que van por las capas del modelo OSI o TCP/IP.

-FCS / CRC: Son importantes para detectar si los datos tuvieron errores en el camino de la base de datos de la red física.

-Subcapa LLC: La parte superior del enlace de datos que ve la Identificación de protocolos como un puente de software y hardware.

-Subcapa MAC: Es la parte inferior del enlace de datos que controla el acceso al medio físico y se usa como interfaz del software y del hardware.

-CSMA/CD: Es un protocolo de control de acceso para redes Ethernet semidúplex que detecta colisiones y vuelve a intentar la transmisión tras un retraso 16 veces antes de parar.

-CSMA/CA: Es un protocolo de control de acceso al medio utilizado principalmente en redes inalámbricas para evitar choques antes de transmitir, debido a que no se pueden detectar mientras ocurren.

### COMANDOS DE REDES

-ping: Es una herramienta en redes que mide el tiempo que tardan los datos en viajar el paquete desde el dispositivo hasta un servidor para ver si hay conexión y cuánto tarda en responder.

-ipconfig: Es una herramienta de línea de comandos puesta en el sistema operativo que permite ver la información red de una computadora, es útil para saber qué IP se tiene.

-tracert: Es una herramienta de diagnóstico de red que enseña el camino para rastrear la ruta que sigue el paquete de datos desde la computadora hasta su destino, sirve para ver en dónde se atora el internet.

-cd: O Change Directory Sirve para poder moverse entre las carpetas de la terminal o símbolo del sistema, por ejemplo para entrar a una carpeta que alguien escribe.

-dir: O Directory se muestra una lista con todos los archivos y carpetas que están adentro del directorio en el que alguien puede estar en ese momento.


# Práctica 3: Tabla de direcciones MAC del switch

  

**Unidad 3:** Capa física y de enlace de datos

**Herramienta:** Cisco Packet Tracer

**Duración aproximada:** 25 a 30 minutos

  

## Objetivo

  

Observar cómo un switch aprende las direcciones MAC de los dispositivos conectados y las asocia con sus puertos.

  

## Material

  

- 1 switch 2960

- 4 PCs (PC0 a PC3)

  

## Desarrollo

  

### Paso 1. Arma la red

  

1. Coloca un switch 2960 y 4 PCs (PC0 a PC3).

2. Conecta cada PC al switch con cable directo (*Copper Straight-Through*):

  

   | PC | Puerto del switch |

   |---|---|

   | PC0 | Fa0/1 |

   | PC1 | Fa0/2 |

   | PC2 | Fa0/3 |

   | PC3 | Fa0/4 |

  

3. Espera a que los enlaces se pongan en verde.

  

### Paso 2. Asigna las IPs

  

En cada PC, entra a **Desktop → IP Configuration** y escribe:

  

| PC | IP | Máscara |

|---|---|---|

| PC0 | 192.168.1.1 | 255.255.255.0 |

| PC1 | 192.168.1.2 | 255.255.255.0 |

| PC2 | 192.168.1.3 | 255.255.255.0 |

| PC3 | 192.168.1.4 | 255.255.255.0 |

  

> Las IPs solo sirven para poder hacer ping. Lo que se analiza en esta práctica son las direcciones MAC.

  

### Paso 3. Anota la MAC de cada PC

  

1. En cada PC, abre **Desktop → Command Prompt**.

2. Escribe `ipconfig /all`.

3. Copia la **Physical Address** de cada PC en una tabla con estas columnas: PC, puerto del switch y MAC.

  

### Paso 4. Revisa la tabla del switch antes de enviar tráfico

  

1. Haz clic en el switch y abre la pestaña **CLI**.

2. Presiona Enter, escribe `enable` y presiona Enter.

3. Escribe:

  

   ```

   show mac address-table

   ```

  

   Si el comando no se reconoce, usa `show mac-address-table`.

4. Toma una captura de pantalla. La tabla debería estar vacía o casi vacía, porque el switch todavía no ha visto tramas.

  

### Paso 5. Genera tráfico entre dos PCs

  

1. En PC0, abre **Command Prompt** y ejecuta:

  

   ```

   ping 192.168.1.2

   ```

  

2. El primer ping puede fallar con "Request timed out". Es normal: PC0 primero necesita conocer la MAC de PC1 mediante ARP.

3. Ejecuta el ping otra vez hasta que responda.

  

### Paso 6. Revisa la tabla otra vez

  

1. Regresa al CLI del switch y ejecuta `show mac address-table`.

2. Deben aparecer las MAC de PC0 y PC1, cada una asociada a su puerto (Fa0/1 y Fa0/2), con tipo **DYNAMIC** y VLAN 1.

3. Toma otra captura de pantalla.

  

### Paso 7. Completa la tabla

  

1. Desde PC2, haz ping a PC3:

  

   ```

   ping 192.168.1.4

   ```

  

2. Revisa la tabla del switch una tercera vez.

3. Ahora deben aparecer las 4 MAC, cada una en su puerto.

4. Compara contra las MAC que anotaste en el paso 3: deben coincidir. Toma una captura.

  

### Paso 8 (opcional). Borra la tabla y observa cómo se aprende de nuevo

  

1. En el CLI del switch, ejecuta:

  

   ```

   clear mac address-table dynamic

   ```

  

2. Ejecuta `show mac address-table`: la tabla debe estar vacía otra vez.

3. Haz un ping entre dos PCs y consulta la tabla de nuevo: el switch vuelve a aprender las MAC.

  

## Entregable

  

1. Capturas de pantalla de la tabla del switch en tres momentos: paso 4 (antes del ping), paso 6 (después del primer ping) y paso 7 (con las 4 MAC).
      
      ![[Captura de pantalla 2026-10-20 210833.png]]
     Muestra la tabla del switch completamente vacía antes de enviar tráfico.![[Captura de pantalla 2026-10-20 211453.png]]
     Muestra las MACs de PC0 (Fa0/1) y PC1 (Fa0/2) aprendidas de manera dinámica.![[Captura de pantalla 2026-10-20 211949.png]]
     Muestra las direcciones de las 4 PCs registradas en la tabla (Fa0/1, Fa0/2, Fa0/3, Fa0/4)
     
1. La tabla escrita con PC, puerto del switch y MAC.
    PC0  192.168.1.1  Fa0/1  0001.C974.CE85
    PC1  192.168.1.2  Fa0/2  0006.2A6A.EC67
    PC2  192.168.1.3  Fa0/3  0060.70BD.744B
    PC3  192.168.1.4  Fa0/4  00E0.A38E.A910  
	 
2. Respuestas breves a estas preguntas
     
   3. ¿De dónde aprende el switch las direcciones MAC?
     El switch aprende las direcciones MAC leyendo la dirección MAC de origen (Source MAC) que viene en las tramas Ethernet que entran por sus puertos. Cuando una PC transmite datos, el switch anota esa MAC y la asocia automáticamente al puerto físico por el cual ingresó la trama, guardándolo en su tabla interna.
     
   4. ¿Por qué falló el primer ping?
     El primer intento de ping suele fallar con un mensaje de tiempo de espera agotado (_Request timed out_) porque la PC emisora necesita primero descubrir la dirección física (MAC) del destinatario a través del protocolo ARP (Address Resolution Protocol) antes de poder encapsular los datos en una trama Ethernet y enviarlos. Una vez resuelto el ARP, los siguientes pings responden con normalidad.
     
   5. ¿Qué tipo de entrada (dinámica o estática) tiene cada MAC y qué significa?
     Entrada Dinámica (DYNAMIC): Son las entradas que el switch aprende automáticamente al escuchar el tráfico de los dispositivos en la red. Tienen la característica de borrarse solas si pasa cierto tiempo sin actividad (tiempo de expiración) o si se reinicia el equipo/comando de limpieza.
     Entrada Estática (STATIC): Son las direcciones MAC que un administrador configura manualmente en el switch para que permanezcan fijas y no se borren por expiración, otorgando mayor seguridad o control estricto sobre qué dispositivos pueden conectarse a un puerto.

6. Guarda tu archivo de Packet Tracer (`.pkt`) y entrégalo junto con lo anterior.


### Artefacto 2.1

Nombre: Jaime Abdel Castañeda Valadez

Campo 1
Dato de ejemplo: 10101010 10101010 10101010 10101010 10101010 10101010 10101010 10101011 (8 bytes)
Nombre del campo: Preámbulo
Para qué sirve: Sincroniza los relojes de los dispositivos antes de que comenzar a transmitir los datos. Los primeros 7 bytes permiten estabilizar y alinear su reloj fisico con la señal entrante. Y el ultimo byte actua como un aviso que rompe el patrón.

Campo 2
Dato de ejemplo: FFFF.FFFF.FFFF (6 bytes)
Nombre del campo: Dirección MAC de Destino
Para qué sirve: Sirve al indicar que dispositivos de la red local va dirigida. Al solo tener puras F, significa que es un mensaje dirigido a todos los equipos conectados a esa misma red.

Campo 3
Dato de ejemplo: 0001.4321.ABCD (6 bytes)
Nombre del campo: Dirección MAC de origen
Para qué sirve: Sirve para que el receptor sepa quien mando el mensaje y le pueda responder, y lee el switch para ver el puerto por el cual llego la trama.

Campo 4
Dato de ejemplo: 0x0806 (2 bytes)
Nombre del campo: EtherType
Para qué sirve: Sirve como una etiqueta de identificación que le dice al dispositivo que protocolo de capa superior viene dentro de los datos de la trama.

Campo 5
Dato de ejemplo: ¿Quién tiene la IP 192.168.1.2? Responde a 192.168.1.1 (entre 46 y 1500 bytes)
Nombre del campo: Datos o Carga útil
Para qué sirve: Contiene la información de las capas que se está pasando a través de la red, y tiene diferentes tamaños (46 y 1500 bytes).

Campo 6
Dato de ejemplo: 0x3A7F91C2 (4 bytes)
Nombre del campo: Secuencia de Verificación de Trama
Para qué sirve: Sirve para ver si la trama sufre un error o durante su transmisión física por el cable o red.


### Diferencias de Switch

| Switch 2                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | Switch 3                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ¿Qué son?  <br>Conmutadores que operan solo en la Capa 2. Utilizan el MAC de los dispositivos almacenadas en su tabla interna para saber a qué puerto reenviar los paquetes de red dentro de una misma red local o LAN.                                                                                                                                                                                                                                                           | ¿Qué son?  <br>Dispositivos avanzados de red que combinan las funciones de un switch tradicional de Capa 2 con las capacidades de un router de la Capa 3. Pueden cambiar paquetes a alta velocidad basándose en direcciones MAC y, al mismo tiempo, enrutar paquetes basándose en direcciones IP.                                                                                                                                                                                                                                                         |
| Diferencias  <br>Sin enrutamiento: No entienden ni procesan direcciones IP; por lo que no pueden enrutar tráfico entre diferentes redes o subredes por ellos mismos.<br><br>Inter-VLAN: Para comunicar distintas VLANs necesitan obligatoriamente conectarse a un router externo ométodo conocido como Router-on-a-stick.<br><br>Uso principal: Se emplean en la capa de acceso para conectar de forma directa a los clientes, computadoras y servidores de una oficina o planta. | Diferencias  <br>Capacidad de Enrutamiento: Tienen la facultad de realizar enrutamiento estático y dinámico como OSPF o EIGRP de manera interna entre diferentes subredes y redes.<br><br>Inter-VLAN nativo (Routing Inter-VLAN): Pueden rutear tráfico entre distintas VLANs de forma interna mediante interfaces virtuales de switch sin requerir un router físico externo.<br><br>Uso principal: Se ubican normalmente en la capa de distribución o núcleo de redes corporativas grandes y centros de datos donde se maneja un alto tráfico segregado. |
