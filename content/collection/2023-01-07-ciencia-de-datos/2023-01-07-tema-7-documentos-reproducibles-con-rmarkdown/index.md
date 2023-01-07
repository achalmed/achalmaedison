---
title: 'Tema 7: Documentos reproducibles con **Rmarkdown**'
author: Edison Achalma Mendoza
date: '2023-01-07'
slug: tema-7-documentos-reproducibles-con-rmarkdown
categories: []
tags: []
---

<script src="{{< blogdown/postref >}}index_files/clipboard/clipboard.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/primer-tooltips/build.css" rel="stylesheet" />
<link href="{{< blogdown/postref >}}index_files/klippy/css/klippy.min.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/klippy/js/klippy.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/twitter-widget/widgets.js"></script>
<script src="{{< blogdown/postref >}}index_files/twitter-widget/widgets.js"></script>

<link href="{{< blogdown/postref >}}index_files/vembedr/css/vembedr.css" rel="stylesheet" />

<script>
  addClassKlippyTo("pre.r, pre.markdown");
  addKlippy('right', 'top', 'auto', '1', 'Copy code', 'Copied!');
</script>

------------------------------------------------------------------------

<br>

# 1. Introducción

El proceso habitual para hacer un informe (o unas transparencias) en el que aparezcan gráficos o tablas resumen de algún análisis estadístico consiste en :

1.  Escribir el texto en un programa (Word, Powerpoint, Prezi, etc.)
2.  Realizar los cálculos estadísticos y gráficos en otro programa (R, Stata, Eviews, etc.)
3.  Pegar los gráficos y tablas en el documento de texto.

Este proceso tiene ciertas desventajas: dificulta la investigación reproducible y puede ser tedioso de rehacer si por ejemplo cambian ligeramente los datos, etc.

<br>

**En R es posible realizar todo el informe**, tanto la escritura del texto como la realización de los cálculos y gráficos, **en un único documento**. Hay varias formas de hacerlo, pero nos centraremos en los documentos RMarkdown (.Rmd).

Los **documentos RMarkdown (.Rmd)** facilitan mucho la realización de informes y transparencias ya que permiten combinar texto, código y resultados de la evaluación del código en un único documento. Si por ejemplo cambian los datos sólo habría que cambiar la ruta a los nuevos datos y el informe (gráficos, tablas etc…) se volvería a generar automáticamente con los nuevos datos.

