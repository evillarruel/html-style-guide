html-style-guide
================

MercadoLibre HTML Style Guide


##HTML5
Es la combinación de nuevos elementos de markup o sintaxis. Estas nuevos elementos suponen herramientas más avanzadas, lo cual se traduce en mejores experiencias para el usuario final.

###Ventajas de usar HTML5
* Permite la carga mas rápida al ser más sencillo y simple el código.
* Añade etiquetas para manejar la semántica, permitiendo describir cual es el contenido
* Permite interactuar e insertar directamente video y música sin utilizar flash.

##Elementos
El markup HTML5 incorpora algunas etiquetas nuevas pensadas para hacer que la estructura de las paginas webs sean mas logicas y funcionales.

### Nuevas reglas de semantica
* No es necesario el cierre de las siguientes etiquetas

````html
<!-- DON'T -->
<br />
<hr />
<img src=''... />
<input ... />
````

````html
<!-- DO -->
<br>
<hr>
<img src=''... >
<input ... >
````

* La declaración del documento está completamente minimizada

````html
<!DOCTYPE html>
````

* Se puede usar tanto minúsculas como mayúsculas en el código.

##Nuevos elementos de HTML5
````html
<header> <nav> <article> <section> <aside> <footer> <audio> <canvas> <command> <datalist> <details> <dialog> <embed> <figure> <mark> <meter> <output> <progress> <ruby> <rp> <rt> <source> <time> <video>
````

##Estructura basica de elementos
````html
<body>
    <header>...</header>
    <nav>...</nav>
    <article>
        <section>...</section>
    </article>
    <aside>...</aside>
    <footer>...</footer>
</body>
````
