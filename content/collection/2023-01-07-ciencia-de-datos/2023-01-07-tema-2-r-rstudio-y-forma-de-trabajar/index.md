---
title: Tema 2. R, RStudio y forma de trabajar
author: Edison Achalma Mendoza
date: '2023-01-07'
slug: tema-2-r-rstudio-y-forma-de-trabajar
categories: []
tags: []
---

<script src="{{< blogdown/postref >}}index_files/clipboard/clipboard.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/primer-tooltips/build.css" rel="stylesheet" />
<link href="{{< blogdown/postref >}}index_files/klippy/css/klippy.min.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/klippy/js/klippy.min.js"></script>
<script>
  addClassKlippyTo("pre.r, pre.markdown");
  addKlippy('right', 'top', 'auto', '1', 'Copy code', 'Copied!');
</script>

------------------------------------------------------------------------

<br>

El objetivo de esta sección es proporcionar una breve primera introducción a R y RStudio para personas que no han tenido contacto previo con estos programas y explicitar la forma que tendremos de interactuar con ellos; es decir, la forma de trabajar con ellos (**workflow**).

El curso es una introducción a la Ciencia de Datos: haremos diversos análisis con datos y para ello utilizaremos R. R será el programa que hará los cálculos, gráficos, informes, pero interactuaremos con R, le daremos las ordenes a R, a través de otro programa: RStudio. Así que tendremos que instalar los 2 programas. Por ello, en la [web del curso](https://perezp44.github.io/intro-ds-21-22-web/) tienes un fichero donde se explica como hacerlo: concretamente [aquí](https://perezp44.github.io/intro-ds-20-21-web/mas-recursos/Instrucciones_instalacion-a.html).

[Aquí](https://www.dataquest.io/blog/tutorial-getting-started-with-r-and-rstudio/) tienes un articulo que explica, con mucho detalle, como empezar a trabajar con R: instalación, configuración, paquetes, etc…

<br>

Se puede trabajar con R/RStudio de varias formas. Nosotros trabajaremos, casi siempre, con `Rprojects`. Enseguida diremos qué son los Rprojects, pero de momento podemos pensar que son carpetas donde se almacenan los ficheros necesarios para hacer un análisis de datos.

Dentro de esas carpetas o `Rprojects` tendremos distintos tipos de ficheros: ficheros de datos, imágenes etc… y unos ficheros, llamados habitualmente **scripts** que contendrán las instrucciones que queramos que sean ejecutadas por R/RStudio. Bien, pues esos scripts o ficheros de ordenes pueden ser de varios tipos. Concretamente, durante el curso utilizaremos 2 tipos de ficheros para darle las ordenes a R:

- `ficheros .R` , y

- `ficheros Rmarkdown` o `ficheros .Rmd`.

Lo normal es que nunca hayas oído hablar de todo esto, así que al principio te sonará complicado, pero en nada te parecerá lo más natural del mundo. Bird by bird!!!

## 1. R

Ya hemos hablado de R, pero …

### ¿Qué es R?

Ya lo habéis visto mientras hacíamos algún ejemplo, pero para los nuevos: R es un lenguaje de programación y un entorno para el análisis estadístico y gráfico. Se puede utilizar para muchas cosas ya que es un lenguaje de programación, pero principalmente se utiliza en el campo de la estadística y la ciencia de datos; de hecho, R fue inicialmente creado en 1993 por dos estadísticos de la Universidad de Auckland: R. Ihaka y R.Gentleman[^1]. A partir de 1997 el desarrollo de R (o **base-R**) es gestionado por un grupo de programadores conocido como “The R-core team”; pero actualmente, el entorno o ecosistema R es el resultado de la colaboración de toda una comunidad de usuarios que extiende las utilidades de base-R mediante la creación de nuevos paquetes y funciones.

R forma parte del sistema [GNU](https://es.wikipedia.org/wiki/GNU) y se distribuye bajo la licencia [GNU GPL](https://es.wikipedia.org/wiki/GNU_General_Public_License) por lo que los usuarios tenemos la libertad de usar, estudiar, compartir (copiar) y modificar el software; es decir, R es [**software libre**](https://www.gnu.org/philosophy/free-sw.es.html). Además de software libre, R es gratuito y multiplataforma: está disponible para Windows, Macintosh y GNU/Linux.

La página web oficial de R se llama: [The R Project for Statistical Computing](https://www.r-project.org/). Allí podrás encontrar toda la información y documentación oficial acerca de R. Aunque si alguna vez la necesitas, se puede consultar desde R con la función `help.start()` o, en un formato visualmente más agradable, en [este repositorio](https://colinfay.me/r-manuals/) de Collin Fay un destacado miembro de la actual comunidad R. Si quieres ver las personas que forman parte del R core-team o que han contribuido al desarrollo de R no tienes mas que teclear en R `contributors()`.

R proporciona un amplio abanico de herramientas estadísticas y gráficas (modelos lineales y no lineales, tests estadísticos, análisis de series temporales, algoritmos de clasificación y agrupamiento, etc.). Como R también es un lenguaje de programación, permite que los usuarios lo extiendan definiendo sus propias funciones y paquetes. De hecho, actualmente R se ha convertido de un proyecto colaborativo y abierto en el que sus usuarios pueden publicar paquetes que extienden su configuración básica. Para darte una idea de lo prolífica y colaborativa que es la comunidad R puedes visitar estos 2 proyectos: [R-bloggers](https://www.r-bloggers.com/) y [R-Weekly](https://rweekly.org/). Precisamente estos 2 aspectos (abundancia de paquetes y comunidad de usuarios) son claves en el éxito de R

Ya hemos dicho que R (junto con sus paquetes) puede implementar una gran variedad de técnicas estadísticas y gráficas. Existe un repositorio oficial de paquetes: Comprehensive R Archive Network o [CRAN](https://cran.r-project.org/). CRAN alcanzó los [10.000 paquetes](https://blog.revolutionanalytics.com/2017/01/cran-10000.html) en enero de 2017, y actualmente, julio de 2019, tiene 14.553 paquetes. Además, existen muchos más paquetes en repositorios como [Bioconductor](https://www.bioconductor.org/), [Github](https://github.com/) y otros.

<br>

### Instalación de R

Obviamente, para usar R y sus paquetes tenemos que instalarlo primero. Para ello “solo” tienes que ir a [CRAN](https://cran.r-project.org/) y descargar la distribución de R adecuada para tu sistema operativo. Obviamente mejor la última versión. En el momento de re-escribir estas notas la última versión es `R-4.1.1` llamada “Kick Things” released on 2021/08/10.

No te va a a hacer falta pero por si acaso, [aquí](https://jjallaire.shinyapps.io/learnr-tutorial-00-setup/#section-install-r) tienes un vídeo de 1:30 donde se explica de manera sencilla como instalar R, y [aquí](https://github.com/pachamaltese/tutoriales/blob/master/2019-04-24-instalar-r.md) tienes una explicación muy detallada del proceso de instalación.

Como recomiendan [aquí](https://teachdatascience.com/cloud/) el primer día de clase usaremos R a través de la plataforma [RStudio Cloud](https://rstudio.cloud/). Demoraremos los potenciales problemas que puedan surgir en la instalación de R al segundo o tercer día de clase[^2].

## 2. RStudio

### ¿Qué es RStudio?

Pues es un programa que utilizaremos para interactuar con R. Las instrucciones que queramos dar a R para que las ejecute se las daremos a través de RStudio. La razón es que la interfaz de usuario (GUI, Graphical User Interface) de R no es muy amigable ni versátil, así que interactuaremos con R a través de RStudio.

RStudio es un programa que nos permitirá interactuar con R de forma más amigable, además de facilitar muchas de las tareas de programación y análisis de datos en R; es decir, RStudio es una GUI (Graphical User Interface). En realidad, RStudio es más que una GUI, es una IDE, un entorno de desarrollo integrado para R, en inglés *‘integrated development environment’* o **IDE**.

El actual científico jefe de RStudio es [Hadley Wickham](http://hadley.nz/). Wickham es uno de los más prolíficos desarrollador de paquetes para R y creador de un nuevo estilo de programar y analizar datos en R conocido como *‘[tidyverse](https://blog.rstudio.org/2016/09/15/tidyverse-1-0-0/)’*. Muchos de los packages que utilizaremos en el curso han sido desarrollados por él y el equipo de RStudio.

<br>

### Instalación de RStudio

La versión de escritorio de RStudio también es libre y gratuita. Se puede descargar [aquí](https://www.rstudio.com/products/rstudio/download/). Tienes que descargarte el *‘installer’* adecuado para tu sistema operativo.

Se puede trabajar perfectamente con las opciones por defecto de RStudio, pero os recomiendo cambiar algunas opciones, así que vamos a configurar RStudio.

### Configurando RStudio

Está sección no es obligatoria, solo que es recomendable configurar las opciones de RStudio. ¿Cómo? En RStudio, sigue está ruta de menús: `Tools > Global OPtions...`

Se abrirá una ventana (que puedes ver abajo) con las opciones de configuración de RStudio. De momento vamos sólo a tocar la categoría que ves en la imagen; es decir, `R General`. Tienes que hacer dos cosas:

1.  desmarcar todas las casillas (quitarles los ticks)

2.  Es importante, poner `Never` en la casilla donde pone “Save workspace to .RData on exit”.

Al final, en mi ordenador, la ventana con las opciones de `R General` queda como:

En tu ordenador debe quedar todo igual excepto la caja de texto. El texto de la caja le dice a RStudio donde se guardarán los archivos que vayamos generando; es decir, indica el directorio de trabajo por defecto. Como mi sistema operaivo es Linux y habitualmente trabajo en el escritorio de mi PC, en la imagen de abajo pone “\~/Escritorio”, si mi sistema operativo fuese Windowns pondría algo como “C:/Users/perezp/Desktop”. Te recomiendo trabajar sobre el escritorio o Desktop, pero puedes seleccionar la carpeta en la que más cómoda trabajes[^3].

Ya explicaré en clase porqué seleccionamos estas opciones en RStudio.

#### Aún más configuración de RStudio

1.  En RStudio sigue está ruta de menús: `Tools > Global OPtions...` y selecciona `Code`. Intenta dejar la opciones de la pestaña `Editing` como ves en la imagen de abajo. Concretamente lo que más me interesa es que esté marcada la opción `Insert spaces for tab`

2.  En RStudio sigue está ruta de menús: `Tools > Global OPtions...` y selecciona `Code`. Ahora intenta dejar las opciones de la pestaña `Saving` como ves en la imagen de abajo. Lo más importante es que en la caja de texto `Default text encoding` ponga: `UTF-8`. Esto evitará que tengamos problemas con la codificación de loa caracteres, por ejemplo con la eñe o con las tildes.

Ya tenemos R y RStudio instalados y configurados, así que vamos a empezar a toquetear RStudio.

### Conociendo la interfaz de RStudio

Durante el curso vamos a utilizar R para hacer análisis estadísticos pero lo vamos a hacer a través de RStudio, así que el primer paso es familiarizarnos un poco con la interfaz de RStudio. Para acostumbrase a R y RStudio lo mejor es la práctica, pero si os hiciese falta, [aquí](https://ismayc.github.io/rbasics-book/index.html) tenéis un fantástico libro para habituarse a trabajar con R y RStudio.

Al abrir RStudio verás que al principio tiene 3 paneles, aunque enseguida abriremos un cuarto panel. La consola es el panel de la izquierda. Cuando tengamos 4 paneles la consola será el panel situado izquierda-abajo. Podemos pensar que la consola es lo más parecido a R, ya que en la consola se pueden ejecutar instrucciones de R directamente.

Cuando abras RStudio veras lo siguiente:

- Consola (izquierda)

- Environment/History (arriba-derecha)

- Files/Plots/Packages/Help (abajo-derecha)

Ya sabemos que el panel de la izquierda es la consola. En la consola se ve un mensaje de bienvenida que nos dice que versión de R estamos usando y alguna cosa más. Al final del texto aparece el símbolo `>`. A este símbolo se le conoce como *prompt* y simplemente nos indica que el intérprete de R, que R, está listo para ejecutar nuestras instrucciones.

¿Cómo le damos las instrucciones u ordenes a R? La forma más inmediata es escribiendo las ordenes en la consola, después del prompt (`>`). Por ejemplo, si escribimos en la consola `2+2` y presionamos <kbd>Enter</kbd>, R ejecutará la instrucción y nos devolverá el resultado.

A veces usaremos la consola para ejecutar alguna instrucción, pero en general ejecutaremos las instrucciones a través de un “script”. Una razón para no usar la consola es que trabajar en la consola es muy limitado ya que las instrucciones se han de introducir una a una. Otra razón es que queremos tener un registro con todas las instrucciones que ejecutemos para poder replicar nuestro análisis en otro momento; así que lo habitual es trabajar con **scripts** o **ficheros de instrucciones**.

Un script no es más que un fichero de texto con extensión `.R` en el que escribiremos las instrucciones que queramos que R ejecute.

Vamos a crear nuestro primer script. Para ello tienes que seguir esta ruta de menús en RStudio: `File > New File > R Script`. Visualmente:

Cuando pinches con el ratón en `R Script` se abrirá en RStudio un nuevo panel, el cuarto, arriba a la izquierda. Visualmente:

Este cuarto panel (arriba-izquierda) en realidad es un editor de texto. En él podemos
escribir las instrucciones que queramos que ejecute R. Por ejemplo, fíjate en la siguiente imagen lo que he escrito en el panel arriba-izquierda:

He escrito estas cuatro lineas:

``` r
# mi primer script de R
2 + 2
5 * 6
400/2
```

Escribe tú también (o copia y pega) estás cuatro lineas de texto en el editor (arriba-izquierda) de tu Rstudio.

R ejecutará, cuando se lo indiquemos, las lineas de instrucciones una a una.

Una vez hayas escrito o pegado esas 4 lineas en RStudio, verás que la primera linea es diferente: lo más evidente es que está en color verde, pero en realidad lo importante es que comienza con el símbolo `#`. Este hecho, está marcando/diciendo a R que esa linea es un comentario para los humanos, para nosotros, no es código R y por tanto R no la ejecutará.

En un script sólo se pueden escribir 2 cosas:

- comentarios (si la linea comienza con `#`). R no las ejecutará

- instrucciones R (no comienzan con `#`). R las ejecutará si están escritas en R; es decir, si siguen las reglas del lenguaje R. Si están mal escritas R nos devolverá un mensaje de error. Tenemos que aprender R ya!!!

Hemos escrito cuatro lineas en nuestro script y ahora queremos que R las ejecute. R ejecutará, cuando se lo indiquemos, las lineas de instrucciones una a una.

Para ejecutar una linea, situamos el cursor en ella y pulsamos <kbd>Crtl</kbd> + <kbd>Enter</kbd>.

Please, sitúa el cursor en la primera linea y pulsa <kbd>Crtl</kbd> + <kbd>Enter</kbd>. Observa qué ha ocurrido. Le hemos dicho a R que ejecute la primera linea, pero como esta primera linea comienza con `#`, R la ha interpretado (correctamente) como un comentario y, por supuesto, no la ha ejecutado, por lo que ha pasado a la segunda linea, y esta vez sí que la ejecuta. Como la segunda linea no comienza con `#`, R la interpreta como una instrucción de R y, sí la entiende (si las has escrito correctamente siguiendo la sintaxis o lenguaje de R), ejecutará la instrucción. R entiende que significa `2 + 2`, así que ejecuta la instrucción y nos devuelve el resultado en la consola.

<br>

En la imagen de abajo yo ya he ejecutado la instrucción `2 + 2`. R nos muestra el resultado en la consola: primero nos muestra, en azul, la instrucción que ha ejecutado; es decir `> 2 + 2` y luego nos nos muestra, en negro, el resultado de la ejecución de la instrucción; es decir `[1] 4`. Ya veremos que significa el \[1\] de la linea de resultados.

Es más fácil hacerlo que contarlo, aunque puede que te atasques en alguna cosa, normal!!. Por ejemplo, si en lugar de poner el cursor en la segunda linea, señalas o subrayas solo parte de la linea, entonces, seguramente R no te entenderá. Ahora te toca a ti: please, ejecuta la tercera linea de tu script.

¿Cómo le decimos a R que ejecute la tercera linea `5 * 6`? Cuando lo hacíamos en la consola simplemente había que pulsar <kbd>Enter</kbd>, pero ahora estamos trabajando en un script: hay que situar el cursor en la linea que queremos ejecutar y darle a <kbd>Crtl</kbd> + <kbd>Enter</kbd>. R ejecutará la instrucción y nos devolverá el resultado en la consola.

Enseguida aprenderemos más instrucciones o funciones de R, ahora solo estamos intentando familiarizándonos con el interfaz de RStudio. Ya sabemos como crear un fichero con instrucciones de R (ó script) y como ejecutar esas instrucciones.

Lo normal es que guardes tus scripts en un archivo por si tuvieses que volver a correr las mismas instrucciones más adelante. Para guardar tus instrucciones en un fichero sólo tienes que seguir esta ruta de menús en RStudio: `File > Save as ...`

Tendrás que elegir un nombre para tu script y decidir en que carpeta de tu ordenador guardarlo. Si decides que tu script se llame `my_script_01`, se creará un fichero (donde tú hayas decidido) llamado `my_script_01.R`. Fíjate que la extensión del archivo es **`.R`**, está extensión identifica los scripts o ficheros con instrucciones de R.

Esto vas a acabar entendiéndolo en poco tiempo, pero cuanto antes lo entiendas mejor: damos las ordenes/instrucciones a R por escrito, generalmente usamos “scripts”; es decir, escribimos las instrucciones en un fichero con extensión .R. Para ejecutar las ordenes que hemos escrito en nuestro fichero R hemos de, linea por linea, teclear: <kbd>Crtl</kbd> + <kbd>Enter</kbd>. Si la orden tiene sentido, es decir, si R entiende la orden, la ejecutará y te mostrará el resultado en la Consola.

<br>

Bien, ya sabemos hacer que R ejecute nuestras instrucciones: podemos ejecutar ordenes en la Consola (con <kbd>Enter</kbd>) o en un script (<kbd>Crtl</kbd> + <kbd>Enter</kbd>). Usaremos la consola a veces, muchas veces trabajaremos con scripts o ficheros .R pero, poco a poco, acabaremos trabajando de otra forma.

Como queremos que nuestros análisis sean reproducibles, habitualmente trabajaremos con `Rprojects` y con `ficheros .Rmd`. **Sí!!**, en lugar de con `ficheros .R` (o scripts) trabajaremos con `ficheros  **Rmarkdown**` ó `ficheros .Rmd`. Ya lo veremos, pero antes tendremos que familiarizarnos un poco más con el lenguaje R. De momento seguimos con el interfaz de RStudio.

<br>

#### Los 4 paneles de RStudio

Vamos a mirar con un poco más de detalle **los 4 paneles de RStudio**. Como puedes ver en la imagen de abajo, generalmente, a la izquierda encontramos la consola y el editor de scripts. Ya sabemos que desde estos dos paneles podemos dar instrucciones a R para que las ejecute.

Veamos un poco los 2 paneles de la derecha. Podemos pensar que son paneles auxiliares, nos ayudarán en determinadas tareas. Estos dos paneles de la derecha tienen cada uno varias pestañas. Por ejemplo, el panel que está en la posición arriba-derecha tiene cuatro pestañas: `Environment` y 3 más[^4]. En seguida veremos que al interactuar con R iremos creando objetos (por ejemplo un vector o una matriz o una tabla de datos). Estos objetos estarán guardados en la memoria del ordenador pero los “veremos”, aparecerán en la pestaña `Environment`. En la pestaña `History` tendremos un listado con las instrucciones de R que hayamos ejecutado previamente en nuestra actual sesión de R (por ejemplo `2 + 2`). Otro ejemplo: a veces en nuestro análisis con R haremos un gráfico o varios, podremos ver el gráfico en la pestaña `Plots` en el panel situado abajo-derecha.

La imagen de arriba es de hace unos años, si te fijas el panel superior-derecha tiene solo 2 pestañas. En 2020 salió la versión 1.3 de RStudio, en la que en el panel superior-derecha, en lugar de haber 2 pestañas, hay 4, una de ellas, llamada “Tutorials”, permite ejecutar tutoriales para aprender R dentro de RStudio.

<br>

## 3. Forma de trabajar con R y RStudio

Ya hemos dejado claro que vamos a usar RStudio para interactuar con R. Ok, pero hay distintas formas de trabajar, o distintos “workflows”.

Cuando hagas un análisis estadístico complejo, por ejemplo para tu TFG, o para el trabajo final de este curso, lo normal es que para realizar el proyecto no sea suficiente con un único script; lo habitual es que cada proyecto necesite de varios inputs (datos, imágenes, scripts etc…). En estos casos, utilizaremos un **Rproject** para cada proyecto.

En seguida veremos como podemos crear un Rproject, y explicaremos sus ventajas, pero de momento puedes pensar que un Rproject no es más que una carpeta dedicada en exclusiva a tu proyecto, una carpeta creada para almacenar todo lo relacionado con tu proyecto.

¿Por qué utilizaremos **Rprojects**? Las razones son varias, pero como casi siempre quien mejor lo explica es [Jenny Bryan](https://twitter.com/jennybryan?lang=es), por ejemplo [aquí](https://whattheyforgot.org/project-oriented-workflow.html).

Voy a intentar resumir yo lo que nos aconseja Jenny:

- es beneficioso poner todos los archivos (datos, scripts, imágenes, etc…) necesarios para un análisis en una única carpeta dedicada en exclusiva a ese análisis o proyecto.

- en la carpeta del proyecto es útil utilizar subcarpetas, por ejemplo una carpeta para datos, otra para imágenes, etc…

- los nombres de los archivos y las carpetas también son importantes. Hay que intentar que los nombres de los archivos sean explicativos de lo que hace o contiene el archivo. Los nombres de los ficheros han de ser legibles por las personas, pero también por las máquinas. Jenny lo explica [aquí](https://speakerdeck.com/jennybc/how-to-name-files). Por favor, no dejéis espacios en blanco en los nombres de los ficheros, si queréis separar palabras usad `-` y/o `_`. No uséis espacios en blanco!!!

- una de las características más interesantes de un Rproject es que el directorio de trabajo del proyecto es la propia carpeta del proyecto[^5]. Repito, en un Rproject, el directorio de trabajo es la propia carpeta del Rproject, y así podemos trabajar con **rutas** o paths **relativas**, lo que tiene la ventaja de que las rutas relativas funcionarán en cualquier ordenador[^6].

<br>

Trato de explicarlo un poco más: cuando trabajemos en un proyecto, generalmente, tendremos que cargar unos datos. Por ejemplo, imagina que los datos que vas a usar están en el fichero “mis_datos.xlsx”, así que tendrás que decirle a R donde están los datos. Tendrás que darle la ruta o path hasta el archivo de datos. Normal!!

Pero como vamos a trabajar con proyectos, los datos estarán dentro de la carpeta de mi proyecto, quizás en una subcarpeta llamada “datos”. Es posible que la ruta real o absoluta a mis datos sea la siguiente: `C:/Users/perezp/my_proyecto/datos/mis_datos.xlsx`, pero como trabajamos con proyectos, nuestro directorio de trabajo es la propia carpeta del proyecto, así que solo tendremos que usar una ruta relativa, solo tendremos que poner `./datos/mis_datos.xls`.

La ventaja de esto no es solamente que ahorramos tiempo escribiendo los nombres de las rutas, que también, la principal ventaja consiste en que, si por ejemplo, queremos compartir nuestro análisis con un colaborador, le daremos nuestra carpeta con todo el proyecto y los scripts **seguirán funcionando en SU ordenador** independientemente de donde ponga él la carpeta del proyecto que le hemos dejado.

La razón obviamente es que en nuestro proyecto hemos usado **rutas relativas**. Las rutas relativas, toman como referencia, empiezan desde el directorio de trabajo, y en un `Rproject` la carpeta de trabajo es siempre la propia carpeta del proyecto.

Para alguno de vosotros esto os parecerá complicado, pero ya veréis, en clase, que una vez lo entiendes, es muy-muy sencillo. Os habituareis enseguida a usar proyectos y rutas relativas.

Como dice Jenny:

> These habits guarantee that the project can be moved around on your computer or onto other computers and will still “just work”.

<br>

Para acabar esta sección, no puedo resistirme a citar otra vez a Jennyfer Bryan:

<blockquote class="twitter-tweet">
<p lang="en" dir="ltr">
File organization and naming are powerful weapons against chaos by <a href="https://twitter.com/JennyBryan?ref_src=twsrc%5Etfw">(**JennyBryan?**)</a> <a href="https://twitter.com/hashtag/Mozfest?src=hash&amp;ref_src=twsrc%5Etfw">\#Mozfest</a> <a href="https://twitter.com/hashtag/MozCookie?src=hash&amp;ref_src=twsrc%5Etfw">\#MozCookie</a> <a href="https://twitter.com/hashtag/FortuneCookie?src=hash&amp;ref_src=twsrc%5Etfw">\#FortuneCookie</a> <a href="https://t.co/W08ugLLrSa">pic.twitter.com/W08ugLLrSa</a>
</p>
— David Guarch 🖖 🎗️ ((**DGuarch?**)) <a href="https://twitter.com/DGuarch/status/663049353007931392?ref_src=twsrc%5Etfw">November 7, 2015</a>
</blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<br><br>

### Creando un Rproject

Bien, ya nos has dicho que trabajaremos con Rproject, vale, pero ¿cómo se crea un Rproject?

Simplemente has de abrir RStudio y seguir está ruta de menús: `File > New Project...` y se abrirá una ventana donde tendrás que seleccionar `New Project`. Entonces, se abrirá otra ventana y tendrás que seleccionar `New Directory`. Se abrirá otra ventana con dos cajas de texto, una, la de abajo, estará escrita la ruta donde se va a crear nuestra carpeta o proyecto y la caja de arriba estará vacía y has de poner allí el nombre que quieres que tenga tu proyecto. Como puedes ver en las imágenes de abajo, yo he llamado al proyecto “my_primer_project”.

Una vez hagas todo esto, RStudio creará una carpeta nueva en tu ordenador que será nuestra carpeta para el proyecto. En mi caso la carpeta estará en “C:/Users/perezp/Desktop/my_primer_proyecto”. Es una carpeta normal con un archivo dentro con un icono azulito y que tendrá por nombre “my_primer_proyecto.Rproj”; es un fichero de texto con extensión **.Rproj**. Ya hablaremos de él. Además de crear una carpeta en nuestro ordenador, RStudio habrá iniciado una nueva sesión de R con nuestro proyecto y verás algo como esto:

Sencillamente tenemos R y RStudio listos para trabajar; es decir, para ejecutar instrucciones en la consola o para crear nuestros scripts. Eso sí, los scripts que creemos ahora, se crearán directamente en la carpeta del proyecto. Ya parlarem mès de cómo interactuar con los Rprojects en clase.

Podemos pensar que un Rproject no es más que una carpeta en nuestro ordenador. De hecho puedes buscar la carpeta de tu proyecto en tu ordenador y manipularla como haces con cualquier carpeta de tu ordenador; es decir, puedes abrirla, moverla, cambiarle el nombre, crear subcarpetas, crear archivos, borrar archivos o borrar toda la carpeta. **Insisto**, para tu sistema operativo es una carpeta como cualquier otra. De momento esa carpeta solo contiene un archivo de texto con extensión **.Rproj**, poco a poco la iremos llenando con los archivos de nuestro proyecto (datos, scripts, etc …)

La carpeta del proyecto es una carpeta normal para tu sistema operativo, pero no es una carpeta normal para RStudio. Si vas a la carpeta de tu proyecto y pinchas en el archivo “my_primer_proyecto.Proj” se abrirá RStudio, y RStudio reconocerá esa carpeta como un proyecto; es decir, entre otras cosas fijará el directorio de trabajo a la propia carpeta del proyecto y podremos usar rutas relativas.

**Acuérdate siempre de lanzar un proyecto pinchando en el archivo con extensión “.Rproj” !!!!** Hay otras formas de lanzar el proyecto pero de momento usaremos esta.

### ¿Por qué usamos Rprojects?

Gestionar tus análisis utilizando Rprojects tiene ventajas:

1)  puedes gestionar varios proyectos a la vez, cada uno con su espacio de trabajo (ó environment), pero sobre todo,

2)  facilita el compartir tus análisis; es decir, favorece la investigación reproducible.

Podemos pensar que un Rproject es una carpeta, pero es más que eso: cada Rproject tiene su propio directorio de trabajo, espacio de trabajo (environment), historial de instrucciones; además, permite crear una estructura de carpetas donde guardar los documentos asociados al proyecto en carpetas separadas (p.ej: una carpeta para datos, otra para imágenes, …).

Cuando abres un Rproject en RStudio (pinchando en el fichero `.Rproj`) ocurre lo siguiente:

- Comienza un nuevo proceso de R (esto también es importante para la investigación reproducible)

- El directorio de trabajo se fija a la carpeta que contiene el Rproject, con lo que podemos usar rutas relativas (relativas a la carpeta del proyecto)

<br>

#### Cuidado con los paths!!

- Un gran inconveniente para conseguir informes (plenamente) reproducibles son los paths o rutas de ficheros. Si un programa necesita llamar a un fichero de datos (por ejemplo para cargar unos datos), tendrás que especificar la ruta y si alguien quiere ejecutar tus *scripts* en **su** ordenador deberá cambiar la ruta.

- Trabajar con Rprojects permite solventar este problema, ya que el directorio de trabajo del Rproject coincide con la carpeta donde está alojado el Rproject y esto permite (ya lo veremos en el próximo tutorial) trabajar con rutas (o paths) relativas en lugar de absolutas. (!!)

<br>

- En palabras de [Jenny Bryan](https://github.com/jennybc) una de mis he**R**oínas y destacada miembro de la comunidad R, si empiezas tus scripts con `setwd()`, significa que estás usando rutas absolutas, puedes hacerlo, pero Jenny nos aconseja que … **PLEASE STOP DOING THAT !!** Ademas Jenny nos lo explica:

  > This makes your script very fragile, hard-wired to exactly one time and place. As soon as you rename or move directories, it breaks. Or maybe you get a new computer? Or maybe someone else needs to run your code?

- Para Jenny la solución es usar el pkg `here`, y tiene razón, pero nosotros (de momento) sólo usaremos Rprojects (suficiente!!). `remo::ji("thinking")` . Bueno no, eso era en el curso para profesores, a vosotros sí que os veo capacitados para aprender como usar `here::here()`. `remo::ji("devil")` `remo::ji("lol")` . Lo veremos. El que tenga curiosidad puede leer en [este post](https://malco.io/2018/11/05/why-should-i-use-the-here-package-when-i-m-already-using-projects/) porqué, a pesar de trabajar con Rprojects, tiene ventajas especificar las rutas con el paquete `here`.

<br>

## 4. RMarkdown (archivos **.Rmd**)

Sí, ya sabemos que trabajaremos con Rprojects. OK, pero también dije que muchas veces en lugar de dar las instrucciones a R por medio de scripts o ficheros `.R`, trabajaríamos con ficheros `Rmarkdown`. Estos ficheros Rmarkdown tienen extensión `.Rmd`.

- Los documentos **RMarkdown** son ficheros con extensión **`.Rmd`**.

- Si acabas utilizando R para hacer análisis estadísticos, los ficheros `.Rmd` te permitirán escribir muy-muy fácilmente informes, tutoriales y transparencias para presentaciones.

- Estos ficheros .Rmd son (plenamente) reproducibles.

- Lo veremos, pero en esos ficheros .Rmd se mezclan trozos de texto escritos en Markdown (narratives) y trozos con código R (chunks) para hacer análisis estadísticos.

- Estos ficheros se procesan con un paquete de R llamado `knitr` desarrollado por [Yihui Xie](https://yihui.name/knitr/) … y salen unos informes o transparencias fantásticas … en una gran variedad de formatos.

- Con RStudio es muy fácil: solo hay que usar los menús desplegables de RStudio para crear un documento Rmarkdown, escribir lo que quieres contar y darle al botón Knitr y `knitr` tejerá el documento y lo transformará a …. pdf, word, html …

<br>

Tardaremos unas 3-4 clases en explicar en detalle qué son y para que sirven los ficheros Rmarkdown, pero vamos ya a crear uno. Para ello tienes que seguir en RStudio esta ruta de menús: `File > New File > R Markdown...`. Visualmente:

Se abrirá una ventana. De momento no cambies nada, sólo pincha en `OK`.

Verás que se ha abierto una pestaña en el editor de RStudio (arriba-izquierda), con lo que parece que son muchas lineas de código R. Sí, ha creado para nosotros un archivo `.Rmd` y ha puesto unas lineas de código que nos sirven como ejemplo de cómo se escribe en Rmarkdown. Ya lo veremos. Visualmente:

Estos ficheros `.Rmd` se ejecutan de otra forma. Tienes que pinchar en el icono que pone `Knit`. Visualmente:

Aparecerá una ventana pidiéndote que le pongas un nombre al fichero `.Rmd`. Como puedes ver abajo yo le puse el nombre “para_borrar”, pero puedes poner el nombre que quieras.

Una vez le hayas puesto nombre. R ejecutará todas las instrucciones que hay en el fichero .Rmd y generará un nuevo documento que podrás ver en el panel de abajo-derecha. Además si pinchas en el icono que aparece marcado con una mano( panel abajo-derecha) en la imagen de abajo podrás verlo en tu navegador. Visualmente:

Durante el curso vamos a trabajar mucho con ficheros .Rmd, así que tendremos que explicarlos/entenderlos bien. Pero será otro día/lesson. Si os apetece podéis ver [este video](https://www.youtube.com/watch?v=lNWVQ2oxNho) donde se explica las ventajas de trabajar en con ficheros Rmarkdow. Igual mañana lo pregunto.

<br><br>

Para finalizar un consejo: estamos empezando, así que PATIENCE!!! cuesta un poco aprender/empezar con R. Además todo el mundo comete errores, pero la mayoría de los errores son “tontos”. Eso sí, tenéis que entender las ideas básicas: script, .R, .Rmd, Rproject, rutas relativas etc… si no lo entiendes, no lo dejes pasar, pregúntalo en clase, seguro que más de uno te lo agradece o podemos arreglarlo en tutorías, pero no lo dejes pasar.

<blockquote class="twitter-tweet" align="center" data-width="550" data-lang="en" data-dnt="true" data-theme="light"><p lang="en" dir="ltr">Troubleshooting lessons I guess I&#39;ll just relearn forever: <br><br>- take a break<br>- it&#39;s almost certainly not a bug<br>- extra eyes are awesome<br>- spelling <a href="https://t.co/J17S8I6b3W">pic.twitter.com/J17S8I6b3W</a></p>&mdash; Allison Horst 🥑 (@allison_horst) <a href="https://twitter.com/allison_horst/status/1213275783675822080?ref_src=twsrc%5Etfw">January 4, 2020</a></blockquote>

[^1]: [Aquí](https://dl.acm.org/doi/abs/10.1145/3386334) tienes un artículo con la historia de R

[^2]: De esto esta vez no estoy seguro porque en Agosto de 2020 RStudio Cloud comenzará a ser de pago. Veremos como queda la versión gratuita

[^3]: Siempre que esa carpeta no esté muy abajo en la lista de directorios para que la ruta hacía ese directorio no sea demasiado larga para Windows

[^4]: Igual en vuestro ordenador tenéis más (o menos) pestañas, eso dependerá de la versión de RStudio que tengáis instalada. Yo ahora mismo tengo cuatro, pero igual la próxima versión de Rstudio puede tener 5 pestañas

[^5]: Sí, sé que si parece un trabalenguas, pero es muy importante que esto lo acabes entendiendo. Cuando lo entiendas, y seguro que lo haces pronto, verás que en realidad es muy fácil.

[^6]: Esto lo conseguiremos trabajando con Rprojects y con el paquete `here`. Lo veremos pronto
