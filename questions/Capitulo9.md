###Capítulo 8
----------------------------------------------------------------------------------------------------------------------------

1. Un alias es la asociación de una identidad con una cuenta existente.

2. El relayhost se suele utilizar cuando la IP proporcionada por nuestro proveedor de internet tiene un dudoso pasado y est'aen blacklist. Con **relayhost** podemos redirigir el correo saliente a nuestroporveedor de servicios de Internet, y que este haga el envío, evitandoque los mails no puedan llegar por salir desde una IP baneada.

3. Si, con postfix se puedegestionar un dominio de correo en una red local, y presentarlo al exterior con otro nombre de dominio. Con la directiva **myorigin** en el fichero de configuración de postfix.

4. Alcomparar el dominio de destino con los definifos en **mydestination**, si coincide, el servidor de correo sabe que es el responsable de tratar ese mensaje, y no reenviarlo.

5. Si,para comprobarla validez del fichero de configuración de postfix, hay que utilizar el comando **postfix check** o **postconf -n**.

6. Para definir el final de un correo usando el comando mail, se ha de escribir una línea que contenga únicamente un punto ( . ) .

7. Se puede automatizar un procesado en los mensajes entranter a un MTA usando **procmail**. Se ha de declarar en el fichero de configuración de postfix, y definir las propias reglas de procmail.

8. Si, para enviar un mensaje a todos los usuarios que tienen una sesion interactiva abierta en el servidor, se puede utilizar el comandp **wall**. Con wall se puede enviar un mensaje a todos esos usuarios.

9. EL archivo **/etc/issue** muestra un mensaje a los usuarios antes de abrir la sesión, mientras que **/etc/motd** muestra un mensaje a todos los usuarios una vex han iniciadosesión.

10. Si, sepuede comprobar la autentificación de los servidores courier sin tener que configurar un cliente de correo, mediante el comando **authtest**.
