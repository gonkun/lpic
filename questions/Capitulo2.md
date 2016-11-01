###Capítulo 2
----------------------------------------------------------------------------------------------------------------------------

1. Porque el sistema de ficheros permite organizar el espacio de almacenamiento. Sin sistema de ficheros, una particón y/o volumen lógico, es inservible. El sistema de fichero ste permite gestionar los archivos.

2. Ninguno. Como dice su nombre, son sistemas de archivos virtuales. No existen físicamente, se ubican en la memoria RAM y se montan en un sistema de ficheros real.

3. El azar. Aunque se puden utilizar criterios para generar UUIDs, su aleatoriedad de 128bits garantizan que sean únicos.

4. Con una escritura asíncrona. De esta forma,los datos se escriben primero en memoria comocaché, y luego se escriben en disco. Este método tiene riesgos como que por una avería (corte de luz, disco estropeado, etc.), los datos que estén en memoria se pierden.

5. Porque los comandos que comprueban el estado de los sistemas de archivos, lo hacen en sistemas de archivos demsontados. Estos comandos se ubican en el sistema de archivos raíz, y desmontarlo implica no poder acceder a dichos comandos. Por lo tanto es imposible desmontar el sistema de archivos raíz. La solución es forzar la comprobación en el arranque del sistema, antes de que se monte la raíz. 2 métodos:
   * Mediante el comando e2fsck. modificar la comprobación periódica
   * Forzarlo con el comando shutdown y la opción -F

6. lsdev busca la información en el sistema de ficheros virtual /proc (/proc/interrupt, /proc/ioports y /proc/dma)

7. Gran volumen de datos y ficheros grandes. ext4 está limitado a 16TB de tamaño mñaximo en un volumen. Y es más estable en producción en al actualidad que btrfs.

8. Porque la compresión de datos hacen que estos sean mas difíciles de utilizar en caso de perdida parcial.

9. No, el sistema de archivos hay que montarse si se requiere copiar ficheros concretos. En el caso de un dd, copia bloques sin importar su contenido. No e snecesario montar el CD-ROM.

10. Mínimo tres. Dos para los datos y otro como disco de paridad. Si incluimos en la configuración un disco de recambio (spare), el mínimo pasa a ser cuatro. Este último sirve de reemplazo en caso de que falle uno de los otros tres.

11. Desde un punto de vista funcional, ninguna. Ambos tendrán un sistema de archivos. Pero en el caso  de un volumen lógico (LV), se puede expandir o reducir su tamaño sin necesidad de modificar los archivos.

12. El iniciador iSCSI, es el sistema cliente que quiere utilizar un recurso servido por la parte servidor, el destino iSCSI, como si fuese un dispositivo local. El destino iSCSI es una interfaz de red gesitonada por un servidor iSCSI que permite el acceso a dispositivos lógicos de almacenamiento (LUN), que el cliente ve como un dispostivo local. Linux puede proporcionar los 2 roles.
