###Capítulo 13
----------------------------------------------------------------------------------------------------------------------------

1. Algunos directorios del sistema de ficheros procfs aparecen y desaparecen porque son directorios aociados  aun proceso. Cuando un procesose ejecuta, se crea un directorio con informacion del proceso en el sistema de ficheros procfs. Al terminar/morir el proceso, dicho directorio se elimina de forma automática.

2. El comandopara obtener toda la lista de procesos ejecutandose es *ps*. 2 opciones: ps -ef   o   ps aux

3. El comando *dmesg* permite obtener los mensajes alamcenados en el buffer circular que utiliza el kernel, sobretodo al arrancar el sistema. E sposible que, al ser circular, se hayan sobreescrito mensajes mas antiguos. También se puede consultar medante los ficheros de log del sistema (syslog).

4. Para obtener información sobre la memoria físic ay su uso, hay varios comandos como *free*, *vmstat* y *top*. El dichero *meminfo* de *procfs* también tiene dicha información.

5. Para saber si se ha establecido una coneión entrante de ssh, se puede utilizar el comando *netstat -a*, qu emuestra las conexiones de red del sistema. Sólohay que buscar en la lista las conexiones por elpuerto 22.

6. Para diagnosticar el estado de salud de un disco, se utiliza el protocolo de controlde discos *SMART*, mediante el demonio *smartd* y el comando *smartctl* para comprobar su fiabilidad.

7. La falta de memoria libre puede relentizar las operaciones de entrada-salida (input-output) a causa del uso de la swap. Si queda poca memoria libre, elsistma utiliza la swap (espacio en disco), que provoca una relentización en el sistema.

8. Para saber que un fichero nose estña utilizando, se utiliza el comando *lsof* que devuelve una lista de ficheros abiertos y los procesos que lo están utilizando.

9. Para evaluar el impacto de un amuento del número de usuarios de una aplicacion sobre el rendimiento del sistema, se ha de implementar un mecanismo de control de los recursos del sistema, de forma que se puedan obtener estadísticas del consumo de recursos. Una vez estudiados esos datos, se puede sacar conclusiones del impacto de dicho aumento,

10. El monitor delsistema permite ver el estado en tiempo real del uso de lso recursos de es amáquina localen concreto. Nagios en cambio, es una solución global de supervisionde un conjunto de servidores en red, incluyendo todos lo selementos conectados (switches, routers, firewalls, servidores, cabinas de discos, etc...) 
