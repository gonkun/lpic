###Capítulo 10
----------------------------------------------------------------------------------------------------------------------------

1. Si, un servidor Linux es capaz de enrutar paquetes. Sólo hay que habilitar la opción de kernel *net.ipv4.ip_forward* con valor *1* ya que viene desactivada por defecto. Tabién se ha de modificar el valor de */proc/sys/net/ipv4/ip_forward*.

2. Se coge la ruta de dichos ficheros del pseudosistema *proc*, por ejemplo */proc/sys/net/ipv4/ip_forward* y se sustituyen las barras por puntos e ignorando */proc/sys*, de la forma que quedaría así. *net.ipv4.ip_forward* en el fichero */etc/sysctl.conf*. Al arrancar, el sistema lee este fihcero y aplica los valores en el pseudosistema.

3. Si, se dispone de una tabla de enrutamiento en un sistema Linux aunque tenga una sola interfaz de red.

4. Con el comando *iptables -L* se muestran las reglas de la tabla por defecto, *filter*.

5. hay que getsionar reglas distintas según la cadena que se desea configurar. INPUT hace referencia al tráfico entrante con destine el propio sistema, FORWARD aplica al tráfico enrutado a travé sdel sistema.

6. Si no se aplica ninguna de las reglas definidas en las cadenas de las tablas, se aplica la regla por defecto, o policy definidas con laopción *-P.*.

7. En el propio funcionamiento de NAT, se puede decir que aporta una protección a las redes privadas. Las IPs de las máquinas en una red privada, no van mas allá del router que las comunica con el resto de redes del mundo. NAT reemplaza dicha IP privada en una pública, agregandocierta privacidad a las IPs privadas o locales.

8. Se puede automatizar la creación de reglas iptables usando aplicaciones como *fail2ban*.

9. Bugtraq y CERT son organismos de investigación de vulnerabilidades. Publican vulnerabilidades descubiertas.

10. OpenVAS tiene arquitectura cliente/servidor, lo cual permite centralizar la configuración y su administración en un servidor mientras que los clientes se instalan en el resto de máquinas que hay que proteger.
