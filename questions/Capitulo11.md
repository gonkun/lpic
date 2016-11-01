###Capítulo 11
----------------------------------------------------------------------------------------------------------------------------

1. telnet, aún siendo inseguro, dispone de ciertos mecanismo de seguridad como la autentificación por contraseña. El problema es que la transmisión de dicha contraseña se envía sin cifrar.

2. Un cliente SSH guada un registro de las conexiones establecidos mediante SSH con otras máquinas y almacenan su huelal digital en el fichero *known_hosts*.

3. La creación de claves públicas y privadas requiere que se creen conjuntas. ssh-keygen permite hacerlo.

4. MEdiante el comando *ssh-agent* podemos almacenar varias claves privadas en memoria. Un avez arrancado el ssh-agent, se pueden ir agregando claves privadas a una pila.

5. *scp* se bas aen *ssh* para poder transferir ficheros de un host a otro de forma segura.

6. Se llama *tunel SSH* la configuración de SSH que permite transportar el tráfico de una aplicación mediante SSH.

7. Si, se pueden reenviar sesiones X11 en un tunel SSH. Hay que configurar la directiva *X11Forwarding yes* en el fichero *sshd_config* del servidor SSH.

8. Un *tunel punto a punto* conecta a 2 hostas directamente entre ellos de forma segura. El modo sitio a sitio es igual pero todos los hosts de ambas redes conectadas pueden comunicarse enter ellos mediante el tunel. Como lo usamos en BMAT.

9. Con OpenVPN se pueden conectar 2 hosts enter si sin proporcionar enrutamiento. Es lo que se denomina, *modo puente*.

10. Se puedecomprobar si hay un túnel OpenVPN en una máquina revisando la configuración de las interfaces de red.
