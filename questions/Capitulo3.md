### Capitulo 3
----------------------------------------------------------------------------------------------------------------------------------
1. **Daemon**: Programa, aplicación o proceso que se ejecuta en segundo plano.
**Servicio**: Programa formado por una serie de daemons que proporcionan funcionalidades a clientes.
*Nivelde ejecución*: Estado funcionalde un sistema que tiene funcionando una serie de servicios diferentes.

2. **restart** ejecuta un **stop** y un **start**, provocando que la aplicación vuelva a cargar la config. **reload** mantiene los procesos en ejecución, obligándolos a releer los ficheros de configuración,y se reconfiguren de forma dinámica, enviando una señal 1 (hup).

3. `/etc/rc.local` En él, el sysadmin puede incluir comandos aejecutar al final del arranque del sistema.

4. Usando **symlinks**. De esta forma se matiene una cierta coherencia enter diferentes distribuciones.

5. En el MBR, que está en los primeros sectores del disco, antes de la tabla de particiones, y donde la BIOS accede primero.

6. En caso de que haya problemas en las particiones, montándolas en modo Read-Only, se pueden hacer tareas de mantenimiento si afectar a los datos.

7. El parámetro **init=** permite definir qué ejecutable debe arrancar justo después de cargar el kernel. Si el ejecutable es **shell**, arrancará una terminal de forma independiente del resto de servicios. Es una forma de acceder a un sistema del cual se ha perdido la contraseña.

8. Modificiar el fichero **inittab**, donde se define el runlevel del arranque. Concretamente el parámetro **initdefault**.

9. Porque para arrancar un sistema Linux es necesario cargar el kernel mediante un gestor de arranque, el cual se encuentra fuera de cualquier partición, por lo tanto, no se puede copia rmediante herramientas de gestor de ficheros ordinarios.

10. Después de modificar el fichero de configuración,se ha de lanzar el comando que actualiza dicha configuración en el programa cargador. El comando es `/sbin/lilo`
