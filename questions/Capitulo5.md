###Capítulo 5
----------------------------------------------------------------------------------------------------------------------------

1. Porque el fichero **/etc/passwd** ha de ser accesible en modo lectura, donde se almacena al informacion de los usuarios y sus contraseñas cifradas mediante un algoritmo de hash. Con elpasodel tiempo, la potencia de los procesadores, se llegó al punto de poder descifrar la scontraseñas a partir de su hash. Para evitar este problema, se movieron las ubicación de las contraseñas cifradas al fichero **/etc/shadow**, el cual sólo es accesible mediante el usuario **root**.

2. El fichero **/etc/nsswitch.conf** contiene toda la info de resolución de nombres. Enter ellos, los parámetros de la fuente de la cual resolverá lso nombres, ya sea local (files) o un servidor dns (dns).

3. Porque los desarrolladores sólo tienen que hacer que sus aplicaciones sean compatibles con las librerías PAM. Si el sistema de autentificación evoluciona, sólo han de modificar la configuración PAM sin modificar la aplicación.

4. El interés de poder ejecutar una serie de módulos en una sola operación de autentificación.

5. En el caso de que un módulo llamado con elcontrol de comportamiento **required** o **requisite** ha fallado previamente.

6. Se continúa ejecutando el siguiente módulo. El éxite de un módulo llamadocon **required** no interrumpe la ejecución del resto.

7. Es muy difícil. LDIF está íntegramente ligado al esquema del directorio y dos directorios distintos tienen casi siempre distintos esquemas. Los atributos LDAP no serán los mismos en ambos lados y una exportación contendrá elementos que no serán asumibles por el segundo directorio.

8. Porque modifica la contraseña cifrándola. Con **ldapmodify** la modificaría sin cifrar.

9. si, asignando a la variable **LDAPBASE** con el contexto de la búsqueda qye deberán usar los clientes de LDAP.

10. Por si en algún momento, no es accesible el servidor LDAP desde neustro cliente. De esta forma, podemos acceder  anuestro sistema Linux usando cuentas locales.
