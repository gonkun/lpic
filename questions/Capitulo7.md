###Capítulo 7
----------------------------------------------------------------------------------------------------------------------------

1. Para guardar informaición de distinto tipo. Así, un cliente puede solicitar a un servidor DNS información precisa.

2. Los registros MX hacen referencia a los servidores de correo y mensajería de un dominio DNS. Si no se registra un servidor de correo con el registro MX en un servidor DNS, dicho servidor de correo puede no recibir correos y mensajes del exterior.

3. Al disponer de una caché, guarda en memoria las resolución de nombres consultadas anteriormente. De esta forma, si se le vuelve a solicitar una resolución de nombre que ya había resuelto anteriormente, responderá de forma más rápida; ya que el servidor no ha de volver a consultar a su servidor DNS superior.

4. No hace falta, viene integrado en el sistema ya que formaparte de la pila IP.

5. Si, esta directiva incluye a los ficheros de configuración anexas alficheroprincipal **named.conf**. Pero por contra, al configurar todo en un solo fichero, provocará que el fichero named.conf será muy grande.

6. Configurando una redirección hacia el servidor DNS del proveedor de Internet usando la **directiva forwarders**. El servidor resolverá todas als resoluciones de nombres locales, el resto las reenviará al servidor DNS del proveedor de Internet.

7. Mediante el comando **rndc** se puede volver a cargar la configuración de una sola zona sin reiniciar el servicio.

8. dig

9. Mediante 2 formas. La primera es enjaulando el proceso **named** mediante un **chroot** (cambio de raíz). La prisión es una estructura de directorios que tiene una copia de todos los elementos necesarios para ejecutar el proceso. Además, se combina con el segundo método, que es ejecutar el proceso con una cuenta de sistema con privilegios limitados, por lo que una posible vulnerabilidad, no afectará a otros procesos.

10. Una delegación es externalizar la administración de una zona hija usando otro servidor. Todas las peticiones que se hagan en el servidor padre a la zona hija, se reenviarán de forma dinámica al servidor de la zona hija. Sin comunicación, no es posible hacer dicho reenvío.
