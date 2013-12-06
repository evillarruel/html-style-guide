html-style-guide
================

MercadoLibre HTML Style Guide


##HTML5
Es la combinación de nuevos elementos de markup o sintaxis. Estas nuevos elementos suponen herramientas más avanzadas, lo cual se traduce en mejores experiencias para el usuario final.

###Ventajas de usar HTML5
* Permite la carga mas rápida al ser más sencillo y simple el código.
* Añade etiquetas para manejar la semántica, completa y homogenea permitiendo describir cual es el contenido, su importancia y su finalidad. No tienen especial impacto en la visualización, se orientan a buscadores.
* Permite una mejor indexación e interpretacion de la información.
* Permite interactuar con elementos multimedia como audio y videos.

### Nuevas reglas de semantica
* No es necesario el cierre de las siguientes etiquetas.

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
<<<<<<< HEAD
<!-- DO -->
<!DOCTYPE html>
=======
    <!DOCTYPE html>
>>>>>>> f7abdbdcae581f9a351e0457e1c1d9a2ad3425f4
````

* Se puede usar tanto minúsculas como mayúsculas en el código.

###Nuevos elementos de HTML5
<<<<<<< HEAD
El markup HTML5 incorpora etiquetas nuevas para mejorar la semantica web, haciendo la estructura de la pagina mas logica y funcional.
=======
>>>>>>> f7abdbdcae581f9a351e0457e1c1d9a2ad3425f4
````html
<header> <nav> <article> <section> <aside> <footer> <audio> <canvas> <command> <datalist> <details> <dialog> <embed> <figure> <mark> <meter> <output> <progress> <ruby> <rp> <rt> <source> <time> <video>
````
####Header
Representa la cabecera de una sección, y es de suponer que se le dé más importancia que al resto, sobre todo si la sección es un artículo.
````html
<header>  
    <h1>MercadoLibre - Donde compras y vendes de todo</h1>
    <!-- Header content -->
</header>
````

####Nav
Representa una sección dedicada a la navegación entre el sitio, como la típica barra superior de los periódicos.
````html
<!-- DON'T -->
<div id="nav">
    <ul>
        <li> <a .... /> </li>
    </ul>
</ul>
````
````html
<!-- DO -->
<nav>
    <ul>
        <li> <a href="/login/">Login</a> </li>
        <li> <a href="/account/">My account</a> </li>
        <li> <a href="/notification/">Notification</a> </li>
    </ul>
</nav>
````
####Article
Permite declarar una parte del contenido auto-contenida, como las opiniones.
````html
<!-- DO -->
<article>
    <header>
        <h4>
            Excellent product
        </h4>
        by <a href="/user/...">USERNAME...</a>
        <time datetime="2013-08-29T13:58Z">August 29th, 2013 at 13:58</time>
    </header>
    <p>Review content ...</p>
</article>
````
####Section
Representa una sección "general" dentro de un documento o aplicación. Puede contener subsecciones y si lo acompañamos de h1-h6 podemos estructurar mejor toda la página.
````html
<!-- DO -->
<section>
    <h1>Promotions</h1>
    <p>Promo description</p>
</section>
````

####Aside
Representa un contenido que está muy poco relacionado con el resto de la página, como una barra lateral. Esencial para delimitar el contenido "importante" del contenido "de apoyo", haciendo más caso al primero que al segundo.

````html
<!-- DO -->
<aside>
    <h2>Blogroll</h2>
    <ul>
        <li><a href="#">My Friend</a></li>
        <li><a href="#">My Other Friend</a></li>
        <li><a href="#">My Best Friend</a></li>
    </ul>
</aside>
aside
````

El contenido del elemento ```` aside ```` está directamente relacionada con el artículo.
````html
<!-- DO -->
<article>
    <h1>My Blog Post</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
    eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
    <aside>
        <h1>Glossary</h1>
        <p>ipsum dolor sit amet</p>
    </aside>
</article>
````

El elemento ```` aside ```` puede estar fuera del artículo. Su contenido está relacionado a la página, pero no tan estrechamente con el artículo.
````html
<!-- DO -->
<article>
    <h1>Products Apple</h1>
    <p>The <b>apple</b> is the pomaceous fruit of the apple tree...</p>
    ...
</article>
<aside>
    <h2>Oder products</h2>
    <ul>
        <li><a href="#">AMD</a></li>
        <li><a href="#">Intel</a></li>
        ...
    </ul>
</aside>
````
####Footer
Representa el pié de una sección, con información acerca de la página/sección que poco tiene que ver con el contenido de la página, como el autor, el copyright o el año.

````html
<!-- DON´T -->
<div id="footer">
    <ul>
        <li>copyright</li>
        <li>More information</li>
        ...
    </ul>
<div>
````

````html
<!-- DO -->
<footer>
    <ul>
        <li>copyright</li>
        <li>More information</li>
        ...
    </ul>
</footer>
````
#####El footer dentro de otro elemento
######Section
````html
<!-- DO -->
<section>
   Section content appears here.
   <footer>
   Footer information for section.
   </footer>
</section>
````

######Article
````html
<!-- DO -->
<article>
   Article content appears here.
   <footer>
   Footer information for article.
   </footer>
</article>
````

###Nav
Representa una sección dedicada a la navegación entre el sitio.
````html
<!-- DON´T -->
<div id="nav">
    <ul>
        <li><a href="#">Item of menu</a></li>
    </ul>
</div>
````
````html
<!-- DO -->
<nav>
    <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="/about/">About</a></li>
    </ul>
</nav>
````

###Estructura basica de elementos
````html
<!-- DO -->
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

###
hola mundo




