###Capítulo 6
----------------------------------------------------------------------------------------------------------------------------

1. Meidante una operación de montaje. El directorio compartido se monta en un directorio local.

2. Si, usando el comando *exportfs* con el parámetro -a .

3. El control de acceso del NFS se basa en el UID de los clientes que se conectan. La cuenta root siempre tiene el UID 0 y la opción root_squash hace que sus privilegios desaparezcan, de forma que el usuario root no tenga plenos derechos en el volumen NFS montado. Este comportamiento se puede modificar usando el parámetro no_root_squash.

4. NFS depende de 3 procesos: *nfsd*, *portmapd* y *mountd*.

5. La opción de montaje *sync* permite que las escrituras sean sincronas sin pasar por una caché. El cliente no estará informadop de que se ha completado un proceso de escritura hasta que este haya sido finalizado realmente.

6. Si, usando el comando *testparm*. Comprueba la validez del archivo de configuración de Samba y muestra las directivas activas por pantalla.

7. Deshabilitando o no aplicando el parámetro *browseable*.

8. No se puede las contraseñas Unix se cifran con MD5 y las de Samba en MD4. Nose puedencrear conrtaseñas a partir de datos cifrados con algoritmos hash.

9. Si, incluyendo la opción *unix passwd sync = yes* en fichero de configuración de Samba.

10. Porque el modo activo eradetectado por los firewalls como amenazas.
