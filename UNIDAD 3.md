### ACTIVIDAD 3.1
Hacer una figura explicando porque van en pares
¿Qué capa de modelo OSI entra?
![[Diagrama 3.1.drawio.png]]
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