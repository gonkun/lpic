###Capítulo 4
----------------------------------------------------------------------------------------------------------------------------

1. ifconfig , que además permite configurar la máscara de subred, la IP principal, la secundaria y la dirección MAC.

2. En principio no es necesario, ya que la puerta de enlace se define de forma independiente a las interfaces de red. Pero puede darse el caso de que se requiera configurar una puerta de enlace para una interfaz de red, y otra puerta de enlace para la otra.

3. Se hace la asociación de la tabla ARP de direcciones IP y direcciones MAC de forma directa, sin necesidad de recurrir a peticiones ARP. Pero el beneficio e snulo, ya que las peticiones ARP son muy rápidas y pequeñas en volumen de tráfico. Puede ser útil en términos de seguridad.

4. El que utiliza el fichero hosts.allow, ya que en dicho fichero se indica que hosts pueden acceder a determinado servicio del servidor, el resto son denegados.

5. No, el comando ifconfig muestra información de las interfaces de red incluídas las interfaces WiFi, pero no muestra info de SSID, calidad de señal, etc.. En cambio, el comando iwconfig si es útil para esta función y , además, permite configurarlas.

6. Porque evita que el comando realice resoluciones de nombre inversas. Estos comandos reciben direcciones IPs, MACs y puertos, y por defecto, intentat traducir estos números en nombres. Dicha resolución provoca lentitud en la respuesta.

7. con el comando lsof. El comando lsof muestra los ficheros que están abiertos o están siendo accesibles por los procesos del sistema en ese momento y el usuario que lo ha ejecutado.

8. Para captura de tramas del tráfico en las redes. Muchas aplicaciones como tcpdump o wireshark usan dicha librería.

9. Porque el cliente, en esa fase de la negociación de la dirección IP, no dispone aún de ninguna IP. Para enviar un mensaje unicast, es necesario de disponer una dirección IP.

10. Obtienen el servidor DNS de la subnet porque prevalece.
