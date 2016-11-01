###Capítulo 8
----------------------------------------------------------------------------------------------------------------------------

1. Permitir sólamente los módulos necesarios para el funcionamiento que queremos darle.

2. Ejecutando el comando **apache -t**.

3. La cantidad de módulos y directivas de Apache e smuy grande,por lo tanto, la web con la documentación oficial es esencial.

4. El servidor consulta la URL solicitada por el cliente, y averigua qué nombre se ha usado para la solicitud. El método mas común, es que el servidor se basa en el nombre del VirtualHost definido. Otro método es a partir de la IP a la cual está destinada la petición del cliente.

5. Usando el comando **htpasswd**. Dicho comando nos permite crear, modificar y eliminar cuentas de usuarios para método de autentificación sencilla de Apache.

6. Se pueden poner las mismas directivas que se pueden poner en un contexto Directory. La configuración se encuentra en un fichero mas cerca de los datos que en el archivo de configuración de Apache.

7. Indica a Apache que ha de buscar en el Directory donde se declara la directiva AllowOverride, ha de buscar un fichero de configuración adicional (**htpasswd**) de forma automática.

8. Esencialmente para asociar una entidad a una clave pública. Dicha identidad puede ser una referencia a un usuario, un nombre, una IP, etc... La asociación está garantizada por una Autoridad de Certificación ya que está firmada por dicha Autoridad.

9. En u nproxy, el cliente se dirige al servidor proxy indicándole el servidor web objetivo. El proxy captura la petición y, a su vez, enví auna petición al servidor objetivo, pero en nombre del cliente. Se tiene un flujo de datos del cliente al proxy, y otro flujo de datos del proxy al servidor objetivo.

10. Si, la directiva ACL usada en el fichero de configuración de Squid puede hacer referencia a un parámetro de red o designar un archivo que contena este mismo parámetro.

11. Consume menos recursos ya que un proceso de nginx puede gestionar varias peticiones de forma simultánea.

12. Un bloque de tipo ubicación permite asociar directivas a una petición de un cliente que corresponda a un patrón. El patrón puede ser una cadena de carácteres única (operador =), un inicio de cadena de carácteres (sin operador) o una expresión regular (operador ~). Las peticiones que corresponden al criterio de selección del bloque se pueden asociar a un directorio, a una URI o a un servidor de destino remoto.

13. Que son estáticos. Por lo tanto, no se pueden cargar de forma dinámica como los de Apache. Hay que compilar previamente el módulo con el ejecutable de Nginx. Esta característica es una elección del creador de Nginx para obtener mejor rendimiento.

14. La directiva try_files permite especificar qué elementos buscar y en qué orden, en respuesta a una petición asociada a su ubicación. Elservidor puede ejecutar diferentes intentos de respuesta. El último argumento puede ser elnombre de un bloque de ubicación que sirva.

15. Si, como servidor de correo proxy, gestiona protocolos SMTPm POP3 e IMAP4.