La razón para hacer los análisis reproducibles no sólo es cumplir con los estándares científicos, que también, sino también hay un interés personal para el analista. Para entenderlo puedes ver el siguiente [video de 1’44’’](https://www.youtube.com/watch?v=s3JldKoA0zw&feature=youtu.be) que muestra una de las principales ventajas de usar documentos `.Rmd`.

Hace poco David Keyes pregunto en Twitter a la comunidad R cuales eran los principales beneficios de usar ficheros .Rmd para tus investigaciones/informes:

<blockquote class="twitter-tweet" align="center" data-width="400" data-lang="en" data-dnt="true" data-theme="light"><p lang="en" dir="ltr">Help me out <a href="https://twitter.com/hashtag/rstats?src=hash&amp;ref_src=twsrc%5Etfw">#rstats</a> hive mind. I&#39;ve been asked to explain the benefits of RMarkdown. I&#39;m developing a list on a continuum from simple (i.e. do what you currently do, just better) to complex (i.e. completely transform how you work). Here &#39;tis:</p>&mdash; David Keyes (@dgkeyes) <a href="https://twitter.com/dgkeyes/status/1101554699566641152?ref_src=twsrc%5Etfw">March 1, 2019</a></blockquote>

Con las respuestas al tweet, David elaboró [este post](https://rfortherestofus.com/2019/03/r-killer-feature-rmarkdown/).

<br>

Ya hemos trabajado con algunos **documentos Rmarkdown** (`.Rmd`); de hecho, todos los tutoriales del curso (incluido éste que estás viendo) se han elaborado usando ficheros .Rmd. Los tutoriales se escriben en ficheros RMarkdown, pero estos ficheros .Rmd se convierten a html, que suele ser el formato final en el que se muestran los tutoriales. En RStudio el proceso de conversión de .Rmd a .html consiste simplemente en pinchar un botón; además, simplemente cambiando una linea podemos convertir los documentos .Rmd a una gran variedad de formatos: html, pdf, word, ioslides, beamer, etc…

Si quieres ver algunos ejemplos de la gran variedad de formatos a los que puedes transformar un documento .Rmd ve a la siguiente [galería](http://rmarkdown.rstudio.com/gallery.html). Para iniciarte en el universo Rmarkdown puedes consultar [`R Markdown: The Definitive Guide`](https://bookdown.org/yihui/rmarkdown/).

<br>

#### Proceso para convertir los .Rmd a otro(s) formatos \[OPCIONAL\]

Como trabajamos con RStudio, en la práctica, procesar los ficheros .Rmd consistirá solamente en pinchar en el icono `Knit`[^1]. Muy fácil!!

No es necesario, pero quizá os interese saber cómo se procesan realmente los ficheros .Rmd para acabar convirtiéndose en html, pdf, etc.

La respuesta es que se ocupa de ello el paquete [`rmarkdown`](https://github.com/rstudio/rmarkdown) que llama otro paquete de R, [`knitr`](https://yihui.name/knitr/) y a un programa llamado [`pandoc`](https://es.wikipedia.org/wiki/Pandoc). Si quieres más detalles puedesir [aquí](https://stackoverflow.com/questions/40563479/relationship-between-r-markdown-knitr-pandoc-and-bookdown)

**En palabras:** knitr se ocupa de ejecutar todos los trozos con código R que haya en el fichero .Rmd, después de ejecutar el código, pegará los resultados de la evaluación del código (gráficos, tablas etc…) junto con el texto en un documento intermedio (con extensión .md), para después transferir, con la ayuda del paquete `rmarkdown`, este documento .md a `pandoc` que se encargará de traducirlo al formato elegido (html, pdf, …)[^2]. Knitr sabe diferenciar el texto del código R porque éste se señaliza con unas marcas.

**Visualmente:**

<br>

------------------------------------------------------------------------

# 2 Creando .Rmd’s en RStudio

En la práctica, RStudio facilita mucho la creación de documentos Rmarkdown. Para generar un documento .Rmd basta con seguir la siguiente ruta de menús: `File > New File > R Markdown ...`

Se abrirá una ventana que nos solicitará un título y un autor para nuestro .Rmd, así como el formato de salida.

Cuando aceptemos nos generará un documento/plantilla para nuestro .Rmd. Si queremos procesarlo o “knitearlo” tendremos que hacer click en el icono **`Knit`**

<br>

------------------------------------------------------------------------

# 3. ¿Qué son los documentos .Rmd?

Son simplemente ficheros de texto (se pueden escribir en cualquier editor de texto, por ejemplo Notepad); PERO **facilitan mucho la tarea de generar informes o transparencias** con contenido estadístico, ya que permiten mezclar en un mismo documento texto y código R.

El código R (así como los resultados de la evaluación del código) se mostrarán automáticamente (gracias a `knitr`) en el documento final; de esta forma, se facilita mucho la realización de informes y transparencias ya que evita el tener que ir copiando los resultados (tablas, gráficos etc…) en el informe.

<br>

Veamos un **ejemplo** con un documento Rmarkdown muy sencillo:

<br>

Como veis, los documentos Rmarkdown tienen 3 partes o elementos:

- encabezamiento
- trozos de código R
- texto

Luego hablaremos de ellas. Antes veamos como quedaría el documento .Rmd tras ser procesado por knitr (“kniteado”). Tras pasar por knitr y pandoc se generará un documento .html que se verá así:

Como veis, el chunk con código R `summary(iris)` se ha ejecutado y se ha mostrado tanto el código como el resultado de su evaluación en unas cajas de texto.

<br>

------------------------------------------------------------------------

# 4. Partes de los ficheros .Rmd

Los documentos Rmarkdown tienen 3 partes o elementos:

- Encabezamiento o YAML header
- Trozos de código R(chunks)
- Texto (escrito en markdown)

Veámoslas una a una.

<br>

------------------------------------------------------------------------

## Encabezamiento (YAML header)

<br>

Abajo tenéis un ejemplo sencillo de un YAML header:

<br>

Como podéis imaginar, el encabezamiento se coloca **al principio del documento y comienza y acaba con una marca de 3 guiones**: **`---`**

En el encabezamiento se introducen elementos básicos del documento como el título, el autor, fecha, y el formato de salida del documento. En el ejemplo hemos elegido como formato de salida `html`; si preferimos pdf, habría que sustituir `output: html_document` por `output: pdf_document`

<br>

El YAML header puede incluir otros elementos para personalizar un poco más el documento final o output. Abajo tenéis un ejemplo más complejo de un YAML header. Es el que utilizo para hacer los tutoriales del curso.

En [este post](https://scienceloft.com/technical/useful-yaml-options-for-generating-html-reports-in-r/) y en [esta vignette](https://ymlthis.r-lib.org/articles/yaml-fieldguide.html) del paquete `ymlthis` tienes más opciones/posibilidades a especificar en el YAML.

<br>

------------------------------------------------------------------------

## Chunks (o código R)

<br>

Los trozos de código R o chunks permiten hacer análisis estadísticos y mostrar los resultados en el documento final.

Para que knitr distinga las instrucciones de R del texto normal **tenemos que poner las instrucciones de R dentro de unas marcas** o identificadores: ```` ```{r} ```` al principio y ```` ``` ```` al final.

Por ejemplo:

Knitr interpreta ese trozo de texto como instrucciones de R porque van dentro de las marcas, y hará que R las ejecute y muestre los resultados en el documento final.

<br>

Los chunks pueden tienen diversas opciones que permiten una mayor flexibilidad en como se muestra el código y los resultados en el documento final. Las opciones más usadas son:

- echo
- eval

<br>

Por ejemplo, si introducimos este texto en nuestro fichero .Rmd:

En este caso, se mostrará el chunk(`echo = TRUE`) y también se evaluará (`eval = TRUE`) y, por tanto, se mostrarán los resultados en el documento final. Se verá algo como:

``` r
summary(iris)
#>   Sepal.Length    Sepal.Width     Petal.Length    Petal.Width   
#>  Min.   :4.300   Min.   :2.000   Min.   :1.000   Min.   :0.100  
#>  1st Qu.:5.100   1st Qu.:2.800   1st Qu.:1.600   1st Qu.:0.300  
#>  Median :5.800   Median :3.000   Median :4.350   Median :1.300  
#>  Mean   :5.843   Mean   :3.057   Mean   :3.758   Mean   :1.199  
#>  3rd Qu.:6.400   3rd Qu.:3.300   3rd Qu.:5.100   3rd Qu.:1.800  
#>  Max.   :7.900   Max.   :4.400   Max.   :6.900   Max.   :2.500  
#>        Species  
#>  setosa    :50  
#>  versicolor:50  
#>  virginica :50  
#>                 
#>                 
#> 
```

<br>

Mientras que si en el .Rmd escribimos lo siguiente:

Se mostrará el código (`echo = TRUE`), pero no se evaluará (`eval = FALSE`) y ,por lo tanto, no se mostrarán los resultados en el documento final.

<br>

Si en el .Rmd escribimos lo siguiente:

NO se mostrará el código (`echo = FALSE`), pero SÍ se evaluará (`eval = FALSE`) y ,por lo tanto, SI se mostrarán los resultados en el documento final.

<br>

Si en el .Rmd escribimos lo siguiente:

NO se mostrará el código (`echo = FALSE`), SI se evaluará (`eval = FALSE`), PERO como `results = "hide"` NO se mostrarán los resultados en documento final.

<br>

Hay más opciones sobre los chunks que nos permiten una mayor flexibilidad sobre como mostrar los resultados y el código; pero si quieres ver todas las opciones tendrás que ir a la [página web de knitr](https://yihui.name/knitr/options/) o al [cheat sheet sobre Rmarkdown](https://www.rstudio.com/wp-content/uploads/2016/03/rmarkdown-cheatsheet-2.0.pdf).

Una opción útil es `include = FALSE`; en este caso, el chunk se ejecutará, pero ni se mostrará en el documento final ni se mostrarán los resultados de la ejecución del código. Esta opción es muy útil para los chunks que se utilizan para hacer el “setup”.

Generalmente los documentos .Rmd tienen un primer chunk (chunk de setup) donde se fijan opciones globales para los chunks, fijra opciones globales, incluso se puede utilizar para cargar paquetes básicos como el `tidyverse`. Por ejemplo este suele ser el primer chunk en mis documentos .RMd:

<br>

Con la llegada de [`knitr v1.35`](https://github.com/yihui/knitr/releases) disponemos de una nueva forma de especificar las opciones de los chunks.

<blockquote class="twitter-tweet" align="center" data-width="550" data-lang="en" data-dnt="true" data-theme="light"><p lang="es" dir="ltr">Si vas a pasar el tiempo tratando de humillarme, haciendo que la clase sea innecesariamente dura, entonces mejor me voy, pero si de verdad quieres hacer el esfuerzo de ser un buen maestro entonces yo también estoy dispuesto a intentarlo.</p>&mdash; Edison Achalma (@achalmaedison) <a href="https://twitter.com/achalmaedison/status/1597228787431002113?ref_src=twsrc%5Etfw">November 28, 2022</a></blockquote>

<br>

------------------------------------------------------------------------

## El texto (en Rmarkdown)

<br>

La parte principal de un informe suele ser texto (narratives). En un fichero .Rmd, todo lo que no sea encabezamiento o chunks será interpretado por knit como texto y lo mostrará tal cual; es decir, como texto.

Aquí podríamos acabar nuestro tutoría sobre como escribir texto en un fichero .Rmd; pero generalmente en un texto queremos resaltar ciertas palabras con negrita, o ponerlas en cursiva, o poner un titulo de sección y de sub-secciones. Todo esto lo tendremos que hacer utilizando **Markdown**. Markdown es un lenguaje de marcas ligero y muy sencillo de aprender (lo básico se aprende en unos 10 minutos) pero muy utilizado. Es posible que alguno de vosotros haya utilizado una variante de Markdown al escribir en negrita en Whatsapp.

El texto de un documento .Rmd es “simplemente” texto PERO está escrito en **Markdown**. Ahora lo veremos, pero antes vamos a ver un poco más sobre qué es Markdown.

<br>

#### ¿Qué es Markdown? \[OPCIONAL\]

Mardown es un lenguaje de marcado ligero ideado en 2004 por Jhon Grueber y [Aaron Swartz](https://es.wikipedia.org/wiki/Aaron_Swartz). Hay diversas variantes de Markdown, [aquí](https://blog.codinghorror.com/standard-markdown-is-now-common-markdown/) peuedes leer sobre un intento de estandarización.

Podemos pensar que Markdown es un método de escritura[^3]: evidentemente sirve para escribir. La ventaja de escribir en Markdown es que es un lenguaje muy fácil de aprender y que como está basado en un formato de texto plano, es y será compatible con la mayoría de plataformas.

La mayoría de vosotros escribís en Word. Es muy fácil escribir en Word pero un archivo word solo es posible leerlo en el programa WORD de Microsoft. Si intentas abrir un documento .doc en Notepad, éste será completamente ilegible; sin embargo, la mayoría de plataformas y servicios web saben interpretar y mostrar correctamente un documento escrito en Markdown.

Lo que escribas en Rmarkdown se mostrará tal cual en el documento final, pero lo más habitual es que quieras dar un poco de formato el texto: negritas, cursivas, listas, enlaces de internet, etc…

Todos estos formatos (negrita, …) se introducen en rmarkdown con marcas; por ejemplo si quieres que una palabra se resalte en negritas tienes que escribirla enmarcada en `**`: **`**esto se mostraría en negrita**`**

Para aprender las principales reglas de Rmarkdown podéis usar un [editor on-line de Markdown](https://vuejs.org/v2/examples/) y probar a escribir algo.

En este otro [tutorial de Markdown](https://www.markdowntutorial.com/), se puede leer lo siguiente:

> Markdown is a way to write content for the web. It’s written in what nerds like to call “plaintext”, which is exactly the sort of text you’re used to writing and seeing. Plaintext is just the regular alphabet, with a few familiar symbols. Unlike cumbersome word processing applications, text written in Markdown can be easily shared between computers, mobile phones, and people. It’s quickly becoming the writing standard for academics, scientists, writers, and many more. Websites like GitHub and reddit use Markdown to style their comments.

##### Aquí tienes algunas reglas de Markdown

<br>

# 5. Más cosas de RMarkdown

En la página web de Markdown, concretamente [aquí](https://daringfireball.net/projects/markdown/syntax#html) nos avisan de lo siguiente:

> Markdown is not a replacement for HTML, or even close to it. Its syntax is very small, corresponding only to a very small subset of HTML tags … The idea for Markdown is to make it easy to read, write, and edit prose. HTML is a publishing format; Markdown is a writing format. Markdown was not designed to solve everything.

A pesar de que, como nos avisó Jhon Grueber, el desarrollador de Markdown, Markdown no está diseñado para resolver todas las necesidades de un escritor/científico, en Rmarkdown se pueden introducir también elementos como:

### Ecuaciones

Se pueden introducir formulas matemáticas escritas en Látex. Para formulas en linea se usa la marca `$` y para formulas independientes se usa `$$`.

- Para fórmulas en linea (o dentro del texto) se utiliza la marca `$` al principio y final de la formula. Por ejemplo `$\sum_{i=1}^n X_i$` se mistaría así: `\(\sum_{i=1}^n X_i\)`. Ves, la formula está dentro del texto, en una linea del texto.

- Para presentar una ecuación independiente (en una linea independiente), se usa la marca `$$` al principio y final de la formula. Si escribes `$$E = mc^{2}$$`, se mostrará en una linea independiente tal que así:

`$$E = mc^{2}$$`

¿Que pasa, que no sabes escribir formulas o ecuaciones en Latex? Yo tampoco mucho, pero puedes utilizar un programa como [Lyx](https://www.lyx.org/), o mucho más fácil, puedes utilizar algún editor online de Latex, por ejemplo: [este](http://www.sciweavers.org/free-online-latex-equation-editor) o [este](https://www.latex4technics.com/). En [este libro](https://dereksonderegger.github.io/570L/16-rmarkdown-tricks.html) tienen algunos ejemplos de ecuaciones en Latex.

Recientemente, el paquete [`equatiomatic`](https://github.com/datalorax/equatiomatic) permite obtener fácilmente la ecuación de un modelo:

``` r
# remotes::install_github("datalorax/equatiomatic")
library(equatiomatic)

# Fit a simple model
mod1 <- lm(mpg ~ cyl + disp, mtcars)

# Give the results to extract_eq
extract_eq(mod1)
```

$$
\operatorname{mpg} = \alpha + \beta_{1}(\operatorname{cyl}) + \beta_{2}(\operatorname{disp}) + \epsilon
$$

También de un modelo estimado:

``` r
extract_eq(mod1, use_coefs = TRUE)
```

$$
\operatorname{\widehat{mpg}} = 34.66 - 1.59(\operatorname{cyl}) - 0.02(\operatorname{disp})
$$

<br>

### Imágenes

Para mostrar una imagen basta con poner:

    ![Una imagen chula](./imagenes/img1.jpeg) 

Aunque yo prefiero hacerlo así:

    ```{r eval = TRUE, echo = TRUE}
    knitr::include_graphics(here::here("imagenes", "rmarkdown_ejemplos", "imagenes", "fucking_ages_image.jpeg")  )
    ```

### Hyperlinks

Para poner hyperlinks se puede escribir lo siguiente: `<http://www.wikipedia.es>` y se mostrará así: <http://www.wikipedia.es>

Pero es mejor ponerlo así: `[enlace a la Wikipedia](http://www.wikipedia.es)` y se mostrará así: <a href="http://www.wikipedia.es" target="_blank">enlace a la Wikipedia</a>.

Si quieres que el enlace se abra en el navegador en una página nueva has de añadir `{target="_blank"}`

### Notas al pie de página

Para poner notas al pie has de poner `[^1]` y luego al final del documento poner `[^1]: esto es una nota al pie.`, y se verá esto: [^4]

O alternativamente poner, en el sitio del texto donde quieras insertar una nota al pie, esta marca: `^[el texto que quiero que se lea en la nota al pie]` y se mostrará como una nota al pie.

### Tablas

Habrá un tutorial especifico para tablas, pero para mostrar una tabla, lo más básico y sencillo es utilizar la función `knitr::kable()`:

    ```{r}   
    knitr::kable(summary(iris))    
    ```    

|     | Sepal.Length  | Sepal.Width   | Petal.Length  | Petal.Width   | Species       |
|:----|:--------------|:--------------|:--------------|:--------------|:--------------|
|     | Min. :4.300   | Min. :2.000   | Min. :1.000   | Min. :0.100   | setosa :50    |
|     | 1st Qu.:5.100 | 1st Qu.:2.800 | 1st Qu.:1.600 | 1st Qu.:0.300 | versicolor:50 |
|     | Median :5.800 | Median :3.000 | Median :4.350 | Median :1.300 | virginica :50 |
|     | Mean :5.843   | Mean :3.057   | Mean :3.758   | Mean :1.199   | NA            |
|     | 3rd Qu.:6.400 | 3rd Qu.:3.300 | 3rd Qu.:5.100 | 3rd Qu.:1.800 | NA            |
|     | Max. :7.900   | Max. :4.400   | Max. :6.900   | Max. :2.500   | NA            |

<br>

# 6. Aún más cosas

Hay más cosas, como referencias bibliográficas, pero ya será para el segundo curso de R o lo tendrás que aprender por tu cuenta en [`R Markdown: The Definitive Guide`](https://bookdown.org/yihui/rmarkdown/).

A pesar de que Markdown permite formatear el texto, en ciertos sentidos es limitado; pero si quieres aún más flexibilidad en el output, tendrás que aprender html y mejor html+CSS.

<br>

**Algunos ejemplos:**

1.  Si quieres introducir un párrafo en otro color tendrás que hacerlo en html, tendrás que escribir: `<FONT COLOR="Red">Esto se mostrará en ROJO!!</FONT>`

    <FONT COLOR="Red">Esto se mostrará en ROJO!!</FONT>

<br>

2.  si quieres centrar un párrafo, tendrás que escribir: `<CENTER>Este párrafo irá centrado</CENTER>`

<CENTER>
Este párrafo irá centrado
</CENTER>

<br>

3.  Puedes insertar en tu documento (sólo si el output es html) una página web completa, para ello has de escribir: `<iframe src="http://www.eldiario.es/" height="400" width="800"></iframe>`

<br>

<iframe src="http://www.eldiario.es/" height="400" width="800">
</iframe>

<br>

4.  Un vídeo. Has de escribir: `<iframe width="560" height="315" src="https://www.youtube.com/embed/ACv9zaBa1A4" frameborder="0" allowfullscreen></iframe>`

<div class="vembedr">
<div>
<iframe src="https://www.youtube.com/embed/ACv9zaBa1A4" width="533" height="300" frameborder="0" allowfullscreen="" data-external="1"></iframe>
</div>
</div>

Aunque también hay un paquete, al menos, que facilita la inserción de videos en documentos .Rmd: es el paquete [`vembedr`](https://ijlyttle.github.io/vembedr/articles/vembedr.html).

<br>

------------------------------------------------------------------------

<br>

## Aún más cosas (II)

- El paquete [`demoR`](https://github.com/kbodwin/demoR) ayuda a presentar el código R en documentos Rmd. Por ejemplo, permite marcar/highligt algunas partes de una sentencia o código R. Para aprender puedes ir a la [viñeta](https://web.calpoly.edu/~kbodwin/demoR/articles/demoR.html) del paquete. Por ejemplo, en el próximo chunk voy a marcar en amarillo el operador pipe `%>%`

- Podemos [usar iconos](https://ropensci.org/technotes/2018/05/15/icon/) en nuestros Rmds. Por ejemplo: `ricons::icon_style(icons::fontawesome("rocket"), fill = "#1FA67A")` +
  `ricons::icon_style(icons::fontawesome("r-project"), fill = "#384CB7")` =
  `ricons::icon_style(icons::fontawesome("heart"), fill = "red")`

- Podemos usar cajas de colores para resaltar un trozo de texto por ejemplo para poner conclusiones. Esto lo aprendí [aquí](https://holtzy.github.io/Pimp-my-rmd/#figures_caption). En este [otro post](https://desiree.rbind.io/post/2019/making-tip-boxes-with-bookdown-and-rmarkdown/) nos enseñan a hacer esos cuadros realmente bonitos.

<style>
div.blue {background-color:#e6f0ff; border-radius: 5px; padding: 20px;}
</style>

<div class="blue">

**Conclusiones:**  
- This is my first conclusion
- This is my second conclusion

</div>

- si queremos que los chunks puedan copiarse en el portapapeles, podemos usar el paquete [`klippy`](https://rlesur.github.io/klippy/index.html)

``` r
klippy::klippy()  #- remotes::install_github("rlesur/klippy")
```

## Aún más cosas (III)

- Puedes cambiar algunos aspectos de tu documento html. Puedes verlo [aquí](https://bookdown.org/yihui/rmarkdown/html-document.html#appearance-and-style.)

- Con CSS se puede personalizar completamente el aspecto de los documentos html que se generan con Rmarkdown. Aunque no sepas CSS tienes una gran variedad de formatos predefinidos. Puedes ver un listado [aquí](https://www.datadreaming.org/post/r-markdown-theme-gallery/), [aquí](https://github.com/gadenbuie/cleanrmd)o [aquí](https://github.com/juba/rmdformats).

- El paquete [bslib](https://rstudio.github.io/bslib/) facilita el tuneado de los html.

- El paquete [thematic](https://rstudio.github.io/thematic/) puede hacer que los gráficos reflejen el theme de RStudio que estas usando: sólo hay que hacer `thematic_on()`

- El paquete [checkdown](https://agricolamz.github.io/checkdown/) permite crear campos y casillas de verificación. Por ejemplo:

<!-- -->

    ¿Cuanto es 7 + 2?

<form name="form_29902" onsubmit="return validate_form_29902()" method="post">
<input type="text" name="answer_29902"><br><input type="submit" value="check">
</form>
<p id="result_29902">
</p>
<script> function validate_form_29902() {var x, text; var x = document.forms["form_29902"]["answer_29902"].value;if (x == "9"){text = 'Acertaste!!!';} else {text = 'no way';} document.getElementById('result_29902').innerHTML = text; return false;} </script>

- Puedes incluir páginas web con `knitr::include_url()` , shiny’s con `knitr::include_app ()` e imágenes con `knitr::include_graphics()`

- El paquete [fontawesome](https://github.com/rstudio/fontawesome) permite incluir iconos de [**Font Awesome**](https://fontawesome.com/) en documentos RMarkdown. Por ejemplo con `` ` fontawesome::fa("r-project", fill = "steelblue")` `` podemos insertar el icono de <svg aria-hidden="true" role="img" viewBox="0 0 581 512" style="height:1em;width:1.13em;vertical-align:-0.125em;margin-left:auto;margin-right:auto;font-size:inherit;fill:steelblue;overflow:visible;position:relative;"><path d="M581 226.6C581 119.1 450.9 32 290.5 32S0 119.1 0 226.6C0 322.4 103.3 402 239.4 418.1V480h99.1v-61.5c24.3-2.7 47.6-7.4 69.4-13.9L448 480h112l-67.4-113.7c54.5-35.4 88.4-84.9 88.4-139.7zm-466.8 14.5c0-73.5 98.9-133 220.8-133s211.9 40.7 211.9 133c0 50.1-26.5 85-70.3 106.4-2.4-1.6-4.7-2.9-6.4-3.7-10.2-5.2-27.8-10.5-27.8-10.5s86.6-6.4 86.6-92.7-90.6-87.9-90.6-87.9h-199V361c-74.1-21.5-125.2-67.1-125.2-119.9zm225.1 38.3v-55.6c57.8 0 87.8-6.8 87.8 27.3 0 36.5-38.2 28.3-87.8 28.3zm-.9 72.5H365c10.8 0 18.9 11.7 24 19.2-16.1 1.9-33 2.8-50.6 2.9v-22.1z"/></svg> para instalar usar install.packages(“fontawesome”)

<br>

------------------------------------------------------------------------

<br>

# 7. Investigación reproducible y Rmd

Hemos hablado muy poco de investigación reproducible pero, es evidente que usar documentos `.Rmd` y trabajar con `Rprojects` facilita la investigación reproducible. No la garantiza del todo, para ello habría que ver/usar más herramientas (docker, packrat, github, …). No lo vamos a hacer, pero al menos señalar dos prácticas que facilitan que tus análisis se acerquen a ser reproducibles:

<br>

1.  Cuando estás haciendo un análisis y quieres compartirlo hay que estar seguro de los packages que se necesitan cargar para replicarlo, por eso es bueno hacer el análisis desde una sesión nueva/fresca de R y cargar los paquetes al principio del script. Para ello, puede ser de utilidad saber que paquetes tienes cargados en un momento dado, y puedes saberlo con: `(.packages())`.

2.  A pesar de que yo no lo suelo hacer (`remo::ji("-1")`), es recomendable introducir al final de los ficheros `.Rmd` la siguiente instrucción: `sessionInfo()`. De esta forma, proporcionarás información sobre que ordenador, sistema operativo y versión de R utilizaste en tu análisis, así como de las opciones locales de tu sistema (idioma, etc …) y de los paquetes que tienes cargados en memoria. Por ejemplo, ahora mismo mi sessionInfo es:

<br>

``` r
sessionInfo()
```

    #> R version 4.0.4 (2021-02-15)
    #> Platform: x86_64-pc-linux-gnu (64-bit)
    #> Running under: Parrot OS 5.1 (Electro Ara)
    #> 
    #> Matrix products: default
    #> BLAS:   /usr/lib/x86_64-linux-gnu/openblas-pthread/libblas.so.3
    #> LAPACK: /usr/lib/x86_64-linux-gnu/openblas-pthread/libopenblasp-r0.3.13.so
    #> 
    #> locale:
    #>  [1] LC_CTYPE=es_PE.UTF-8       LC_NUMERIC=C              
    #>  [3] LC_TIME=es_PE.UTF-8        LC_COLLATE=es_PE.UTF-8    
    #>  [5] LC_MONETARY=es_PE.UTF-8    LC_MESSAGES=es_PE.UTF-8   
    #>  [7] LC_PAPER=es_PE.UTF-8       LC_NAME=C                 
    #>  [9] LC_ADDRESS=C               LC_TELEPHONE=C            
    #> [11] LC_MEASUREMENT=es_PE.UTF-8 LC_IDENTIFICATION=C       
    #> 
    #> attached base packages:
    #> [1] stats     graphics  grDevices utils     datasets  methods   base     
    #> 
    #> other attached packages:
    #>  [1] icons_0.2.0        demoR_0.0.0.9000   vembedr_0.1.5      equatiomatic_0.3.1
    #>  [5] forcats_0.5.1      stringr_1.4.0      dplyr_1.0.10       purrr_0.3.4       
    #>  [9] readr_1.4.0        tidyr_1.2.1        tibble_3.1.8       ggplot2_3.4.0     
    #> [13] tidyverse_1.3.0   
    #> 
    #> loaded via a namespace (and not attached):
    #>  [1] httr_1.4.2        sass_0.4.4        jsonlite_1.7.2    modelr_0.1.8     
    #>  [5] bslib_0.4.2       shiny_1.5.0       assertthat_0.2.1  highr_0.8        
    #>  [9] cellranger_1.1.0  yaml_2.2.1        pillar_1.8.1      backports_1.2.1  
    #> [13] glue_1.6.2        digest_0.6.27     promises_1.1.1    rvest_0.3.6      
    #> [17] colorspace_2.0-0  htmltools_0.5.4   httpuv_1.5.5      pkgconfig_2.0.3  
    #> [21] tweetrmd_0.0.9    broom_0.7.4       haven_2.3.1       bookdown_0.31    
    #> [25] xtable_1.8-4      scales_1.2.1      fontawesome_0.4.0 later_1.1.0.1    
    #> [29] timechange_0.1.1  generics_0.1.3    ellipsis_0.3.2    cachem_1.0.3     
    #> [33] withr_2.5.0       klippy_0.0.0.9500 cli_3.5.0         magrittr_2.0.1   
    #> [37] crayon_1.4.0      readxl_1.3.1      mime_0.9          evaluate_0.19    
    #> [41] fs_1.5.2          fansi_0.4.2       xml2_1.3.2        blogdown_1.16    
    #> [45] tools_4.0.4       hms_1.0.0         lifecycle_1.0.3   munsell_0.5.0    
    #> [49] reprex_1.0.0      compiler_4.0.4    jquerylib_0.1.4   rlang_1.0.6      
    #> [53] grid_4.0.4        rstudioapi_0.13   rappdirs_0.3.3    rmarkdown_2.19   
    #> [57] checkdown_0.0.7   gtable_0.3.0      DBI_1.1.1         curl_4.3         
    #> [61] markdown_1.1      R6_2.5.0          lubridate_1.9.0   knitr_1.41       
    #> [65] fastmap_1.1.0     utf8_1.1.4        stringi_1.5.3     Rcpp_1.0.6       
    #> [69] vctrs_0.5.1       dbplyr_2.2.1      tidyselect_1.2.0  xfun_0.36

Otra forma de poner los detalles de la sesión es utilizar `sessioninfo::session_info()`; además lo usamos junto a `details::details()` que genera un desplegable para ver (o no) el outpt).

``` r
sessioninfo::session_info() %>% details::details(summary = 'current session info') 
```

<details closed>
<summary>
<span title="Click to Expand"> current session info </span>
</summary>

``` r

─ Session info ───────────────────────────────────────────────────────────────
 setting  value
 version  R version 4.0.4 (2021-02-15)
 os       Parrot OS 5.1 (Electro Ara)
 system   x86_64, linux-gnu
 ui       X11
 language (EN)
 collate  es_PE.UTF-8
 ctype    es_PE.UTF-8
 tz       America/Lima
 date     2023-01-07
 pandoc   2.19.2 @ /usr/lib/rstudio/resources/app/bin/quarto/bin/tools/ (via rmarkdown)

─ Packages ───────────────────────────────────────────────────────────────────
 package      * version    date (UTC) lib source
 assertthat     0.2.1      2019-03-21 [3] CRAN (R 4.0.0)
 backports      1.2.1      2020-12-09 [3] CRAN (R 4.0.3)
 blogdown       1.16       2022-12-13 [1] CRAN (R 4.0.4)
 bookdown       0.31       2022-12-13 [1] CRAN (R 4.0.4)
 broom          0.7.4      2021-01-29 [3] CRAN (R 4.0.3)
 bslib          0.4.2      2022-12-16 [1] CRAN (R 4.0.4)
 cachem         1.0.3      2021-02-04 [3] CRAN (R 4.0.3)
 cellranger     1.1.0      2016-07-27 [3] CRAN (R 4.0.0)
 checkdown      0.0.7      2020-11-01 [1] CRAN (R 4.0.4)
 cli            3.5.0      2022-12-20 [1] CRAN (R 4.0.4)
 clipr          0.7.1      2020-10-08 [3] CRAN (R 4.0.3)
 colorspace     2.0-0      2020-11-11 [3] CRAN (R 4.0.3)
 crayon         1.4.0      2021-01-30 [3] CRAN (R 4.0.3)
 curl           4.3        2019-12-02 [3] CRAN (R 4.0.0)
 DBI            1.1.1      2021-01-15 [3] CRAN (R 4.0.3)
 dbplyr         2.2.1      2022-06-27 [1] CRAN (R 4.0.4)
 demoR        * 0.0.0.9000 2023-01-07 [1] Github (kbodwin/demoR@a8dc5db)
 desc           1.4.2      2022-09-08 [1] CRAN (R 4.0.4)
 details        0.3.0      2022-03-27 [1] CRAN (R 4.0.4)
 digest         0.6.27     2020-10-24 [3] CRAN (R 4.0.3)
 dplyr        * 1.0.10     2022-09-01 [1] CRAN (R 4.0.4)
 ellipsis       0.3.2      2021-04-29 [1] CRAN (R 4.0.4)
 equatiomatic * 0.3.1      2022-01-30 [1] CRAN (R 4.0.4)
 evaluate       0.19       2022-12-13 [1] CRAN (R 4.0.4)
 fansi          0.4.2      2021-01-15 [3] CRAN (R 4.0.3)
 fastmap        1.1.0      2021-01-25 [3] CRAN (R 4.0.3)
 fontawesome    0.4.0      2022-10-25 [1] CRAN (R 4.0.4)
 forcats      * 0.5.1      2021-01-27 [3] CRAN (R 4.0.3)
 fs             1.5.2      2021-12-08 [1] CRAN (R 4.0.4)
 generics       0.1.3      2022-07-05 [1] CRAN (R 4.0.4)
 ggplot2      * 3.4.0      2022-11-04 [1] CRAN (R 4.0.4)
 glue           1.6.2      2022-02-24 [1] CRAN (R 4.0.4)
 gtable         0.3.0      2019-03-25 [3] CRAN (R 4.0.0)
 haven          2.3.1      2020-06-01 [3] CRAN (R 4.0.1)
 highr          0.8        2019-03-20 [3] CRAN (R 4.0.0)
 hms            1.0.0      2021-01-13 [3] CRAN (R 4.0.3)
 htmltools      0.5.4      2022-12-07 [1] CRAN (R 4.0.4)
 httpuv         1.5.5      2021-01-13 [3] CRAN (R 4.0.3)
 httr           1.4.2      2020-07-20 [3] CRAN (R 4.0.2)
 icons        * 0.2.0      2023-01-07 [1] Github (ropenscilabs/icon@6e4dc37)
 jquerylib      0.1.4      2021-04-26 [1] CRAN (R 4.0.4)
 jsonlite       1.7.2      2020-12-09 [3] CRAN (R 4.0.3)
 klippy         0.0.0.9500 2023-01-07 [1] Github (rlesur/klippy@378c247)
 knitr          1.41       2022-11-18 [1] CRAN (R 4.0.4)
 later          1.1.0.1    2020-06-05 [3] CRAN (R 4.0.1)
 lifecycle      1.0.3      2022-10-07 [1] CRAN (R 4.0.4)
 lubridate      1.9.0      2022-11-06 [1] CRAN (R 4.0.4)
 magrittr       2.0.1      2020-11-17 [3] CRAN (R 4.0.3)
 markdown       1.1        2019-08-07 [3] CRAN (R 4.0.0)
 mime           0.9        2020-02-04 [3] CRAN (R 4.0.0)
 modelr         0.1.8      2020-05-19 [3] CRAN (R 4.0.0)
 munsell        0.5.0      2018-06-12 [3] CRAN (R 4.0.0)
 pillar         1.8.1      2022-08-19 [1] CRAN (R 4.0.4)
 pkgconfig      2.0.3      2019-09-22 [3] CRAN (R 4.0.0)
 png            0.1-7      2013-12-03 [3] CRAN (R 4.0.2)
 promises       1.1.1      2020-06-09 [3] CRAN (R 4.0.2)
 purrr        * 0.3.4      2020-04-17 [3] CRAN (R 4.0.0)
 R6             2.5.0      2020-10-28 [3] CRAN (R 4.0.3)
 rappdirs       0.3.3      2021-01-31 [3] CRAN (R 4.0.3)
 Rcpp           1.0.6      2021-01-15 [3] CRAN (R 4.0.3)
 readr        * 1.4.0      2020-10-05 [3] CRAN (R 4.0.3)
 readxl         1.3.1      2019-03-13 [3] CRAN (R 4.0.0)
 reprex         1.0.0      2021-01-27 [3] CRAN (R 4.0.3)
 rlang          1.0.6      2022-09-24 [1] CRAN (R 4.0.4)
 rmarkdown      2.19       2022-12-15 [1] CRAN (R 4.0.4)
 rprojroot      2.0.2      2020-11-15 [3] CRAN (R 4.0.3)
 rstudioapi     0.13       2020-11-12 [3] CRAN (R 4.0.3)
 rvest          0.3.6      2020-07-25 [3] CRAN (R 4.0.2)
 sass           0.4.4      2022-11-24 [1] CRAN (R 4.0.4)
 scales         1.2.1      2022-08-20 [1] CRAN (R 4.0.4)
 sessioninfo    1.2.2      2021-12-06 [1] CRAN (R 4.0.4)
 shiny          1.5.0      2020-06-23 [3] CRAN (R 4.0.4)
 stringi        1.5.3      2020-09-09 [3] CRAN (R 4.0.2)
 stringr      * 1.4.0      2019-02-10 [3] CRAN (R 4.0.0)
 tibble       * 3.1.8      2022-07-22 [1] CRAN (R 4.0.4)
 tidyr        * 1.2.1      2022-09-08 [1] CRAN (R 4.0.4)
 tidyselect     1.2.0      2022-10-10 [1] CRAN (R 4.0.4)
 tidyverse    * 1.3.0      2019-11-21 [3] CRAN (R 4.0.0)
 timechange     0.1.1      2022-11-04 [1] CRAN (R 4.0.4)
 tweetrmd       0.0.9      2023-01-07 [1] Github (gadenbuie/tweetrmd@075102b)
 utf8           1.1.4      2018-05-24 [3] CRAN (R 4.0.2)
 vctrs          0.5.1      2022-11-16 [1] CRAN (R 4.0.4)
 vembedr      * 0.1.5      2021-12-11 [1] CRAN (R 4.0.4)
 withr          2.5.0      2022-03-03 [1] CRAN (R 4.0.4)
 xfun           0.36       2022-12-21 [1] CRAN (R 4.0.4)
 xml2           1.3.2      2020-04-23 [3] CRAN (R 4.0.0)
 xtable         1.8-4      2019-04-21 [3] CRAN (R 4.0.0)
 yaml           2.2.1      2020-02-01 [3] CRAN (R 4.0.0)

 [1] /home/achalmaedison/R/x86_64-pc-linux-gnu-library/4.0
 [2] /usr/local/lib/R/site-library
 [3] /usr/lib/R/site-library
 [4] /usr/lib/R/library

──────────────────────────────────────────────────────────────────────────────
```

</details>

<br>

Otro ejemplo de uso de `details::details()`:

``` r
#details::details(plot(sin, xlim = c(0, 20)), summary = "My curvy plot. Thanks McBain!!")
```

<br>

Si quieres ver todos los paquetes que tienes instalados en tu ordenador, lo puedes hacer así:

``` r
pkgs_instalados <- installed.packages(fields = c("Package", "Version")) %>% 
                        as.data.frame()
```

<br>

<br>

------------------------------------------------------------------------

------------------------------------------------------------------------

# Bibliografía

[Tutorial oficial de Rmarkdown](http://rmarkdown.rstudio.com/lesson-1.html) Muy bueno y muy completo. Quizás la primera opción para aprender.

[Tutorial completo](http://www.sfs.uni-tuebingen.de/~jvanrij/Tutorial/tutorialMarkdown.html). Tutorial sencillo pero bastante completo. Bastante didáctico.

[Pagina oficial de knitr](https://yihui.name/knitr/). Solamente para verla. Usarla sólo cuando ya “pilotes”.

[Cheat Sheet de Rmarkdon en castellano](https://www.rstudio.com/wp-content/uploads/2015/03/rmarkdown-spanish.pdf). Parece complicado, pero cuando te acostumbras es una fantástica chuleta.

[Tutorial de Rmarkdown en español](https://fernandosansegundo.wordpress.com/2016/05/05/programacion-literaria-en-r-con-knitr-y-markdown/)

[Tutorial de Markdown en español](http://joedicastro.com/pages/markdown.html)

[Customizing & Extending R Markdown](https://slides.yihui.name/2017-rstudio-conf-ext-rmd-Yihui-Xie.html#1). Tutorial del desarrollador de knitr. Corto pero avanzado.

[R Markdown: The Definitive Guide](https://bookdown.org/yihui/rmarkdown/). Pues eso, la guía definitiva. Fantástica!!

[R Markdown Cookbook](https://bookdown.org/yihui/rmarkdown-cookbook/). Nuevo libro, 2020, de Yihui Xie, Christophe Dervieux y Emily Riederer.

[Officeverse](https://ardata-fr.github.io/officeverse/index.html). Un bookdown para facilitar la generación de documentos word desde Rmarkdown.

[RMarkdown for Scientists](https://rmd4sci.njtierney.com/) de Nicholas Tierney.

[^1]: En realidad, under the hood estaremos usando la función `rmarkdown::render()`

[^2]: Si te interesa saber un poco más de este proceso puedes ir [aquí](https://stackoverflow.com/questions/40563479/relationship-between-r-markdown-knitr-pandoc-and-bookdown)

[^3]: Markdown es un lenguaje de marcado que permite la aplicación de formato a un texto empleando una serie de marcas o caracteres especiales

[^4]: esto es una nota al pie.
