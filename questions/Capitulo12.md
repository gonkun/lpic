###Capítulo 12
----------------------------------------------------------------------------------------------------------------------------

1. La ejecución de un programa interpretado requiere el uso de otro programa intérprete para que el procesador pueda ejecutarlo. Encaso de un programa compilado, el binario del programa compilado contiene directamente instrucciones inteligibles por el procesador. Por lo tanto, el tratamiento es mucho mas rápido. Como desventaja, un programa compilado, es menos portable ya que está intimamente relacionado con el juego de intrucciones del procesador.

2. El script *configure* que viene el el código fuente sirve para comprobar la validez del entorno de compilacion y generar el fichero *Makefile* que utilizará el compilador.

3. *make clean* limpia el directorio de las fuentes de todos los elementos resultantes de la compilación. *make mrproper* borra cualquier otro elemento que no pertenezca a las fuentes, incluso los de configuración. deja la situación comosise hubiese eliminado todo lo hecho hasta ahora.

4. Cuando un programa se compila de forma dinámica, depende de las librerías compartidas.

5. El comando *ldconfig* consulta al fichero */etc/ld.so.conf* para saber que librerías del sistema ha de inventariar. Este fichero contiene la lista de directorios que se deben de analizar para encontrar los archivos de librerías.

6. El objetivo del comando *make* para poder basarnos en un archivo *.config* de una compilación anterior es el objetivo *oldconfig*.

7. No se debe instalar un kernel con versión 2.5.8 porque es una versión en desarrolo. La segunda cira es impar, por lo tanto, indica que es un kernel en estado de desarrollo.

8. 

9. Los archivos ramdisk son ficheros deltipo *cpio* comprimidos en formato *gzip*.

10. *mkinitrd* ha sido reemplazado por *mkinitramfs* porqueelcomando *initrd* no se basa en la getsion de hardware moderno udev,si no que usa devfs y, además, no es capaz de gesitonar discos duros SATA.
