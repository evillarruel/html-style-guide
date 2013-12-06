html-style-guide
================

MercadoLibre HTML Style Guide


##HTML5
It’s the combination of new elements of markup or syntax. These elements suppose more advanced tools, which translates as better experiences for the user. 

###Advantages of use HTML5
* As the code is simpler and plain, allows a faster load. 
* Adds tags to handle semantics full and homogeneous, allowing  to describe which is the content, their importance and purpose. These tags have no particular impact on display and are orient to searchers. 
* Allows better indexing and interpretation of information.
* Allows to interact with multimedia elements like audio and video.

### New rules of semantics
* Is not necessary to close the following tags.

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

* The document declaration is fully minimized.

````html
<!-- DO -->
<!DOCTYPE html>
````

* Allows both lowercase and capital letters in the code.

###New elements of HTML5
The HTML5 markup incorporates some new tags designed to make web pages structure more logical and functional.

````html
<header> <nav> <article> <section> <aside> <footer> <audio> <canvas> <command> <datalist> <details> <dialog> <embed> <figure> <mark> <meter> <output> <progress> <ruby> <rp> <rt> <source> <time> <video>
````
####Header
Represents the header of a section, and it is assumed to be given more importance than the rest, especially if the section is an ítem.
````html
<header>  
    <h1>MercadoLibre - Where you buy and sell everything</h1>
    <!-- Header content -->
</header>
````

####Nav
Represents a section dedicated to the navigation of the site.
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
####Article
Allows to declare a part of the content which is independent of this, such as reviews.
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
Represents a general section inside a document or an application.  It can contain subsections and if we accompany with h1-h6 we could structure better the entire page.
````html
<!-- DO -->
<section>
    <h1>Promotions</h1>
    <p>Promo description</p>
</section>
````

####Aside
Represents a content which is not much related to the rest of the page, as a sidebar. It is essential to define the “important content" from the “support content", giving more importance to the first that the second.

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

The content of the ```` aside ```` element is related directly with the article.
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

The ```` aside ````element can be out of the article. Its content is related to the page, but not so closely to the article.
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
Represents the bottom of a section with information about the page/section that has little to do with the content itself but has data like the author, copyright or the year.

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
#####The footer inside another element
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

###Basic structure of elements
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
    
    
