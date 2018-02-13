# Unos cuantos ejemplos de uso de Materialize.

### Ordenando las Carpetas y Archivos Necesarios

En vez de empezar con un lienzo en blanco, siempre es bueno ya tener un orden y los archivos mínimos configurados. Es así que empezamos [descargando HTML5 Boilerplate](https://html5boilerplate.com/).

Esto nos da un base con la que empezar.

Además, [descargamos Materialize](http://materializecss.com/getting-started.html) y juntamos el contenido de las dos carpetas en uno solo.

Debería quedar así:

<pre>
HTML5BP+materialize/
  |--css/
  |  |--main.css
  |  |--materialize.css
  |  |--materialize.min.css
  |  |--normalize.css
  |
  |--doc/
  |  |--css.md
  |  |--extend.md
  |  |--faq.md
  |  |--html.md
  |  |--js.md
  |  |--misc.md
  |  |--TOC.md
  |  |--usage.md
  |
  |--font/
  |  |--roboto/
  |
  |--img/
  |  |--.gitignore
  |
  |--js/
  |  |--vendor/
  |  |  |--jquery-3.2.1.min.js
  |  |  |--modernizr-3.5.0.min.js
  |  |--main.js
  |  |--materialize.js
  |  |--materialize.min.js
  |  |--plugin.js
  |
  |--.editorconfig
  |--.gitattributes
  |--.gitignore
  |--.htaccess
  |--404.html
  |--browserconfig.xml
  |--favicon.ico
  |--humans.txt
  |--icon.png
  |--index.html
  |--LICENSE
  |--LICENSE.txt
  |--README.md
  |--robots.txt
  |--tile.png
  |--tile-wide.png
  </pre>

Ahora, lo único que queda es abrir el index.html y linkear el CSS de materialize junto con:
<pre>
&lt;!doctype html&gt;
&lt;html class=&quot;no-js&quot; lang=&quot;&quot;&gt;
    &lt;head&gt;
        &lt;meta charset=&quot;utf-8&quot;&gt;
        &lt;meta http-equiv=&quot;x-ua-compatible&quot; content=&quot;IE=edge,chrome=1&quot;&gt;
        &lt;title&gt;Ejemplos con Materialize&lt;/title&gt;
        &lt;meta name=&quot;description&quot; content=&quot;&quot;&gt;
        &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1&quot;&gt;
        &lt;link rel=&quot;manifest&quot; href=&quot;site.webmanifest&quot;&gt;
        &lt;link rel=&quot;apple-touch-icon&quot; href="icon.png&quot;&gt;
        &lt;!-- Place favicon.ico in the root directory --&gt;

        &lt;!-- Agregamos el Google Icon Font para poder utilizar los íconos de Materialize --&gt;
        &lt;link href=&quot;http://fonts.googleapis.com/icon?family=Material+Icons&quot; rel=&quot;stylesheet&quot;&gt;

        &lt;link rel=&quot;stylesheet&quot; href=&quot;css/normalizecss&quot;&gt;

        &lt;!-- Agregamos materialize.min.css --&gt;
        &lt;link rel=&quot;stylesheet&quot; href=&quot;css/materialize.min.css&quot;&gt;

        &lt;link rel=&quot;stylesheet&quot; href=&quot;css/main.css&quot;&gt;
    &lt;/head&gt;
    &lt;body&gt;
        &lt;!--[if lt IE 8]&gt;
            &lt;p class=&quot;browserupgrade&quot;&gt;You are using an &lt;strong&gt;outdated&lt;/strong&gt; browser. Please &lt;a href=&quot;http://browsehappy.com/&quot;&gt;upgrade your browser&lt;/a&gt; to improve your experience.&lt;/p&gt;
        &lt;![endif]--&gt;

        &lt;p&gt;Hello world! This is HTML5 Boilerplate.&lt;/p&gt;

        &lt;script src=&quot;js/vendor/modernizr-3.5.0.min.js&quot;&gt;&lt;/script&gt;
        &lt;script src=&quot;https://code.jquery.com/jquery-3.2.1.min.js&quot; integrity=&quot;sha256-hwg4gsxgFZhOsEEamdOYGBf13FyQuiTwlAQgxVSNgt4=&quot; crossorigin=&quot;anonymous&quot;&gt;
        &lt;/script&gt; &lt;script&gt;window.jQuery || document.write('&lt;script src=&quot;js/vendor/jquery-3.2.1.min.js&quot;&gt;&lt;\/script&gt;')&lt;/script&gt;
        &lt;script src=&quot;js/plugins.js&quot;&gt;&lt;/script&gt;

        &lt;!-- Agregamos materialize.min.js --&gt;
        &lt;script src=&quot;js/materialize.min.js&quot;&gt;&lt;/script&gt;

        &lt;script src=&quot;js/main.js&quot;&gt;&lt;/script&gt;

        &lt;!-- Google Analytics: change UA-XXXXX-Y to be your site's ID. --&gt;
        &lt;script&gt;
          window.ga=function(){ga.q.push(arguments)};ga.q=[];ga.l=+new Date;
          ga('create','UA-XXXXX-Y','auto');ga('send','pageview')
        &lt;/script&gt;
        &lt;script src=&quot;https://www.google-analytics.com/analytics.js&quot; async defer&gt;&lt;/script&gt;

    &lt;/body&gt;
&lt;/html&gt;
</pre>

Ya con materialize configurado, puedes utilizar cualquier componente de este framework. Es así que pondremos a tu disposición un grupo de videos para que puedas profundizar cada elemento de Materialize.

### CSS Helpers
[Documentación y ejemplos](http://materializecss.com/helpers.html)

<a href="http://www.youtube.com/watch?feature=player_embedded&v=Y_Z2OhK_N2w&feature=youtu.be&t=6s
" target="_blank"><img src="http://img.youtube.com/vi/Y_Z2OhK_N2w/0.jpg" 
alt="Helpers" width="240" height="180" border="10" /></a>


### Imágenes y Videos

[Documentación y ejemplos](http://materializecss.com/media-css.html)

Parte 1:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=eacIJGwi8xQ&feature=youtu.be&t=6s
" target="_blank"><img src="http://img.youtube.com/vi/eacIJGwi8xQ/0.jpg" 
alt="Imagenes y Videos" width="240" height="180" border="10" /></a>

Parte 2:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=oAcHF7CiRhA&feature=youtu.be&t=6s
" target="_blank"><img src="http://img.youtube.com/vi/oAcHF7CiRhA/0.jpg" 
alt="Imagenes y Videos" width="240" height="180" border="10" /></a>


### CSS: Sombras
[Documentación y ejemplos](http://materializecss.com/shadow.html)

<a href="http://www.youtube.com/watch?feature=player_embedded&v=tJ9ZIF7-Dkk&feature=youtu.be&t=6s
" target="_blank"><img src="http://img.youtube.com/vi/tJ9ZIF7-Dkk/0.jpg" 
alt="Sombras" width="240" height="180" border="10" /></a>


### Tablas
[Documentación y ejemplos](http://materializecss.com/table.html)

<a href="http://www.youtube.com/watch?feature=player_embedded&v=YQ-itGMWXuo&feature=youtu.be&t=6s
" target="_blank"><img src="http://img.youtube.com/vi/YQ-itGMWXuo/0.jpg" 
alt="Tablas" width="240" height="180" border="10" /></a>                     


### Tipografía
[Documentación y ejemplos](http://materializecss.com/typography.html)

<a href="http://www.youtube.com/watch?feature=player_embedded&v=kzfF6ZhTVEE&feature=youtu.be&t=18s
" target="_blank"><img src="http://img.youtube.com/vi/kzfF6ZhTVEE/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>


### Íconos
[Documentación y ejemplos](http://materializecss.com/icons.html).

<a href="http://www.youtube.com/watch?feature=player_embedded&v=hFowBrHjOGk&feature=youtu.be&t=6s
" target="_blank"><img src="http://img.youtube.com/vi/hFowBrHjOGk/0.jpg" 
alt="Íconos" width="240" height="180" border="10" /></a>


### Componentes: Tarjetas
[Documentación y ejemplos](http://materializecss.com/cards.html).

<a href="http://www.youtube.com/watch?feature=player_embedded&v=_ghV6QA1FNw&feature=youtu.be&t=18s
" target="_blank"><img src="http://img.youtube.com/vi/_ghV6QA1FNw/0.jpg" 
alt="Tarjetas" width="240" height="180" border="10" /></a>           


### Componentes: Footer
[Documentación y ejemplos](http://materializecss.com/footer.html).

<a href="http://www.youtube.com/watch?feature=player_embedded&v=DMbnVw5YoWc&feature=youtu.be&t=18s
" target="_blank"><img src="http://img.youtube.com/vi/DMbnVw5YoWc/0.jpg" 
alt="Footer" width="240" height="180" border="10" /></a>


### Componentes: Barra de Navegacción (Navbar)
[Documentación y ejemplos](http://materializecss.com/navbar.html).

<a href="http://www.youtube.com/watch?feature=player_embedded&v=14gOldsVACc&feature=youtu.be&t=6s
" target="_blank"><img src="http://img.youtube.com/vi/14gOldsVACc/0.jpg" 
alt="Navbar" width="240" height="180" border="10" /></a>              


### Componentes: Formularios
[Documentación y ejemplos](http://materializecss.com/forms.html).

<a href="http://www.youtube.com/watch?feature=player_embedded&v=Ykx19ugkvi0w&feature=youtu.be&t=18s
" target="_blank"><img src="http://img.youtube.com/vi/kx19ugkvi0w/0.jpg" 
alt="Formularios" width="240" height="180" border="10" /></a>


### Componentes: Botones
[Documentación y ejemplos](http://materializecss.com/buttons.html)

<a href="http://www.youtube.com/watch?feature=player_embedded&v=YQrr7GGV4uVE&feature=youtu.be&t=6s
" target="_blank"><img src="http://img.youtube.com/vi/Qrr7GGV4uVE/0.jpg" 
alt="Botones" width="240" height="180" border="10" /></a>


### Componentes: Colecciones, Listas
[Documentación y ejemplos](http://materializecss.com/collections.html)

<a href="http://www.youtube.com/watch?feature=player_embedded&v=YIZ47U2o9-k&feature=youtu.be&t=18s
" target="_blank"><img src="http://img.youtube.com/vi/YIZ47U2o9-k/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>


### Componentes: Insignias (Badges)
[Documentación y ejemplos](http://materializecss.com/badges.html)

<a href="http://www.youtube.com/watch?feature=player_embedded&v=-FcQk0sAty4&feature=youtu.be&t=18s
" target="_blank"><img src="http://img.youtube.com/vi/-FcQk0sAty4/0.jpg" 
alt="Insignias" width="240" height="180" border="10" /></a>

[Continuar al reto](sem3_reto4.md)