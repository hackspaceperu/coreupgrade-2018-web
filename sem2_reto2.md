# Reto 2 de Frontend

## Introducción

Para este segundo reto deberás de construir una página web existente y programarla tú mismo. No te preocupes si los links no van a ningún lado y el campo búsquedas no hace nada. El objetivo es que empieces a pensar sobre cómo los elementos son colocados en una web y cómo son estilizados y alineados. 

Utiliza los “developer tools” del navegador (F12 si usas Google Chrome, o clic derecho en cualquier parte de la web y seleccionas “inspeccionar elemento” te llevará ahí) será tu mejor aliado. Mientras construyes una página en `.html` puedes visualizarla en tu navegador para ver tus avances.

## Intenta Esto Antes de Empezar

Estas habilidades te serán útiles antes de empezar a desarrollar tu web. Intenta hacerlas por tu cuenta o aunque sea asegúrate de que sabes cómo hacerlo:
1. Dos maneras de mover un div por la página.
2. Que un div se quede en la parte superior o en la parte baja de la página.
3. Identifica el color del background de una página existente.
4. Consigue el URL de una imagen de una página web existente.
5. Centra un elemento horizontalmente.
6. Identifica tres maneras en las que puedes incluir estilos CSS en una página.
7. Comprende cómo usar clases e identificadores para dirigir CSS a elementos específicos en la página.
8. Construye un formulario muy básica (incluso si no "va" a ninguna parte).

# Empecemos con el Reto

### Versión fácil: crea la página de inicio de [Google.com](https://www.google.com) (el simple con solo un cuadro de búsqueda).

Crea la carpeta `reto2-web` junto con tu archivo `index.html`

1. Consejos:
	* NO SEA UN PERFECCIONISTA! Simplemente intenta hacer que se vea como `google.com`, no que funcione realmente como tal y no tiene que estar espaciado exactamente del mismo modo pixel a pixel. Cualquier menú desplegable, envío de formularios o resaltado por desplazamiento debe ignorarse.

	* ¡UTILIZA GOOGLE! Probablemente te encontrarás con barricadas en las que no puede encontrar la manera de hacer algo, pero hasa lo que hacen todos los buenos desarrolladores ... ¡Googléalo!

	* Si estás frustrado tratando de obtener botones o entradas para que tengan el estilo que desea (por ejemplo, parece que no responden a ningún estilo), consulta la propiedad css -webkit-appearance: none; o -moz-appearance si estás usando Firefox.
2. Comienza colocando los elementos principales en la página (la imagen del logotipo y el formulario de búsqueda) y luego colóquelos horizontalmente. Puede descargar el logotipo o el enlace de Google directamente a su URL en la web en su etiqueta `<img>`.

3. Luego haz la barra de navegación en la parte superior, primero construye el contenido y luego intenta posicionarlo. Echa un vistazo a  cómo construir una barra de navegación CSS horizontal si estás perdido.

4.Finalmente, coloque el pie de página, que debería ser muy similar a la barra de navegación superior.

5. En general, haz todo lo que puedas antes de confiar en las herramientas de desarrollador (o ver el código fuente de la página) para ayudarte.

6. ¡Lleva tu proyecto a Github usando las instrucciones de arriba!

### Versión difícil (opcional): Compilar [Página de Resultados de Google.com](https://www.google.com/search?q=construye+esta+pagina)

Deberías poder reutilizar gran parte de tu código anterior si comenzaste con este proyecto. De nuevo, no te preocupe por los enlaces a la nada y los formularios que no se enviarán y la codificación estricta de los resultados de la búsqueda (que tendrás que hacer, por supuesto), simplemente concéntrate en la ubicación y el orden de los elementos en la página.

>Nota: Todas las clases y los identificadores y los nombres de los elementos que inspecciona en la página de inicio de Google son cadenas sin sentido (como `<div class='srg'>`). Esto se debe a que el código fue Minificado ([ver una explicación aquí](https://www.hostinger.es/tutoriales/la-minificacion)), que elimina o acorta caracteres y nombres innecesarios para ayudar a que la página cargue más rápido. El archivo HTML (o Javascript o CSS) será más pequeño pero el navegador aún puede leerlo bien.

### Entrega tu reto

Finalmente solo debes enviar el link de `gh-pages` o `rawgit` donde se aprecia tu página web dentro el formulario que está disponible cuando te logueas en el [CoreUpgrade](https://www.hackspace.la).

![Clic en Desarrollo Web](img/send-reto1.png)