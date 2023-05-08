# Prueba de conexión a base de datos localmente, y contraseñas encriptadas.

Es un codigo en HTML el cual contiene dos formulario , uno de registro y el otro de inicio de sesion con validaciones, en una estructura semantica de HTML, estilos de CSS puro y Bootstrap. <br>
Adicionalmente Conexión a Base de datos, Clase bean, DBConnection.

## Estructura del Proyecto

### Conexión a DB:

- Creamos la etiqueta <!Doctype html> para el identificador de web, para el que el SO identifique que version de html estamos usando. 

- Seguido se creo unas etiquetas de "html lang="es"" para saber en que lenguaje estamos programando, que en este caso es en español.

- Creamos una etiqueta llamada <head> para identificar la cabecera del codigo donde alli, se encontraran 
  - el titulo <title>
  - Las etiquetas <meta>: identificador de caracteres especial (charset="UTF-8"), autor del proyecto (name="author"), contenido de la busqueda (name="content"),           palabras clave del motor de busqueda(name="Keywords"), para que se vea resposive, que es lo minimo que un codigo html deberia tener (name="viewport").
  - Las etiquetas <link>: iconos de pestaña (rel="icon"), estilos de bootstrap@5 y los estilos de CSS. 

- Seguido creamos el cuerpo de la pagina con la etiqueta <body> y dentro de la misma encontraran:
  - Etiqueta "header" el cual se encuentra sin contenido y dentro una etiqueta "nav".
  - Etiqueta "section" dentro de la misma se enceuntra una etiqueta "main".
  - Un formulario (form action="" method="") el cual el action se deja en vacio puesto que aun no se requiere y el method en envio "post" y dentro del formulario ya mencionado colocamos un logo x, etiquedas de <label>, <input> y <button> cada etiqueta con su respectiva validacion con atributos en los inputs (type, id, autofocus, pattern) type: tipo de input, id: identificador unico de etiqueta, autofocus: se selecciona automaticamente el primer campo sin dar click, pattern: validacion de caracteres mas la logitud minima y maxima, finalmente creamos un button type submit para el envio de datos, el cual no envia nada porque solo es estatico, ademas tiene un link de regristro donde es totalmente funcional.

  - Creamos un parrafo con la etiqueta "p" donde iran los derecho de autor y el año actual, el formato del año lo hicimos con codigo java para que nos muestre el año actual automaticamente.

  - Etiqueta "footer" el cual es el pie de pagina.
  
### Encriptacion y desencriptacion:
  

## Dependencias

### Dependencias de Sistema
- IntelliJ IDEA version 2023.1 <br>
- Jakarta EE <br>
- MySql

## Contacto
Jhoann Sebastian Zamudio <br>
jszamudio35@soy.sena.edu.co <br>
https://github.com/JoanZamudio/JAVA_AVANZADO_07_05.git
