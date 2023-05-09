# Prueba de conexión a base de datos localmente, y contraseñas encriptadas.

Es un codigo en el cual se gestiono la conexion de bases de datos con SQL y Java, de importaron dependencias, se crearon diferentes clases JAVA con el codigo de la conexion. <br>
Se hace una encriptacion de contraseñas atravez de SQL y JAVA

## Estructura del Proyecto

### Conexión a DB:
creamos una clase llamada "BasicConnection" para comprobar la conectividad local con variables establecidas del localhost de SQL, seguidamente creamos un archivo llamado "pool de conexiones" donde alli implementamos las dependencias en el pom.xml con la version del Apache.

  
### Encriptacion y desencriptacion:
 en la base de datos ya creada cambiamos el tipo de dato de "VARCHAR" a "VARBINARY", seguidamente definimos una frase, que no sea del diccionario y la convertimos en HASH. <br>
 creamos una insert con AES_ENCRYPT y ponemos la frase UPPER que Devuelve una expresión de caracteres con datos de caracteres en minúsculas convertidos a mayúsculas, en las variables: (user_firstname, user_lastname, user_email, user_password) VALUES (UPPER('nombres'), UPPER('apellidos'), 'buzon@correo.com',AES_ENCRYPT('password', '$2a$12$71SJ2B6qdXDQrZUF4KR5suDytQ062kLQf/QHbatSw8wLqu1DoMppm) aqui en la ultima varible 'password' estara la frase que ejecutamos en el HASH. <br>
para desencriptar se hace con un select de estamanera: <br>
SELECT *, CAST(AES_DECRYPT(user_password, '$2a$12$71SJ2B6qdXDQrZUF4KR5suDytQ062kLQf/QHbatSw8wLqu1DoMppm') AS CHAR(50)) end_dataFROM users_tbl WHERE user_id = 1

## Dependencias

### Dependencias de Sistema
- IntelliJ IDEA version 2023.1 <br>
- Jakarta EE <br>
- MySql

## Contacto
Jhoann Sebastian Zamudio <br>
jszamudio35@soy.sena.edu.co <br>
https://github.com/JoanZamudio/JAVA_AVANZADO_07_05.git
