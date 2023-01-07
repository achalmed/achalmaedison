---
title: 'Tema 3: Iniciación a R-base'
author: Edison Achalma Mendoza
date: '2023-01-07'
slug: tema-3-iniciaci-n-a-r-base
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

El objetivo de este tema es proporcionar una introducción a R para personas que no han tenido contacto previo con el programa. Se presentan algunos de los rudimentos del lenguaje de programación R. Conocer en detalle el lenguaje R es complicado, hay muchas cosas, pero conociendo unas cuantas de ellas puede ser suficiente para hacer análisis de datos complejos.

Se presentan conceptos básicos y, por tanto necesarios, como distintos tipos y estructuras de datos, asignación, funciones, operadores lógicos, subsetting etc… PERO, recuerda que en el curso vamos a enfatizar otra forma de trabajar con R. En el curso priorizamos trabajar con R usando principalmente los paquetes asociados al tidyverse; es decir, vamos a usar R à la tidyverse. Entonces, ¿por qué un tutorial sobre R-base? La razón es sencilla, los paquetes del tidyverse no son otro lenguaje, necesitan a R para funcionar, no tienen sentido fuera de él, así que cuanto mas sepas de R, de R-base, mejor. Al menos hay un mínimo de elementos de R-base que se necesita entender. En el tutorial intentaré centrarme en lo que es más necesario.

Este tutorial/tema no lo vamos a ver en clase en detalle. En clase empezaremos directamente a trabajar con ejemplos y casos con datos reales y con `data.frames`. ¿Entonces para qué este tema/tutorial? Pues para que sirva un poco de referencia, poco a poco iremos viendo trocitos de este tema; además tenéis en Internet excelentes recursos para aprender a programar con R.

En las respuestas a este tweet puedes ver distintas opiniones sobre si es mejor comenzar a aprender R con el tidyverse o con R-base:

<blockquote class="twitter-tweet" align="center" data-width="400" data-lang="en" data-dnt="true" data-theme="light"><p lang="en" dir="ltr">Roommates are doing their <a href="https://twitter.com/hashtag/rstats?src=hash&amp;ref_src=twsrc%5Etfw">#rstats</a> homework and their professor has forbidden the use of *any* packages because they &quot;have to learn the fundamentals.&quot; Is this a thing? I&#39;m frustrated on their behalf but open to opinions.</p>&mdash; Kaija Gahm (@kaija_bean) <a href="https://twitter.com/kaija_bean/status/1217293396706054145?ref_src=twsrc%5Etfw">January 15, 2020</a></blockquote>

Supongo que ya tenéis instalado R y RStudio en vuestro ordenador, así que intenta correr/ejecutar en tu ordenador las instrucciones de R que vayan apareciendo en el tutorial.

# 1. Ideas básicas

## Operaciones matemáticas básicas

R puede utilizarse como calculadora.

``` r
# operaciones básicas con R
2 + 2    
2 - 2    
2 * 2    
2 / 2 

# Potenciación (se puede hacer con el operador ^ o con **)
3^2    
3**2

# división entera y módulo
11 %/% 5    # división entera 
11 %% 5     # módulo (resto de la división entera)
```

<br>

#### ¿Hay que poner espacios entre los elementos de una expresión?

Como ves, no importa si pones o no espacios entre los elementos de una expresión. De todas formas casi siempre es mejor separar los diferentes elementos de una linea de código: usar espacios hace el código más legible. Para convencerte de que uses espacios: ¿que crees que se se lee mejor, esto, *oquizascreesqueseleemejorestootro*?

<br>

#### Orden de precedencia de las operaciones

Lógicamente se pueden combinar varias operaciones. Ten cuidado siempre con el orden de precedencia que da R a las operaciones. El orden es el siguiente: paréntesis, exponentes, multiplicación, división, suma y resta. **Ante la duda usa los paréntesis**.

``` r
6 + 2 * 5   
#> [1] 16
(6 + 2) * 5
#> [1] 40
```

<br>

#### expresiones de varias lineas

De momento es mejor no hacerlo, pero puedes repartir tus expresiones en varias lineas:

``` r
2  + 2 + 2 + 2 + 2 +
10 + 
30
#> [1] 50
```

Más adelante, por ejemplo cuando hagamos gráficos, sí que lo haremos para ganar en claridad en el código. LLegará.

<br>

## Asignación (“creación de objetos”)

En la sección anterior hicimos que R hiciera unos cálculos. Muy bien, pero lo normal en un análisis con datos es que, para alcanzar un resultado final, tengamos que hacer cálculos intermedios e ir combinándolos para llegar al resultado final. Los cálculos que hemos hecho con R en la sección anterior se han perdido; dicho de otra manera, ahora mismo no podemos recuperarlos.

Para poder recuperar o reusar algún calculo intermedio hecho con R, tenemos que “asignar” un nombre a nuestros cálculos. Repito, para poder recuperar/reusar un valor, este ha de tener asociado/asignado un nombre.

Dicho de otra manera, para poder reusar un resultado o valor intermedio, tenemos que crear un objeto que contendrá el valor que hemos calculado, pero para ello tenemos que poner o asignar un nombre a ese objeto[^1].

En R, para **asignar un nombre a un valor**, y así crear un objeto, se usa el operador **`<-`**[^2]. Veámoslo:

``` r
aa <- 2 + 2
```

Fíjate que parece que R no ha hecho nada ya que no nos muestra el resultado de la operación en la consola. Ahora lo que ha hecho es realizar la operación obteniéndose un resultado o valor de `4` (dos mas dos son 4), pero en lugar de mostrarnos/devolvernos el valor, lo que ha hecho es “almacenar” el valor 4 en el objeto `aa`.

En vuestra cabeza una expresión de asignación, por ejemplo `aa <- 44`, debe sonar como `aa toma el valor 44`.

Podemos ver el objeto `aa`en el panel superior-derecha de RStudio, concretamente en la pestaña “Environment”. Ahora el entorno de R, R, tiene un objeto almacenado en su memoria, un objeto que se llama “aa” y cuyo valor es 4.

Veámoslo: si ahora ejecutamos `aa`, R nos devolverá el valor 4. Podemos pensar que `aa` es un objeto, donde se almacena el valor 4.

``` r
aa
#> [1] 4
```

Ahora podemos usar el objeto `aa` para continuar o hacer más cálculos. Por ejemplo:

``` r
aa + 1
#> [1] 5
```

El nombre `aa` está asociado al valor `4`, así que cuando usemos `aa` en una nueva instrucción, R
usará el valor 4. Evidentemente podemos cambiar el valor del objeto `aa`. Por ejemplo:

``` r
aa <- 10
```

Ahora, si llamamos a `aa` nos devuelve el valor 10.

``` r
aa
#> [1] 10
```

¿Qué hacen las siguientes lineas de código? Puedes pensarlo, pero lo mejor es que ejecutes el código en tu ordenador.

``` r
aa <- 2 + 2
bb <- 5 + aa
cc <- 1 + aa * 2
dd <- bb
```

Fijaros que ahora en el entorno o *environment* de R tendremos 4 objetos: aa, bb, cc, dd.

<br>

#### Global environment (primera referencia al)

Cada vez que asignas un nombre a un valor, R crea un nuevo objeto en el `Global environment`. Estos objetos existirán hasta que cierres tu sesión en R, después desaparecerán, a no ser que guardes los objetos en disco en un fichero. Podemos ver los objetos que hay en el Global environment pinchando en la pestaña “Environment” del panel superior-izquierdo de RStudio. También podemos hacerlo con la función `ls()`. Ejecuta las siguientes instrucciones y observa que ocurre en el Global environment.

``` r
ls()              #- muestra los objetos en el Global env. Hace lo mismo que objects()
#> [1] "aa" "bb" "cc" "dd"

rm(cc)            #- borra/elimina el objeto cc del Global env.
rm(list = ls())   #- borra todos los objetos del Global env.
```

<br>

Recuerda que en R, la forma genérica de una operación de asignación, o de “creación de objetos”, es: `nombre_del_objeto <- valor`, por ejemplo `aa <- 2 + 2`, y que para poder recuperar/reusar un valor ha de tener asociado/asignado un nombre.

<br>

#### ¿Puedo usar el nombre que quiera para mis objetos?

No del todo. Para que un nombre sea sintácticamente válido en R sólo puede contener caracteres alfanuméricos (letras y números), puntos (**`.`**) y guiones bajos (**`_`**).

Además:

- un nombre NO puede empezar por un número

- un nombre NO puede empezar por **`_`**

- si el nombre empieza por `.` , el punto NO puede ir seguido de un número

``` r
# nombres válidos
pepe <- 4 
pepe_2 <- 4
pepe_2.3 <- 22
.hola <- 7

# nombres no válidos
4pepe <- 33
_hola <- 66
.2xx  <- 88
```

Lo normal es usar nombres simples y, si puede ser, explicativos de la naturaleza del valor almacenado en el objeto.

R distingue entre mayúsculas y minúsculas así que puede existir un objeto con nombre `Ariadna` y otro con nombre `ariadna`.

Como en todos los lenguajes de programación, R tiene una serie de nombres reservados, ya asignados, y que por tanto no se pueden usar para nombrar a los objetos que nosotros creemos. Lógicamente están prohibidos porque R los usa internamente. Estos nombres prohibidos son:

``` r
if  else repeat  while  for in next break
function
TRUE FALSE 
NULL Inf NaN 
NA NA_integer_ NA_real_ NA_complex_ NA_character_
```

<br>

## Tipos de datos

Ya sabemos que R nos va a ayudar a manejar/analizar datos. Bien, pero ¿qué tipos de datos entiende R?

Los principales tipos son 3: numéricos, de texto y lógicos; en realidad 4 porque R diferencia los datos númericos en doubles e integers[^3]
Cada dato o valor es de un tipo. El tipo de un valor determina la forma de almacenamiento y las operaciones que se pueden hacer con él.

R puede manejar, tiene, 5 tipos de datos:

- Caracteres (texto): Pepe, hola, Madrid

- Doubles: 2,35 , 77,00 , -5,6

- Enteros: 1, -44

- Lógicos: TRUE, FALSE (En operaciones aritméticas toman valores 1 y 0)

- Complejos: 3+2i

Ademas de estos 5, existe un sexto tipo: `raw`, que no vamos a utilizar.

Por ejemplo:

``` r
aa <- "La calle en la que vivo es"    #- texto
bb <- 4L                              #- número entero
cc <- 4.3                             #- número decimal
dd <- TRUE                            #- logical
```

Normalmente sabremos de que tipo(texto, entero, …) es cada objeto, pero conviene saber con certeza de que tipo es cada objeto. Por ejemplo, los objetos creados en el chunk anterior, ¿de que tipo son? Nos lo imaginamos, pero para confirmarlo podemos usar la función `typeof()`

``` r
typeof(aa)
#> [1] "character"
typeof(bb)
#> [1] "integer"
typeof(cc)
#> [1] "double"
typeof(dd)
#> [1] "logical"
```

<br>

En realidad los 3 tipos fundamentales de datos/valores que usaremos son:

- “numeric”: Numéricos (números enteros y reales)

- “character”: Texto (secuencias o cadenas de caracteres)

- “logical”: Lógicos o booleanos (TRUE o FALSE, que en operaciones aritméticas toman valores 1 y 0)

Además, hay 4 valores especiales: `NULL`, `NA`, `NaN`, e infinito

Los `NA`’s serán más adelante importantes y en cierta forma hay que tener cuidado con ellos, siempre habrá que chequear si nuestros datos contienen `NA`’s. NA representa una característica que existe pero de la cual no sabemos su valor, pero ese valor existe. Por ejemplo, imagina que el siguiente vector representa la altura en centímetros de un grupo de personas : `c(182, 187, 159, NA, 166)`. El vector tiene 5 elementos, pero el cuarto elemento es un NA, lo que indica que no sabemos la altura del cuarto individuo. Imagina que queremos calcular la altura media, utilizaremos la función `mean()`. Fíjate que ocurre:

``` r
aa <- c(182, 178, 172, NA, 168)
mean(aa)
#> [1] NA
mean(aa, na.rm = TRUE)
#> [1] 175
```

Como ves, cuando se hace un calculo estadístico con un objeto que contiene NA’s, el resultado es NA; es decir, los NA’s se propagan[^4]. Si quieres que esto no ocurra cuando haces cálculos estadísticos, has utilizar dentro de las funciones la opción `na.rm = TRUE` que lo que hace es excluir los NA’s antes de hacer los cálculos.

<br>

## Operaciones con números

Con datos o **variables numéricas** ya hemos visto que se pueden hacer operaciones aritméticas (suma, resta etc…), pero con números se pueden hacer también **comparaciones**.

Por ejemplo:

``` r
2 < 4    # MENOR que: esta expresión chequea si 2 es MENOR que cuatro. Como es cierto, nos devuelve un TRUE
#> [1] TRUE
2 > 4    # MAYOR que: esta expresión chequea si 2 es MAYOR que cuatro. Como es cierto, nos devuelve un TRUE
#> [1] FALSE
5 >= 7   # MAYOR o IGUAL que.
#> [1] FALSE
8 <= 8   # MENOR o IGUAL que.
#> [1] TRUE
9 == 7   # IGUAL a: como 9 no es igual a 7, nos devolverá un FALSE
#> [1] FALSE
2 == 2   # IGUAL a: como 2 es igual a 2, nos devuelve TRUE
#> [1] TRUE
2 != 4   # NO IGUAL: como 2 no es igual a 4 nos devuelve TRUE
#> [1] TRUE
5 != 5   # NO IGUAL: como 5 es igual a 5, nos devuelve FALSE 
#> [1] FALSE
```

Fíjate que estas expresiones de comparación al ser ejecutadas devuelven un “boolean”: el resultado de la comparación solo puede ser TRUE o FALSE si la afirmación es cierta o, por el contrario no es cierta. Por ejemplo si ejecutas `5 < 2` el resultado sera `FALSE` porque 5 no es menor que 2.

Que ¿para qué necesitamos estos operadores? Para muchas cosas, por ejemplo para ver que valores de una variable están por encima de la media.

Fíjate que el operador para chequear la igualdad de dos valores no es `=`, que es lo que habitualmente usamos en matemáticas para expresar igualdad. En R la igualdad se expresa/chequea con el doble igual: `==`.

Recuerda que el signo `=` se puede usar para hacer una asignación, aunque en R es más habitual usar el `=` dentro de las funciones para asignar un valor al argumento de una función, y se suele usar `<-` como símbolo de asignación.

<br>

## Operaciones con texto

Hay muchas, pero por ejemplo, no podemos sumar 2 strings o 2 cadenas de texto, pero si que se pueden pegar o concatenar. Por ejemplo con la función `paste()`.

``` r
aa <- "mi nombre es"
bb <- "pedro"
paste(aa, bb)
#> [1] "mi nombre es pedro"
paste(aa, bb, sep = " ... ")
#> [1] "mi nombre es ... pedro"
# Prueba tú mismo que hace la función paste0()
```

Veamos algunas otras “operaciones” que se pueden hacer con variables de texto:

``` r
toupper(aa)
#> [1] "MI NOMBRE ES"
tolower(aa)
#> [1] "mi nombre es"
stringr::str_to_sentence(aa)   #- stringr es un pkg del tidyverse
#> [1] "Mi nombre es"

nchar(bb)                      #- nchar() nos devuelve el número de caracteres de un string
#> [1] 5
substring(bb, 2, nchar(bb))    #- substring() extrae caracteres de un string
#> [1] "edro"
```

Si al final necesitamos manipular texto, tendremos que aprender un poco de `regular expressions` y, si puede ser, utilizaremos el paquete [`stringr`](https://stringr.tidyverse.org/articles/regular-expressions.html)

<br>

## Operaciones lógicas

A veces tendremos que hacer operaciones lógicas, por ejemplo, tendremos que seleccionar a los individuos que tengan más renta que la media y que además estén solteros. En R tenemos los siguientes operadores lógicos:

- `&`: es el operador lógico **AND**. Devuelve TRUE si se cumplen todas las condiciones.

- `|`: es el operador lógico **OR**. Solo devuelve FALSE si NO se cumple ninguna de las condiciones.

- `!`: es el operador lógico **NOT**. Cambia el sentido de una afirmación lógica. No confundir con el operador relacional o de comparación `!=`

- `xor()`: es el operador lógico **Exclusive OR**. Devuelve TRUE si se cumple una y solo una de las 2 condiciones.

Hay alguno mas (`all()`, `any()`, `&&` y `||`) pero suficiente con estos tres primeros.

``` r
(4 > 3) & (3 > 2)     #- Y: como se cumplen las dos condiciones nos devuelve TRUE
#> [1] TRUE
(1 == 2) | (2 >3)       #- O: Como no se cumple ninguna de las 2 condiciones nos devuelve FALSE
#> [1] FALSE
!(4 > 3)              #- NOT: 4 es mayor que 3 es TRUE, pero el ! delante de esa condición la niega y pasa a FALSE
#> [1] FALSE
!!(4 > 3)             #- si niegas dos veces, vuelves al principio: TRUE
#> [1] TRUE

xor(10 < 1, 10 >1 ) #- se cumple 1 de las dos condiciones, entonces TRUE
#> [1] TRUE
xor(10 > 1, 10 >1 ) #- se cumplen las 2 condiciones, entonces FALSE
#> [1] FALSE
xor(10 < 1, 10 <1 ) #- no se cumple ninguna de las 2 condiciones: FALSE
#> [1] FALSE
```

## Funciones

Entender qué es una función y cómo “funciona una función” es muuuuy importante!!!

R y sus paquetes tienen muchísimas funciones que nos permiten, por ejemplo, calcular logaritmos, o raíces cuadradas, o calcular desviaciones típicas etc etc… Además, también podemos crear nuestras propias funciones. Seguramente crearemos algunas en el curso, pero antes, es MUY IMPORTANTE entender qué es y cómo “funciona”, cómo se usa, una función de R.

Repito, es muy importante entender qué es y cómo usar una función. De hecho, todo lo que ocurre/pasa en R es porque has llamado a una función. Si algo ocurre en R es porque has hecho una llamada a una función, una “function call”.

Una función no es más un trozo de código R, unas instrucciones de R, a las que les hemos puesto un nombre; entonces, cuando invoquemos ese nombre, esa función, se ejecutarán esas lineas de código.

Empecemos a usar alguna función sencilla (el objetivo es entender como “funciona” una función):

Una función muy sencilla es `sqrt()`. Como igual imagináis, la función `sqrt()` sirve para calcular la raíz cuadrada de un número. Alguien, ha escrito por nosotros unas lineas de código que sirven para hacer raíces cuadradas y ha asignado esas lineas de código al nombre `sqrt`. sqrt es el nombre de la función `sqrt()`

Como alguien se ha preocupado de construir una función para hacer raíces cuadradas, nosotros podemos usar esa función. Si por ejemplo queremos calcular la raíz cuadrada de 9, sólo tendremos que teclear en R `sqrt(9)`.

``` r
sqrt(9)
#> [1] 3
```

Perfecto, está bien que sepamos como hacer raíces cuadradas en R, PERO **lo importante es empezar a entender la estructura de las funciones**.

La forma genérica de utilizar una función es algo como: `nombre_de_la_funcion(argumento_1, argumento_2, ....)`. En el caso de la función `sqrt()` su nombre es `sqrt` y esta función solo admite un argumento. Un vector de números[^5].

`sqrt()` solo admite un argumento, pero otras funciones pueden tener más de un argumento y quizás los argumentos no sean numéricos sino por ejemplo textuales. Buff!! es fácil, pero explicarlo por escrito, sin ver al que va a recibir la explicación, es complicado.

``` r
sqrt(9)
sqrt(9, 4)   # no funciona porque sqrt() solo admite un argumento 
sqrt("9")    # no funciona, solo hemos puesto un argumento pero es textual, y ha de ser numérico
```

Es decir, para usar una función tenemos que saber cuantos argumentos admite y de que tipo han de ser esos argumentos. Generalmente esto es obvio, pero habrá veces que tengamos que usar una función que no sepamos como funciona, entonces tendrás que buscar su ayuda.

Para obtener ayuda sobre una función podemos usar la función `help()`. Si tecleas en R `help(nombre_de_la_funcion)` se abrirá una ventana de ayuda en la pestaña “Help” del panel abajo-derecha. Probémoslo con la función `sqrt()`

``` r
help(sqrt) 
```

Al leer la ayuda de la función te darás cuenta que hace un rato hicimos un poco de trampas, ya que explicamos el funcionamiento de las funciones de una forma un poco simplificada. Vamos a hacerlo ahora mejor.

Yo dije que la estructura de una función es `nombre_de_la_funcion(argumento_1, argumento_2, ....)` cuando en realidad es : **`nombre_de_la_funcion(argumento_1 = valor_1, argumento_2 = valor_2, ....)`**.

Vamos a explicarlo con la función `sqrt()`. El nombre de la función `sqrt()` es `sqrt`; y ¿cuales son sus argumentos? Si miramos más detenidamente la ayuda, veremos que sí, que sólo tiene un argumento `x` , que además debe ser numérico.

Bien, pero ¿cual es el valor del argumento? Intenta descubrirlo con el chunk de código siguiente:

``` r
sqrt(x = 9)
sqrt(x = 4)
```

La sintaxis correcta de `sqrt()` es efectivamente `nombre_de_la_funcion(argumento_1 = valor_1, argumento_2 = valor_2, ....)`, en su caso, como solo tiene un argumento: `sqrt(argumento = valor)`.

El nombre del argumento es `x`, y el valor del argumento es el que nosotros queramos, siempre que sea numérico. La sintaxis correcta-correcta es `sqrt(x = 9)`. 9 es el valor que le damos al argumento `x` de la función `sqrt()`.

Obviamente podemos cambiar el valor de la función, sino la función no nos sería muy útil. Entonces, ¿por qué funcionan las 2 lineas de código siguientes?

``` r
sqrt(9)
#> [1] 3
sqrt(4)
#> [1] 2
```

Pues porque a R no le importa que no pongas el nombre del argumento, puedes poner solamente su valor. Hablaremos de esto un poco más en clase.

A ver si consigues diferenciar, en una función, entre el nombre de un argumento y su valor

``` r
x <- 25
sqrt(9)
#> [1] 3
sqrt(x)
#> [1] 5
sqrt(x = x)
#> [1] 5
```

Sí, cuesta un poco, poquet a poquet, [“bird by bird”](https://www.bookdepository.com/Bird-By-Bird-Anne-Lamott/9780385480017).

<br>

Otra vez más. Por favor, calculad con R el logaritmo de 1000 en base 10. Para ello tenéis que usar la función `log()`, y cómo no sabéis cómo se usa, no sabéis cómo es su sintaxis, no sabéis cuales son sus argumentos, os tocará mirar la ayuda de la función.

``` r
help(log)
log(x = 1000, base = 10)
```

Al principio mirar la ayuda interna de R para las funciones abruma, pero muchas veces con mirar los ejemplos (que están siempre al final) o la sección de “Arguments” es suficiente. En el caso de `log()` vemos que admite dos argumentos, “x” y “base”. La ayuda nos dice que la sintaxis de la función es:

- log(x, base = exp(1))

- “x” ha de ser numérico (o complejo)

- “base” ha de ser un número positivo (o complejo)

Fíjate que la sintaxis de la función no es `log(x, base)`, sino `log(x, base = exp(1))`; esto indica que el argumento “base” tiene un valor asignado por defecto; es decir, si no especificamos el valor de “base”, “base” será exp(1); es decir, el numero e y estaremos tomando logaritmos naturales.

``` r
log(1000)  #- como no especificamos el valor del argumento "base", R lo fija por defecto base = exp(1) y toma logaritmos naturales
#> [1] 6.907755

log(1000, base = 10) #- ahora si estamos calculando logaritmo en base 10
#> [1] 3
```

<br>

Es más seguro poner los nombres de los argumentos, pero si no los pones, o solo los pones parcialmente, también funciona

``` r
log(1000, bas = 10)   #- funciona, pero ...
#> [1] 3
log(1000, 10)         #- esto sí es muy habitual verlo
#> [1] 3
```

Eso sí, si no pones el nombre de los argumentos, has de tener en cuenta el orden de estos.

``` r
log(10, 1000)
#> [1] 0.3333333
```

Poco a poco iremos hablando más de funciones. Cuando usemos una nueva generalmente tendremos que consultar la **ayuda** para ver su sintaxis y sus argumentos.

Saber buscar ayuda es una de las habilidades más importantes a la hora de aprender a programar. [Este post](https://sctyner.github.io/rhelp.html) da buenos consejos sobre cómo buscar ayuda sobre R. En el siguiente apartado desarrollaré un poco la idea de cómo usar la ayuda interna de R sobre sus funciones.

<br>

### Ayuda de las funciones

Hay varias formas de pedir a R la ayuda interna de una función:

1)  usando la función `help()`, o sea, tecleando en R `help(nombre_de_la_funcion)`; por ejemplo `help(log)`

2)  tecleando en R `?nombre_de_la_funcion`; por ejemplo `?(log)`

3)  la forma más cómoda, y la que suelo usar, consiste en situar el cursor en el nombre de la función y pulsar la tecla <kbd>F1</kbd>

Entender y saber leer la ayuda de las funciones es muy útil, así que os recomiendo, para más adelante (de momento tenemos otras cosas que aprender), la lectura de [este post](http://socviz.co/appendix.html#a-little-more-about-r). Explican bien como está estructurada la ayuda de las funciones. Abajo tienes un ejemplo con la función `mean()`.

<br>

Como ejemplo puedes probar a leer la ayuda de la función `seq()`. Mirando la ayuda intenta adivinar que harán las siguientes expresiones R. Tienes que entender porque la cuarta y quinta linea no devuelven el mismo resultado.

``` r
seq(from = 0, to = 10)
#>  [1]  0  1  2  3  4  5  6  7  8  9 10
seq(0, 10)
#>  [1]  0  1  2  3  4  5  6  7  8  9 10
seq(10, 0)
#>  [1] 10  9  8  7  6  5  4  3  2  1  0
seq(0, 10, 3)
#> [1] 0 3 6 9
seq(0, 10, length.out = 3)
#> [1]  0  5 10
```

<br>

No solo tenemos la ayuda oficial, en R también hay funciones que nos pueden ayudar a entender como funciona otra función; por ejemplo la función `args()`, que como su nombre insinúa, nos permite ver los argumentos de una función. Por ejemplo:

``` r
args(sqrt)       #- sqrt() solo tiene un argumento, x
args(log)        #- log() tiene 2 argumentos: x y base. Además base tiene un valor por defecto: exp(1)
args(args)       #- args() solo tiene un argumento, llamado name.
```

<br>

### Ciclo vital de las funciones

Otra idea que conviene conocer, es que las funciones tienen un ciclo vital o “life cycle”: hay funciones que acaban de ser creadas y aún son experimentales. Hay funciones que pueden estar siendo cuestionadas y otras que pasan de experimentales a estables. [Este post](https://www.tidyverse.org/lifecycle/) muestra los diferentes estados de una función. El estado actual de una función se suele conocer por su distintivo o “**badge**”. Por ejemplo, en el siguiente tweet se explica la diferencia entre una función cuyo badge es `deprecated` de otra función cuyo badge es `superseded`:

<blockquote class="twitter-tweet">
<p lang="en" dir="ltr">
Why <a href="https://twitter.com/hadleywickham?ref_src=twsrc%5Etfw">(**hadleywickham?**)</a> and team switched from calling functions “retired” to “superseded” - “When people heard a function was retired they thought we were going to take it out back and shoot it in the head.” <a href="https://twitter.com/hashtag/rstudioconf?src=hash&amp;ref_src=twsrc%5Etfw">\#rstudioconf</a> <a href="https://t.co/462hbOSkRv">pic.twitter.com/462hbOSkRv</a>
</p>
— Emily Robinson ((**robinson_es?**)) <a href="https://twitter.com/robinson_es/status/1222972469650153472?ref_src=twsrc%5Etfw">January 30, 2020</a>
</blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<br>

Ya vale de funciones, pero hay algo que a algunos os rondará por la cabeza.

Cuando hemos visto la ayuda de la función `sqrt()`, sólo tenía un argumento `x`, y este argumento tenía que ser, según la ayuda, un vector (o array[^6]) de números.

**PERO** nosotros no introdujimos un vector en `sqrt()`, sino que introdujimos un sólo número. Sí, es cierto, introdujimos un sólo número, pero R no entiende lo que es un escalar, para él un número aislado es un vector, para R el número 4 es un vector con un sólo elemento, el número 4.

Fíjate que el valor que introduzcamos en `sqrt()` tiene que cumplir dos requisitos, ser un vector y que sus valores sean numéricos. Estas dos ideas hay que tenerlas claras para trabajar con R:

- Tipos de datos: `sqrt()` sólo admite datos numéricos, pero ¿qué otros tipos de datos podemos utilizar en R? Lo hemos visto en una sección anterior (texto, lógicos,…) . Por ejemplo, si ejecutamos `sqrt("99")`, R nos devolverá un error, porque `"99"` no es numérico es texto.

- Estructuras de datos: El vector es una de las estructuras de datos que “entiende R”, una de las estructuras en las que puede almacenar datos y luego volver a encontrarlos, pero hay más (matrices, listas, data frames)

En la próxima sección se presentan las diferentes estructuras de datos que tiene R para almacenar datos, pero en el curso vamos a centrarnos principalmente en una estructura de datos, los datos tabulares, que en R se almacenan en una estructura llamada `data frame`.

En clase ya hemos trabajado con data.frames, es la estructura de datos a la que estamos más acostumbrados, una tabla de datos con filas y columnas. Son las típicas tablas de Excel, con las variables en columnas y las observaciones en filas. Es muy fácil e intuitivo porque estamos acostumbrados a ellas, es lo que estamos acostumbrados a trabajar en ciencias sociales.

Igual de intuitivo resulta el hecho de que hay variables numéricas, como por ejemplo el número de páginas de un libro, y variables cuyos valores son texto; por ejemplo el título o el autor del libro.

<br>

## Estructuras de datos en R

R es un lenguaje/programa/entorno para hacer estadística por lo que generalmente trabajaremos con datos. Pero los datos tienen que estar almacenados en objetos. Igual que en matemáticas podemos almacenar datos en determinadas estructuras como vectores o matrices, en R ocurre lo mismo, los datos se almacenan en objetos. PERO hay distintos tipos de objetos o estructuras de datos[^7].

Para almacenar conjuntos de valores o datos, R tiene definidas determinadas estructuras de datos. ¿Cuántas? ¿Cuáles? ¿Cómo se llaman?

Pues hay varias formas de contarlo, para Hadley Wickham sólo hay una estructura de datos, los vectores. Sólo que estos vectores pueden tener diversas propiedades. Hay vectores atómicos y vectores recursivos. Seguro que tiene razón, pero aunque sea un poco menos preciso, es mucho más útil explicarlo, al menos al principio, de otra forma.

Podemos pensar que las principales estructuras de datos en R son:

- vectores

- matrices

- arrays (matrices multidimensionales)

- listas

- data.frames

Las que más utilizaremos en el curso son los data.frames, y en segundo lugar las listas. Sí, pero en realidad estas 2 estructuras (data.frames y listas) son en realidad agrupaciones de vectores; es decir, la estructura básica, la más importante en R son los vectores. Son los más importantes porque el resto de estructuras se construyen a partir de grupos de vectores o añadiendo alguna propiedad adicional, o atributo, a un vector.

<br>

# 2. Vectores

La **estructura de datos fundamental en R es el vector**[^8]. En R, un vector es una estructura de datos que sirve para almacenar un conjunto ordenado de valores o elementos. Un vector puede contener cualquier número de elementos; sin embargo, **todos los elementos deben ser del mismo tipo**. Por ejemplo, un vector no puede contener números y texto.

Esta estructura para almacenar datos en R es muy fácil de entender porque son los típicos vectores que conocemos de matemáticas.

Vamos a crear nuestro primer vector en R; para ello usamos la función `c()`:

``` r
aa <- c(3, 22, 6)
aa
#> [1]  3 22  6
```

Como vemos con la función `c()` hemos concatenado 3 números para construir un vector, el vector aa.

``` r
is.vector(aa)
#> [1] TRUE
```

Una de las características que tiene esta estructura de datos es que los elementos de un vector tienen que ser todos del mismo tipo. En nuestro caso el vector `aa` tiene 3 elementos, todos ellos de tipo numérico, concretamente doubles. Veámoslo con `typeof()`

``` r
typeof(aa)
#> [1] "double"
```

Creemos ahora un vector con datos textuales o caracteres:

``` r
aa <- c("Hola", "número", "9")
is.vector(aa)
#> [1] TRUE
typeof(aa)
#> [1] "character"
```

Ahora un vector de booleanos:

``` r
aa <- c(FALSE, TRUE, FALSE)
is.vector(aa)
#> [1] TRUE
typeof(aa)
#> [1] "logical"
```

Como R tiene 4 tipos de datos fundamentales (integer, double, character y lógico)[^9] se pueden crear con ellos 4 tipos de vectores; a estos tipos fundamentales de vectores se les suele llamar como “atomic vectors”.

<br>

## Atomic vectors vs. Augmented vectors

Este tópico no es fácil de entender, seguramente, igual empezáis a entenderlo a mitad de curso, pero si que conviene tener al menos una ligera idea sobre ello, por eso lo introduzco mínimamente.

Como R tiene 4 tipos fundamentales de datos, con ellos podemos construir 4 tipos de vectores fundamentales o “atomic vectors”. El tipo de datos, or modes, define cómo se van a almacenar internamente los valores. El tipo de los vectores podemos obtenerlo con la función `typeof()`.

Para ver de que tipo (fundamental) es un vector, disponemos de la función `typeof()`

``` r
typeof(4)
#> [1] "double"
typeof(4L)
#> [1] "integer"
typeof("4")
#> [1] "character"
typeof(TRUE)
#> [1] "logical"
```

**PERO** resulta que sobre la base de estos 4 tipos de vectores fundamentales se han construido otros tipos de vectores, que como son derivados de los fundamentales, se les suele llamar (derived or) **augmented vectors**[^10].

Voy a explicarlo un poco, pero antes hay que saber que los objetos, por ejemplo los vectores, en R pueden tener “atributos”. Podemos pensar que los atributos son una forma de poder almacenar información adicional (metadatos) en un objeto de R. OK, estos atributos son los que permiten crean nuevos tipos de vectores (augmented vectors).

Los augmented vectors o vectores derivados también se almacenarán internamente como numéricos o character o logical, **PERO** al contener información adicional, o atributos, hace que este tipo especial de vectores puedan ser identificados y tratados de forma especial por ciertas funciones de R. Es decir, los augmented vectors son como los atomic vectors (vectores fundamentales), se construyen a partir de ellos, PERO tienen información adicional (metadatos) almacenadas en sus atributos.

Se puede pensar que los atributos son una “named list of vectors” que se adjunta a un objeto. Puedes ver los atributos de un objeto con la función `attributes()`.

Entre los atributos que podemos definir, hay uno especial llamado class, que permite definir la `object’s class` y que es el atributo que va a hacer que algunos vectores se comporten de manera distinta ante algunas funciones; por ejemplo que se impriman o grafiquen de forma un poco especial. Podemos ver la clase (class) de un objeto con la función `class()`.

Entre los vectores aumentados, Hay 4 tipos importantes que conviene conocer: los factores, los factores ordenados, las fechas (date) y las date-time (o posixct).

<div class="figure" style="text-align: center">

<img src="https://d33wubrfki0l68.cloudfront.net/baa19d0ebf9b97949a7ad259b29a1c4ae031c8e2/8e9b8/diagrams/vectors/summary-tree-s3-1.png" alt="Creado por Ildiko Czeller y Graham Parsons" width="90%" />
<p class="caption">
Figure 1: Creado por Ildiko Czeller y Graham Parsons
</p>

</div>

Para tener un ejemplo que ayude a entender lo anterior uasaré el vector `iris$Species`. El vector `iris$Species` es en realidad un vector de integers pero, como ademas de los valores de los enteros, tiene metadatos almacenados en sus atributos, su class es factor. Sí, complicado entenderlo a la primera, PERO lo que si que se os tiene que quedar es que a veces usaremos factores. Lo importante será saber usar los factores correctamente y no tanto saber qué es un factor[^11]. Lo veremos!!

``` r
typeof(iris$Species)
#> [1] "integer"
attributes(iris$Species)
#> $levels
#> [1] "setosa"     "versicolor" "virginica" 
#> 
#> $class
#> [1] "factor"
class(iris$Species)
#> [1] "factor"
```

## Coerción

Ya dijimos que, en R, los elementos de un vector tienen que ser todos del mismo tipo; por eso decimos que los vectores son una estructura de datos homogénea.

Bien, pero ¿qué ocurre si en un vector hay elementos de distinto tipo?

por cómo están definidos internamente los vectores, sólo pueden contener elementos del mismo tipo, pero si por error introducimos valores de distinto tipo, R convertirá todos sus valores a un único tipo. Forzará a que sus elementos sean del mismo tipo. Esta forma de proceder en R, consistente en transformar todos los elementos de un vector a un mismo tipo se llama **coerción**.

¿A que tipo los convierte? Pues al menos flexible. Veámoslo con varios ejemplos:

``` r
aa <- c(4, 6,  "Hola")
```

En la expresión de arriba hemos puesto en el vector `aa` tres elementos, 2 números y un string. No puede ser, estamos violando las reglas internas de R para los vectores: los vectores sólo pueden tener elementos del mismo tipo.

Entonces, ¿por qué R no nos devuelve un mensaje de error? Porque lo que hace es convertir los valores de `aa` a un único tipo, ¿a cual? veámoslo con `typeof()`.

``` r
aa <- c(4, 6, "Hola")
is.vector(aa)
#> [1] TRUE
typeof(aa)
#> [1] "character"
aa               #- ¿qué ha pasado?
#> [1] "4"    "6"    "Hola"
```

Fíjate en los resultados. ha convertido los 2 números a caracteres. El primer elemento de `aa` no es el número cuatro sino el string 4. ¿Veis que está entre comillas? Lo ha convertido en el carácter `"4"`.

<br>

``` r
aa <- c(TRUE, 4L, 4, "Hola")
typeof(aa)
#> [1] "character"
aa <- c(TRUE, 4L, 4)
typeof(aa)
#> [1] "double"
aa <- c(TRUE, 4L)
typeof(aa)
#> [1] "integer"
```

Fíjate que con el chunk de arriba puedes inferir las reglas de conversión que usa R. `character > double > integer > logical`. Si en el vector hay un valor de texto, todos los valores se convertirán al tipo character.

Los valores de tipo carácter son los menos flexibles, piensa que no hay ninguna forma de convertir “Hola” en un número o en boolean. Al contrario sí se puede: el número 9 siempre se puede convertir al carácter “9”. Los booleans (TRUE y FALSE) se pueden transformar tanto en texto como en numérico: TRUE pasará a ser 1 y FALSE = 0.

<br>

### Coerción explícita

A veces tendremos un vector de un tipo, por ejemplo numérico, pero nos gustaría convertirlo a por ejemplo character. ¿Podemos hacerlo? Sí.

``` r
aa <- c(1:4)
aa
#> [1] 1 2 3 4
aa <- as.character(aa)
aa
#> [1] "1" "2" "3" "4"
```

Hay toda una familia de unciones para hacer estas conversiones, si es que son posibles, ya que, por ejemplo, no podremos pasar un vector de strings a numérico.

``` r
as.character()           
as.logical()    
as.numeric()   
y algunas más como as.data.frame() ....
```

<br>

## Propiedades de los vectores

Todo vector tiene dos propiedades claves:

- su tipo, que podemos ver con `typeof()`

- su longitud, orden o número de elementos, que podemos ver con `length()`

``` r
aa <- c(1:10)
typeof(aa)
#> [1] "integer"
length(aa)
#> [1] 10
attributes(aa)
#> NULL
```

Ademas, los vectores pueden tener más propiedades o [atributos](http://adv-r.had.co.nz/Data-structures.html#attributes). Estas propiedades son adicionales, no son necesarias y generalmente se usan para construir tipos especiales de vectores. Se definen los atributos con la función `attr()` y con `attributes()` se pueden ver los atributos que tiene un determinado vector.

``` r
aa <- c(1:3)
attributes(aa)
#> NULL
attr(aa, "atributo_1") <- "This is a vector"
attributes(aa)
#> $atributo_1
#> [1] "This is a vector"
attr(aa, "atributo_2") <- c("primero", "segundo", "tercero")
aa
#> [1] 1 2 3
#> attr(,"atributo_1")
#> [1] "This is a vector"
#> attr(,"atributo_2")
#> [1] "primero" "segundo" "tercero"
```

Un atributo que a veces se usa es poner nombres a los elementos de un vector, se puede hacer directamente al crear el vector o después con `setNames()` o con `set_names()`

``` r
aa <- c(a = 1, b = 2, c = 4)
```

``` r
aa <- c(1,2,4)
aa <- setNames(aa, letters[1:3])       
aa                                      
#> a b c 
#> 1 2 4
```

``` r
aa <- c(1,2,4)
aa <- rlang::set_names(aa, c("a", "b", "c"))
aa                                      
#> a b c 
#> 1 2 4
```

<br>

## Subsetting con vectores

En R podemos agrupar valores en vectores. Perfecto, pero habrá veces que necesitemos manipular los vectores. Por ejemplo necesitaremos acceder a determinados elementos de un vector, quizás a los elementos que sean mayores que 5, o a los que empiecen con la letra A, etc etc… Este tipo de operaciones sobre los vectores se les conoce genéricamente como **subsetting**; porque lo que se hace es crear subconjuntos de un vector. Veámoslo.

Hay varios tipos de subsetting, pero con vectores los principales son 3:

1)  **Positive Index**: podemos seleccionar por posición. Por ejemplo a los 2 primeros elementos o los 2 primeros y los 2 últimos. Veámoslo:

``` r
aa <- c(10:1)
aa[c(1:2)]        #- primer y segundo elemento del vector
#> [1] 10  9
aa[c(1,2,9,10)]   #- dos primeros y 2 últimos
#> [1] 10  9  2  1
aa[c(1,1,10,10)]  #- si repites el indice se repite el elemento del vector
#> [1] 10 10  1  1
```

2)  **Negative index**: eliminamos elementos del vector.

Por ejemplo eliminamos los 2 primeros elementos del vector y los 2 últimos:

``` r
aa <- c(10:1)
aa[- c(1,2, 9:10)]
#> [1] 8 7 6 5 4 3
```

3)  **Logical index**: se seleccionan aquellas posiciones marcadas con TRUE.

Esta forma de hacer subsetting será muy útil. De momento no lo apreciaremos, pero enseguida veremos su utilidad cuando hagamos subsetting lógico con funciones de comparación. Como ejemplo:

``` r
aa <- 1:10
aa <- aa[aa >= 7]
aa
#> [1]  7  8  9 10
```

Si no acabas de entenderlo, corre las siguientes lineas de código:

``` r
aa <- 1:10
aa <= 4
aa[aa <= 4]
aa <- aa[aa <= 4]
```

## Modificando elementos de un vector

``` r
aa <- c(1:10)
aa[4] <- 88             #- el cuarto elemento de aa tomará el valor 88
aa <- c(aa, 111, 112)   #- añadimos 2 elementos al vector aa
```

Los vectores se pueden concatenar

``` r
aa <- c(1:5)
bb <- c(100:105)
cc <- c(aa, bb)
```

## Creación de vectores mediante …

- secuencias  
- repeticiones  
- números aleatorios

### Secuencias

Ya sabemos que podemos generar secuencias de números con el operador `:`. Por ejemplo:

``` r
1:10
#>  [1]  1  2  3  4  5  6  7  8  9 10
```

Pero la función `seq()` nos ofrecen más posibilidades:

``` r
seq(1, 10, 2.5)
#> [1] 1.0 3.5 6.0 8.5
seq(from = 1, to = 10, by = 2.5)
#> [1] 1.0 3.5 6.0 8.5
```

### Repeticiones

la función `rep()` permite generar vectores repitiendo los elementos de un vector o lista

``` r
aa <- 1:3
rep(aa, 2)
#> [1] 1 2 3 1 2 3
rep(aa, each = 2)     
#> [1] 1 1 2 2 3 3
rep(aa, c(2,2,4))
#> [1] 1 1 2 2 3 3 3 3
rep(aa, each = 2, len = 10)   
#>  [1] 1 1 2 2 3 3 1 1 2 2
rep(aa, each = 2, times = 3)  
#>  [1] 1 1 2 2 3 3 1 1 2 2 3 3 1 1 2 2 3 3
```

### generando números aleatorios

<br>

## Operaciones con vectores

Todos sabemos que los vectores se pueden sumar, multiplicar, trasponer, … En realidad en el curso no vamos a utilizar álgebra matricial o vectorial, pero si que vamos a manipular, a hacer operaciones con vectores, aunque generalmente lo haremos usando funciones.

No obstante, conviene saber algunas cosas sobre operaciones con vectores en R. Por ejemplo podemos sumar vectores:

``` r
aa <- 1:10
bb <- 1:10
aa + bb
#>  [1]  2  4  6  8 10 12 14 16 18 20
```

### Recycling

Si intentamos hacer una operación con dos vectores pero estos no tienen el mismo orden, entonces R, automáticamente reciclará el vector más corto hasta que alcance la longitud del más grande y así poder hacer la operación. Este comportamiento se conoce como recycling. Por ejemplo:

Un ejemplo:

``` r
aa <- 1:10
aa + 1
#>  [1]  2  3  4  5  6  7  8  9 10 11
```

Como es que hemos podido sumar `aa+1`, si son vectores de distinto orden. Pues porque R siempre intentará hacer la operación y si no se puede, lo que hace es **reciclar**, aumentar el vector más pequeño, ¿Cómo? Repitiendo los elementos del vector más pequeño hasta que alcance la longitud del vector más grande.

Otro ejemplo de reciclado:

``` r
aa <- 1:6
bb <- 1:2
aa + bb
#> [1] 2 4 4 6 6 8
```

### funciones vectorizadas

La mayoría de funciones, y todos los operadores de R están vectorizados; es decir, si una función recibe como input un vector, se aplicará la función a cada uno de los elementos del vector.

Por ejemplo, la función `sqrt()` tiene un sólo argumento, admite como valor de su único argumento un vector de números[^12]. Se aplicará la función a cada uno de los elementos del vector:

``` r
aa <- c(4, 9, 25)
sqrt(aa)
#> [1] 2 3 5
```

La vectorización de las funciones hace que R sea un lenguaje en la que no es muy frecuente el uso de for loops o bucles, ya que en realidad la vectorización implica que se está ejecutando un bucle interno, pues se aplica la función a cada uno de los elementos del vector.

No siempre, pero en general, en R se sustituyen los bucles `for` tanto por la vectorización como por el uso de una familia de funciones `*apply` o más recientemente con las funciones del paquete `purrr`.

## Operaciones de comparación

Los operadores de comparación también están vectorizados. Si comparamos 2 vectores, las comparaciones se efectúan elemento a elemento

``` r
aa <- 1:3
bb <- 3:1

aa == bb
#> [1] FALSE  TRUE FALSE
aa >= bb
#> [1] FALSE  TRUE  TRUE
aa != bb
#> [1]  TRUE FALSE  TRUE
```

En las operaciones de comparación también aplica el recycling:

``` r
aa <- 1:3
bb <- 2

aa == bb
#> [1] FALSE  TRUE FALSE
aa >= bb
#> [1] FALSE  TRUE  TRUE
aa != bb
#> [1]  TRUE FALSE  TRUE
```

## Operaciones de conjuntos

``` r
aa <- 1:4
bb <- c(1:2, 99)

union(aa, bb)            
#> [1]  1  2  3  4 99
intersect(aa, bb)
#> [1] 1 2

setdiff(aa, bb)       #- Elementos de aa que no están en bb
#> [1] 3 4
setequal(aa,bb)       #- chequea si dos vectores son iguales
#> [1] FALSE
setequal(1:4, 1:4)    #- chequea si dos vectores son iguales
#> [1] TRUE
```

## Funciones útiles con vectores

Hay muchísimas funciones que se pueden utilizar con vectores, pero algunas que merece la pena conocer son[^13] :

<br>

- `length()`: nos da el orden o número de elementos de un vector. Ya la vimos.

``` r
aa <- 1:4
length(aa)
#> [1] 4
```

<br>

- `sum()`: devuelve la suma de los valores de un vector.

``` r
aa <- 1:4
sum(aa)
#> [1] 10
```

¿Qué pasaría si el vector fue de tipo texto o character?

<br>

- `cumsum()`: devuelve un vector del mismo orden con la suma acumulada (hasta ese valor).

``` r
aa <- 1:4
cumsum(aa)
#> [1]  1  3  6 10
```

<br>

- `mean()`: devuelve el valor de la media de los valores del vector.

``` r
aa <- 1:4
mean(aa)
#> [1] 2.5
```

<br>

- `order()`: devuelve un vector con la posición que ocuparían los valores originales de un vector si se ordenasen de menor a mayor

``` r
aa <- c(2.1, 4.2, 3.3, 5.4)
order(aa)
#> [1] 1 3 2 4
```

<br>

- `sort()`: devuelve un vector con los valores del vector original ordenados de menor a mayor

``` r
aa <- c(2.1, 4.2, 3.3, 5.4)
sort(aa)
#> [1] 2.1 3.3 4.2 5.4
```

<br>

- El siguiente chunk utiliza `order()` y subsetting para lograr el mismo resultado que con `sort()`

``` r
x <- c(2.1, 4.2, 3.3, 5.4)
x[order(x)]
#> [1] 2.1 3.3 4.2 5.4
```

<br>

# 3. Matrices

Otra estructura para almacenar valores en R son las matrices. No las usaremos mucho, en realidad nada, pero conviene conocerlas un poco. R si que usa las matrices internamente por ejemplo para hacer análisis de regresión.

Al igual que los vectores, una matriz **sólo puede contener elementos del mismo tipo**, por eso decimos que es una estructura de datos de tipo homogénea.

``` r
(aa <- matrix(1:6, ncol = 2, nrow = 3)) #- creamos una matriz 3x2
#>      [,1] [,2]
#> [1,]    1    4
#> [2,]    2    5
#> [3,]    3    6
```

Las matrices también se pueden crear **concatenando vectores**:

``` r
aa <- c(1:3)
bb <- c(11:13)
cc <- cbind(aa, bb)  #- agrupamos los vectores por columnas con cbind()
dd <- rbind(aa, bb)  #- agrupamos los vectores por filas con rbinb()
```

## Subsetting con matrices

Es muy parecido al subsetting en vectores, el operador que usaremos es el mismo, `[ ]`, pero claro las matrices tienen dos dimensiones, usaremos `[ , ]`. Veámoslo:

``` r
aa <- matrix(1:9, nrow = 3, ncol = 3) #- creamos una matriz 3x3

bb <- aa[2, 3]          #- seleccionamos el elemento (2,3) de la matriz

bb <- aa[ , 2]          #- seleccionamos la segunda columna (devuelve un vector)
bb <- aa[ , c(2,3)]     #- seleccionamos la segunda y tercera columna
bb <- aa[c(2,3), ]      #- seleccionamos la segunda y tercera FILAS

bb <- aa[-2, ]          #- eliminamos la segunda fila
bb <- aa[-2, -c(1,2)]   #- eliminamos la segunda fila y la primera y segunda Columnas
```

## Nombrar las filas y columnas

Al igual que los vectores, las matrices admiten atributos, entre ellos dar nombre a las filas y columnas

``` r
aa <- matrix(1:6, nrow = 2, ncol = 3) #- creamos una matriz 2x3
aa
#>      [,1] [,2] [,3]
#> [1,]    1    3    5
#> [2,]    2    4    6

colnames(aa) <- c("col_1", "col_2", "col_3")    
rownames(aa) <- paste("fila", 1:2, sep = "_")    
aa
#>        col_1 col_2 col_3
#> fila_1     1     3     5
#> fila_2     2     4     6
```

## Funciones para matrices

Hay muchas, por ejemplo:

``` r
aa <- matrix(1:6, nrow = 3, ncol = 2)  #- matriz 3x2
dim(aa)  #- devuelve un vector con las dimensiones de la matriz
t(aa)    #- transpone la matriz
```

Por supuesto se pueden multiplicar matrices, calcular inversas etc etc…

<br>

# 4. Arrays

Otra estructura para almacenar valores en R son los arrays. Son matrices multidimensionales. No las usaremos mucho, en realidad nada. También es una estructura de datos homogénea; es decir, sus elementos tienen que ser todos del mismo tipo

``` r
(aa <- array(1:12, c(2, 3, 2)) )
#> , , 1
#> 
#>      [,1] [,2] [,3]
#> [1,]    1    3    5
#> [2,]    2    4    6
#> 
#> , , 2
#> 
#>      [,1] [,2] [,3]
#> [1,]    7    9   11
#> [2,]    8   10   12
```

<br>

Podéis imaginar que si tuviésemos que hacer subsetting de un array, tendríamos que utilizar `[ , , ]`. Por ejemplo

``` r
aa[1, 2 , 1]
#> [1] 3
```

<br>

# 5. Factores

Podemos pensar que los factores son otro tipo de estructura para almacenar datos, aunque en realidad son vectores, pero vectores de un tipo especial. Veamos qué es un factor, para qué se utilizan, cómo puedo crearlos, etc…

Pues ya he dicho que los factores en realidad **SON VECTORES**, pero tienen un atributo que les hace comportarse de manera un poco especial.

Los creadores de R, crearon este tipo especial de vector llamado **factor** para almacenar información sobre **variables categóricas**; por ejemplo el color de ojos, o los días de la semana, los meses del año, el género etc…

En principio los factores sirven para representar variables categóricas: las categorías o valores que puede tomar la variable deberían ser fijas y conocidas. Por ejemplo, los días de la semana, que es una variable categórica con 7 categorías o grupos.

Mi opinión personal, puede que un poco extrema, es que los factores suelen dar problemas al manipular los datos, mejor evitarlos. Son útiles, sin embargo, al hacer gráficos (permiten ordenar las categorías para mostrarlas de la forma más conveniente) y cuando se trabaja con modelos estadísticos, ya que los factores se usan para representar variables categóricas, y las variables categóricas se incorporan, generalmente, en los modelos estadísticos mediante variables dummy. Si tienes tus variables categóricas almacenadas en factores las funciones relacionadas con los modelos, por ejemplo `lm()` tratarán la información de forma adecuada y generarán las dummies de forma automática en el modelo. Es muy fácil cometer errores al recodificar variables cuando codificas las variables categóricas como numéricas, así que mejor tenerlas como factores y que lo haga R por nosotros. Por ejemplo:

<blockquote class="twitter-tweet" align="center" data-width="400" data-lang="en" data-dnt="true" data-theme="light"><p lang="en" dir="ltr">Data scientists take note. Big JAMA paper retracted because treatment variable coded [1,2] recoded in error to [1,0]. Results of analysis reversed. Lung disease self-management program actually harmed patients. Check recoding carefully! via @themalariaarea<a href="https://t.co/uF4bRLbqy8">https://t.co/uF4bRLbqy8</a></p>&mdash; Prof Ewen Harrison (@ewenharrison) <a href="https://twitter.com/ewenharrison/status/1183424510151872512?ref_src=twsrc%5Etfw">October 13, 2019</a></blockquote>

<br><br>

En mi opinión, otra vez un poco extrema, el tidyverse comenzó como una lucha contra `string.as.factor = TRUE`[^14]. Afortunadamente, la próxima versión de R, la versión 4.0, tendrá la opción `string.as.factor` fijada a FALSE por defecto. El anuncio oficial se hizo en el post al que apunta este tweet:

<blockquote class="twitter-tweet" align="center" data-width="400" data-lang="en" data-dnt="true" data-theme="light"><p lang="da" dir="ltr">New R blog entry by Kurt Hornik: stringsAsFactors<a href="https://t.co/0h0rLvUWIQ">https://t.co/0h0rLvUWIQ</a></p>&mdash; The R Foundation (@_R_Foundation) <a href="https://twitter.com/_R_Foundation/status/1229386343995838465?ref_src=twsrc%5Etfw">February 17, 2020</a></blockquote>

<br>

Ya dije que los factores se usan para representar variables categóricas y que pueden ser útiles cuando trabajas con gráficos, tablas y/o modelos estadísticos pero también son un poco raros/especiales[^15].

Si tienes que usar factores, es mejor que lo hagas con el package [`forcats`](https://forcats.tidyverse.org/). No lo he usado, pero el paquete [`questionr`](https://juba.github.io/questionr/articles/recoding_addins.html) tiene un adding para recodificar variables, entre ellos factores, en R.

Recodificar variables es una tarea muy común en análisis de datos y, a veces, suele ser fuente de errores. Por ejemplo, en [este post](https://www.datasurg.net/2019/10/15/jama-retraction-after-miscoding-new-finalfit-function-to-check-recoding/) nos cuentan un error en la recodificación de una variable que llevo a que un artículo tuviera que ser retirado. No se si el error de codificación llevó a errores en la vida real, pero el artículo analizaba tratamientos en pacientes hospitalizados.

### Creación de factores

Por ejemplo, podemos crear un vector de tipo character con 5 observaciones

``` r
aa <- c("lunes", "martes", "jueves", "lunes", "martes")
aa
#> [1] "lunes"  "martes" "jueves" "lunes"  "martes"
```

De momento `aa` es un vector de texto. Si quisiéramos convertirlo a factor podríamos hacer lo siguiente:

``` r
aa_factor <- as.factor(aa)
is.factor(aa_factor)
#> [1] TRUE
```

Sí, efectivamente, ahora `aa_factor` es un vector, sí, pero es un vector especial, es un un factor. Vamos a imprimirlo para ver si ha cambiado algo.

``` r
aa_factor
#> [1] lunes  martes jueves lunes  martes
#> Levels: jueves lunes martes
```

Sí ahora al imprimir `aa_factor`, como es un factor, R nos ofrece más información. Un factor es un vector con atributos (con más información); en concreto un factor necesariamente tiene un atributo que son los `levels`, que nos indica cuantos grupos o categorías tiene el factor y cómo se llaman las categorías. En nuestro caso `aa_factor` tiene 3 levels o categorías.

``` r
levels(aa_factor)
#> [1] "jueves" "lunes"  "martes"
```

Vuelvo a repetirlo. `aa_factor` es un factor, OK. Como es un factor, resulta que es un vector con un atributo especial, los `levels` (los grupos o categorías). En nuestro caso, `aa_factor` es un vector con 5 observaciones y 3 grupos/categorias/levels. No es tan complicado.

En realidad, los factores sí son un poco más raros de lo que he explicado. Por razones históricas, se trataba de ahorrar memoria en el ordenador, los `levels` (o niveles )se utilizan para mostrar la información, PERO internamente la información se almacena con un vector de enteros y eso a veces genera (o generaba) cosas digamos extrañas. No importa mucho si no lo entiendes del todo. Fíjate, los factores se muestran como texto pero en realidad internamente son enteros:

``` r
aa_factor
#> [1] lunes  martes jueves lunes  martes
#> Levels: jueves lunes martes
typeof(aa_factor)     #- internamente lo almacena como enteros !!
#> [1] "integer"
```

<br>

### El orden de los `levels`

El orden de los `levels` es importante, principalmente al hacer gráficos y tablas. Por defecto, R ordena los levels de forma alfabética y esto no siempre es adecuado. Veamos cual es el orden de los niveles en `aa_factor`

``` r
levels(aa_factor)
#> [1] "jueves" "lunes"  "martes"
```

Como por defecto los niveles se ordenan alfabéticamente, en nuestro `aa_factor` los

PERO hay funciones para reordenar los `levels`, por ejemplo:

``` r
relevel(aa_factor, "martes")
#> [1] lunes  martes jueves lunes  martes
#> Levels: martes jueves lunes
```

También podemos crear el factor directamente:

``` r
aa_factor_2 <- factor(aa, levels = c("lunes", "martes", "jueves"))
aa_factor_2
#> [1] lunes  martes jueves lunes  martes
#> Levels: lunes martes jueves
```

Aquí el orden de los levels lo hemos elegido nosotros. No hemos usado el orden alfabético sino el orden habitual en los días de la semana.

Ya dije que un factor es un vector con atributos. Veámoslo:

``` r
aa <- 1:10
attributes(aa)
#> NULL

aa_factor_2 <- factor(aa, levels = c("lunes", "martes", "jueves"))
attributes(aa_factor_2)
#> $levels
#> [1] "lunes"  "martes" "jueves"
#> 
#> $class
#> [1] "factor"
```

El objeto `aa_factor_2` es un factor de R, aunque en el fondo no es más que un vector con atributos: los “levels” y “class”

### Más cosas sobre factores

Durante el curso trabajaremos con variables categóricas y, por tanto, usaremos factores. Para ello utilizaremos el paquete `forcats`. Si lo necesitáis seguro que encontráis tutoriales o cursos en la web, pero [aquí](https://rstatisticsblog.com/r-beginners/working-with-factors-in-r-tutorial-forcats-package/?utm_source=rss&utm_medium=rss&utm_campaign=working-with-factors-in-r-tutorial-forcats-package) tenéis uno de ellos; aunque quizás sea mejor acudir a la [web de `forcats`](https://forcats.tidyverse.org/).

Un buen resumen visual de qué son los factores es el siguiente mapa conceptual de [este repo](https://github.com/spcanelon/concept-maps):

<div class="figure" style="text-align: center">

<img src="https://raw.githubusercontent.com/spcanelon/concept-maps/master/en/factors.svg" alt="Creado por Ildiko Czeller y Graham Parsons" width="90%" />
<p class="caption">
Figure 2: Creado por Ildiko Czeller y Graham Parsons
</p>

</div>

<br>

# 6. Listas

Esta estructura de datos, aunque en realidad se construye por la agrupación de vectores, sí que se comporta de forma diferente a los vectores[^16]. Las listas son una estructura de datos heterogénea: sí que pueden contener elementos de distinto tipo.

La mejor forma de entender como funciona una lista es pensar que es como una cajonera. En cada cajón podemos poner diferentes cosas, encada cajón podemos poner objetos de diferentes tipos.

Para definir una lista se hace uso de la función `list()`. Creemos nuestra primera lista:

``` r
# defino 3 vectores y una matriz
vec_numerico <- c(1:8)
vec_character <- c("Pedro", "Rebeca", "Susana")
vec_logic <- c(TRUE, FALSE, TRUE)
matriz <- matrix(1:6, nrow = 2, ncol = 3)

# creo una lista con cuatro elementos
my_list <- list(vec_numerico, vec_character, vec_logic, matriz)
my_list
#> [[1]]
#> [1] 1 2 3 4 5 6 7 8
#> 
#> [[2]]
#> [1] "Pedro"  "Rebeca" "Susana"
#> 
#> [[3]]
#> [1]  TRUE FALSE  TRUE
#> 
#> [[4]]
#>      [,1] [,2] [,3]
#> [1,]    1    3    5
#> [2,]    2    4    6
```

Podemos crear la misma lista pero añadiendo nombres a los distintos elementos. Puede sernos útil a la hora de hacer subsetting en una lista.

``` r
my_list <- list(slot_1 = vec_numerico, slot_2 = vec_character, slot_3 = vec_logic, slot_4 =matriz)
my_list
#> $slot_1
#> [1] 1 2 3 4 5 6 7 8
#> 
#> $slot_2
#> [1] "Pedro"  "Rebeca" "Susana"
#> 
#> $slot_3
#> [1]  TRUE FALSE  TRUE
#> 
#> $slot_4
#>      [,1] [,2] [,3]
#> [1,]    1    3    5
#> [2,]    2    4    6
```

Las listas no tienen dimensiones tienen `length()`

``` r
length(my_list) #- nuestra lista tiene 4 slots, 4 elementos
#> [1] 4
```

Las listas son sumamente flexibles porque un elemento de una lista puede ser otra lista.

``` r
my_list_2 <- list(primer_slot = c(44:47), segundo_slot = my_list)
my_list_2
#> $primer_slot
#> [1] 44 45 46 47
#> 
#> $segundo_slot
#> $segundo_slot$slot_1
#> [1] 1 2 3 4 5 6 7 8
#> 
#> $segundo_slot$slot_2
#> [1] "Pedro"  "Rebeca" "Susana"
#> 
#> $segundo_slot$slot_3
#> [1]  TRUE FALSE  TRUE
#> 
#> $segundo_slot$slot_4
#>      [,1] [,2] [,3]
#> [1,]    1    3    5
#> [2,]    2    4    6
```

## Subsetting en listas

Como las listas son más complejas, tenemos más posibilidades para hacer subsetting.

Tendremos 3 operadores para hacer subsetting: `[`, `[[` y `$`.

- Empecemos con `[`. Si hacemos subsetting con `[` el objeto devuelto siempre será otra lista.

``` r
my_list[2]  #- seleccionamos el segundo elemento de la lista. Nos devuelve una lista con un solo slot
#> $slot_2
#> [1] "Pedro"  "Rebeca" "Susana"
```

``` r
my_list[c(2,3)]  #- seleccionamos el segundo y tercer elemento de la lista. Nos devuelve una lista con dos slots
#> $slot_2
#> [1] "Pedro"  "Rebeca" "Susana"
#> 
#> $slot_3
#> [1]  TRUE FALSE  TRUE
```

- con `[` también se puede seleccionar por nombre

``` r
my_list["slot_2"]  #- seleccionamos el segundo elemento de la lista. Nos devuelve una lista con un solo slot
#> $slot_2
#> [1] "Pedro"  "Rebeca" "Susana"
my_list[c("slot_2", "slot_3")]  #- seleccionamos el segundo y tercer elemento de la lista. Nos devuelve una lista con dos slots
#> $slot_2
#> [1] "Pedro"  "Rebeca" "Susana"
#> 
#> $slot_3
#> [1]  TRUE FALSE  TRUE
```

- subsetting listas con `[[`. **NO** devuelve una lista, nos devuelve el objeto que hay en el slot seleccionado

``` r
my_list[[2]]  #- seleccionamos el segundo elemento de la lista. Nos devuelve el elemento que hay en el segundo slot; es decir un vector, vec_character
#> [1] "Pedro"  "Rebeca" "Susana"
```

- subsetting, por nombre, con `$`. No devuelve una lista, sino un elemento de la lista

``` r
my_list$slot_4  #- seleccionamos el cuarto elemento de la lista, cuyo nombre es `slot_4`; es decir, nos devuelve una matriz.
#>      [,1] [,2] [,3]
#> [1,]    1    3    5
#> [2,]    2    4    6
```

- incluso se puede usar `[[` para hacer subsetting por nombre, si es que los elementos de la lista tienen nombre[^17]

``` r
my_list[["slot_4"]]  #- seleccionamos el cuarto elemento de la lista, cuyo nombre es `slot_4`; es decir, nos devuelve una matriz.
#>      [,1] [,2] [,3]
#> [1,]    1    3    5
#> [2,]    2    4    6
```

Las listas se usan para muchas cosas; por ejemplo, para almacenar los resultados de la estimación de un modelo , etc…

Las listas son sumamente flexibles porque un elemento de una lista puede ser otra lista.

``` r
my_list_2 <- list(primer_slot = c(44:47), segundo_slot = my_list)
my_list_2
#> $primer_slot
#> [1] 44 45 46 47
#> 
#> $segundo_slot
#> $segundo_slot$slot_1
#> [1] 1 2 3 4 5 6 7 8
#> 
#> $segundo_slot$slot_2
#> [1] "Pedro"  "Rebeca" "Susana"
#> 
#> $segundo_slot$slot_3
#> [1]  TRUE FALSE  TRUE
#> 
#> $segundo_slot$slot_4
#>      [,1] [,2] [,3]
#> [1,]    1    3    5
#> [2,]    2    4    6
```

¿Cómo podemos seleccionar la matriz que hay en my_list_2? Pues la matriz es uno de los cuatro elementos que hay en el segundo slot de my_list_2. Con `my_lis_2[[2]]` seleccionamos el segundo_slot, que es una lista (my_list), y en el cuarto slot de my_list esta la matriz. Así que podríamos hacerlo de varias maneras:

``` r
my_list_2[[2]][[4]]
#>      [,1] [,2] [,3]
#> [1,]    1    3    5
#> [2,]    2    4    6
my_list_2$segundo_slot$slot_4
#>      [,1] [,2] [,3]
#> [1,]    1    3    5
#> [2,]    2    4    6
```

Para terminar con las listas, [aquí](https://www.johndcook.com/blog/2015/12/02/r-lists-and-xml/) se explica visualmente la diferencia entre hacer subsetting con `[` y hacerlo con `[[`. Además se critica un poco a XML, un lenguaje de marcado que muchas veces se utiliza para almacenar e intercambiar datos.

<br>

# 7. DATA FRAMES

> A data frame is really a list where each element of the list is a single column. In other words, a data frame is a vector of columns

Los data.frames son otra estructura de R para almacenar datos. Es la estructura que más utilizaremos. Se utiliza para almacenar datos tabulares, tablas de datos, que son el formato de datos al que más acostumbrados estamos, son tablas como las que vemos en Excel etc …

En realidad un data.frame **es una lista**, pero una lista especial. Al ser una lista **puede almacenar elementos de distinto tipo** (numéricos, carácter etc…). ¿Por qué es una lista especial? Pues porque podemos pensar que es una lista restringida, restringida a que sus elementos/slots tienen que tener la misma longitud.

Como en cada slot de la lista hay un vector y todos los vectores tienen la misma longitud al final tenemos una tabla de datos. Esos vectores con la misma longitud se almacenan por columnas, así que la longitud de los vectores son el número de filas de la tabla. Habitualmente los data.frames se utilizan para almacenar datos tabulares, donde cada columna es una variable.

Otra propiedad de los data.frames es que los vectores o columnas que lo forman tienen que tener un nombre. Como habitualmente en cada columna del data.frame se almacenan los valores de una variable, el nombre de la columnas se corresponderá con el nombre de la variable.

Generalmente no crearemos data.frames sino que los importaremos de repositorios de datos, por ejemplo de Eurostat o del INE, pero hoy vamos a crear uno con la función `data.frame()`

Además, en general, en lugar de usar data.frames usaremos [tibbles](https://tibble.tidyverse.org/) o data.frames tuneados à la tidyverse. Lo veremos.

``` r
aa <- c(4, 8, 6, 3)
bb <- c("Juan", "Paz", "Adrian", "Marquitos")
cc <- c(FALSE, TRUE, TRUE, FALSE)
df <- data.frame(aa, bb, cc)
df
#>   aa        bb    cc
#> 1  4      Juan FALSE
#> 2  8       Paz  TRUE
#> 3  6    Adrian  TRUE
#> 4  3 Marquitos FALSE
```

En nuestro `df` tenemos 3 variables, cada una de ellas con 4 observaciones.

Podemos ponerle otros nombres a las columnas, nombres que tengan sentido y que nos recuerden las variables que contienen:

``` r
df <- data.frame(Nota = aa, Nombre = bb, Aprobado = cc)
names(df)  #- con names() podemos ver los nombres de las variables del df
#> [1] "Nota"     "Nombre"   "Aprobado"
```

Podemos cambiar los nombres de las columnas con `names()` o de más formas, como con `rlang::set_names()` o con `magrittr::set_colnames()` como se muestra [aquí](https://github.com/sharlagelfand/twofunctionsmostdays/tree/master/2020/03/05#purrrset_names---new-to-me).

``` r
(names(df) <- c("Grade", "Name", "Pass"))
#> [1] "Grade" "Name"  "Pass"
```

## Subsetting en data.frames

La verdad es que cuando tengamos que hacer subsetting en un data.frame, lo haremos à la tidyverse, pero conviene al menos conocer lo básico de como hacer subsetting con R-base.

El subsetting en data.frame à la R-base es muy una mezcla entre el subsetting para matrices y para listas.

1)  Subsetting como si fuera una matriz. Con `[`.

``` r
df_s <- df[,1]       #- seleccionamos la primera columna. devuelve un vector !!!
df_s <- df[,c(2,3)]  #- seleccionamos la segunda y tercera columna. devuelve un df
df_s <- df[1, ]      #- seleccionamos primera fila de todas las variables. devuelve un df. ¿xq no devuelve un vector? Preguntad si no lo sabéis
df_s <- df[c(1,4), ]  #- seleccionamos primera y cuarta fila. devuelve un df
df_s <- df[2, 3]      #- seleccionamos segunda observación de la tercera variable. Devuelve un vector.
```

2)  Subsetting como si fuera una lista. De hecho un df es una clase especial de lista. Podemos usar 3 operadores: `[`, `[[` y `$`.

- subsetting con `[` como si fuera una lista

``` r
df_s <- df[3]        #- devuelve un df. Good!!
df_s <- df[c(1,2)]

#- también se puede hacer por nombre
df_s <- df["Name"]                #- devuelve un df
df_s <- df[c("Name", "Grade")]   
```

- subsetting con `[[` como si fuera una lista

``` r
df_s <- df[[2]]   #- Extraemos la segunda columna. Devuelve un vector, concretamente un factor. Ahhhh!!!!!
```

- subsetting con `$`. Como si fuera una lista (por nombre de los elementos, en este caso los elementos de la lista son las columnas o variables del df)

``` r
df_s <- df$Name   #- Extraemos la columna con nombre "Name". Devuelve un vector, concretamente un factor. Ahhhh!!!!!
df_s <- df$Grade  #- Extraemos la columna con nombre "Grade". Devuelve un vector numérico
```

Hay más formas de hacer subsetting con data.frames, por ejemplo con `subset()`, pero ya he dicho que el manejo de tablas o data.frames lo haremos principalmente con funciones del tidyverse, principalmente funciones del paquete `dplyr`. Lo veremos en otro tutorial.

- con `[` podemos, al igual que en los vectores y matrices, hacer subsetting lógico:

``` r
df_s <- df[df$Grade >= 5, ]   #- selecciono filas que cumplan que el valor de la columna grade sea >= a 5
df_s <- df[!df$Grade >= 5, ]  #- los que NO han sacado igual o mas  de 5
df_s <- df[df$Grade == 8 | df$Grade < 5, ]  #- los que han sacado exactamente 8 ó menos de 5
```

## Funciones útiles

Hay muchas, por ejemplo:

``` r
names(df)    #- devuelve un vector con los nombre de las columnas/variables del df
#> [1] "Grade" "Name"  "Pass"
nrow(df)     #- devuelve el nº de filas
#> [1] 4
ncol(df)     #- nº de columnas
#> [1] 3
length(df)   #- la longitud de las columnas/vectores que componen el df; osea devuelve otra vez el nº de filas
#> [1] 3
```

Podemos añadir columnas a nuestro df:

``` r
aa <- 101:104
df$new_v <- aa
```

También así:

``` r
df_new <- cbind(df, aa)
```

Con la función `as.data.frame()`, podemos convertir un vector o una matriz, e incluso algunas listas, en data.frames.

``` r
aa <- 1:5
df_new <- as.data.frame(aa)  #- df con una sola columna
```

Un resumen del dataframe con `summary()`

``` r
summary(df)
#>      Grade          Name              Pass             new_v      
#>  Min.   :3.00   Length:4           Mode :logical   Min.   :101.0  
#>  1st Qu.:3.75   Class :character   FALSE:2         1st Qu.:101.8  
#>  Median :5.00   Mode  :character   TRUE :2         Median :102.5  
#>  Mean   :5.25                                      Mean   :102.5  
#>  3rd Qu.:6.50                                      3rd Qu.:103.2  
#>  Max.   :8.00                                      Max.   :104.0
```

Y muchas más.

# 8. Paquetes (packages)

Ya sabemos que R tiene muchos paquetes, ya hemos utilizado alguno. ¿Que qué son los paquetes? Pues son colecciones/porciones de código R que podemos instalar en nuestro ordenador y después cargar en nuestra sesión. ¿Qué ganamos con ello? Los paquetes nos proveen de nuevas funciones o nuevos datos; es decir incrementa la funcionalidad de R: R podrá hacer más cosas. Es como instalar una nueva app en tu teléfono.

Imagina que quieres usar R para analizar datos de Eurostat. En ese caso podemos ir directamente a la web de Eurostat, pero es mucho más cómodo instalarnos el paquete [`eurostat`](https://ropengov.github.io/eurostat/) que contiene una serie de funciones que nos facilitan el uso de datos de Eurostat en R; o a lo mejor quieres analizar datos relacionados con la pandemia covid-19. Podrías tratar de recopilar datos por ti mismo pero existen unos cuantos paquetes que ya lo han hecho, por ejemplo, para datos españoles, el paquete [`escovid19data`](https://github.com/montera34/escovid19data).

Para poder usar un paquete ya sabéis que hay que hacer 2 cosas:

1)  Instalar el package en tu ordenador. Sólo hace falta hacerlo una vez. Generalmente con `install.packages("my_pkg")`

2)  Cargar el paquete en memoria. Cada vez que vayas a usar un paquete tendrás que abrirlo, tendrás que hacer accesible el paquete a la memoria de R con library(“my_pkg”).

<br>

#### Instalación de paquetes

Ya sabes que hay un repositorio oficial de paquetes, [CRAN](https://cran.r-project.org/); pero hay muchos otros repositorios, uno de los más famosos y utilizados es [Github](https://github.com/).

Para instalar un paquete de CRAN tienes que usar `install.packages()`.

Para instalar paquetes de otros repositorios se pueden utilizar varios paquetes, pero yo últimamente estoy usando el paquete [`remotes`](https://github.com/r-lib/remotes#readme). El paquete `remotes` permite instalar paquetes alojados en GitHub, GitLab, Bitbucket, etc…

Por ejemplo para instalar un paquete de Github se utiliza: `remotes::install_github("usuario/package")`. Por ejemplo, para instalar el paquete [`emo`](https://github.com/hadley/emo) del usuario [`hadley`](https://github.com/hadley) se haría lo siguiente: `remotes::install_github("hadley/emo")`.

<br>

#### Obtener información sobre un pkg

Instalar un paquete es sencillo, pero para usarlo, generalmente, tendrás que acceder a la documentación del paquete. Los paquetes tienen mucha información sobre como usar sus funciones, sólo hay que saber buscarla.

Veamos un ejemplo concreto. Supongamos que queremos usar el paquete [`eurostat`](https://ropengov.github.io/eurostat/). Para conocer que funcionalidades tiene este paquete y cómo usar sus funciones tenemos varias alternativas:

1.  Si el paquete está en CRAN, pues ir a su página web en CRAN. El paquete. `eursotat` sí está alojado en CRAN, concretamente [aquí](https://cran.r-project.org/web/packages/eurostat/index.html), y hacía el final de esa página está la documentación. Todos los packages en CRAN tienen un **Reference Manual**: un pdf con documentación extensa de cada una de las funciones del pkg. Habitualmente los packages también tienen unos documentos llamados **vignettes** que explican de forma más genérica para qué sirve y cómo se usa el paquete.

2.  Además de en CRAN, es muy habitual que los paquetes estén alojados en otros repositorios, generalmente en Github. `eurostat` está alojado en Github [aquí](https://github.com/rOpenGov/eurostat)

3.  Cada vez es más frecuente que los paquetes tengan su propia página web donde ese explica detalladamente las funcionalidades del paquete. Si un paquete tiene página web, visitarla suele ser la mejor opción para aprender como usarlo. Por ejemplo, la página web del pkg `eurostat` está [aquí](https://ropengov.github.io/eurostat/).

#### Información interna sobre un pkg

Además de poder buscar ayuda sobre un package en la web, se puede acceder a la documentación de un paquete , tanto al reference manual como a las vignettes, directamente desde R/RStudio. Tienes que hacer lo siguiente:

``` r
#- abrimos en RStudio la ayuda del pkg eurostat
help(package = eurostat)
```

**Además**, recordad que ya sabemos que cada función tiene su propia ayuda interna. Puedes acceder a ella con `help(nombre_de_la_funcion)` o situando el cursor en el nombre de la función y pulsar la tecla <kbd>F1</kbd>

<br>

#### Obtener un listado de las funciones de un pkg

Hay varias formas, pero esta funciona:

``` r
library(tidyverse)
aa <- as.data.frame(ls("package:readr", all = TRUE))
```

<br>

#### ¿Cómo saber a que package pertenece una función?

A veces es conveniente saber a que package pertenece una función. Podemos hacerlo con:

``` r
#- usamos la función"find" para encontrar en que package está la función "mean"
find("mean")
```

<br>

------------------------------------------------------------------------

# 9. Más cosas a conocer

En esta sección presentaré algunas ideas y tópicos que creo pueden seros de utilidad.

## Algunas funciones útiles

- `%in%`: retorna un vector de booleans (TRUE or FALSE) para cada uno de los valores del vector a la izquierda dependiendo de si el valor se encuentra o no en el vector de la derecha.

``` r
?`%in%`  #- para ver la ayuda del operador
1:10 %in% c(1,3,5,9)
#>  [1]  TRUE FALSE  TRUE FALSE  TRUE FALSE FALSE FALSE  TRUE FALSE
```

- `str()`: muestra la estructura de un objeto

``` r
str(iris)
#> 'data.frame':	150 obs. of  5 variables:
#>  $ Sepal.Length: num  5.1 4.9 4.7 4.6 5 5.4 4.6 5 4.4 4.9 ...
#>  $ Sepal.Width : num  3.5 3 3.2 3.1 3.6 3.9 3.4 3.4 2.9 3.1 ...
#>  $ Petal.Length: num  1.4 1.4 1.3 1.5 1.4 1.7 1.4 1.5 1.4 1.5 ...
#>  $ Petal.Width : num  0.2 0.2 0.2 0.2 0.2 0.4 0.3 0.2 0.2 0.1 ...
#>  $ Species     : Factor w/ 3 levels "setosa","versicolor",..: 1 1 1 1 1 1 1 1 1 1 ...
```

<br>

<br>

## Directorio de trabajo

Cuando trabajamos con R es importante conocer la noción de directorio de trabajo. Es la carpeta donde R busca por defecto cuando le pidas que abra unos datos o donde los grabará.Muchas veces tendremos que importar o exportar datos así que tenemos que conocer cual es nuestro directorio de trabajo y cómo podemos cambiarlo.

- Para conocer el directorio de trabajo actual usa la función `getwd()`

- Si quisiéramos cambiar el directorio de trabajo podemos hacerlo con la función `setwd()`

Nosotros trabajaremos con Rprojects y el paquete `here` así que generalmente no necesitaremos estas funciones pero conviene conocerlas.

Cuando trabajas con Rprojects, el directorio de trabajo es la propia carpeta del proyecto. La ventaja de esto es que en lugar de rutas absolutas podemos usar rutas relativas y esto facilita la reproducibilidad de nuestros análisis.

Además de trabajar con proyectos usaremos, al meno yo, la función `here()` del paquete `here`. La razón es que quiero poder knitear los .Rmd desde cualquier carpeta del proyecto.

<br>

## NA’s y valores especiales

Recordáis que en una sección anterior dijimos que los principales tipos de datos son 3: numéricos, de texto y lógicos, pero que existían unos valores especiales: `NULL`, `NA`, `NaN` e `Inf`. Veámoslos un poco:

- `NULL`: representa el objeto vacío en R. No se propaga.

``` r
c()
#> NULL
sum(2, 2, NULL)
#> [1] 4
mean(c(2 ,4, NULL))
#> [1] 3
```

- `NA`: Un valor no disponible. Sí se propaga, así que cuando tengamos que calcular medias etc… con vectores que contengan NAs hay que tener cuidado, habrá que usar la opción `na.rm = TRUE`.

``` r
sum(2, 2, NA)
#> [1] NA
mean(c(2 ,4, NA))
#> [1] NA
mean(c(2, 4, NA), na.rm = TRUE)
#> [1] 3
```

- `NaN`: Not a number. Se propaga

``` r
0/0
#> [1] NaN
sum(2, 2, NaN)
#> [1] NaN
mean(c(2 ,4, 0/0))
#> [1] NaN
```

- `Infinito`:

``` r
1/0
#> [1] Inf
-1/0
#> [1] -Inf
sum(2, 2, Inf)
#> [1] Inf
```

## Secuencias

Muchas veces hay que crear secuencias de números. Para ello disponemos de las funciones `:`, `seq()` y `rep()`. Por ejemplo:

- con `:` el incremento siempre es unitario. Devuelve enteros.

``` r
1:3
#> [1] 1 2 3
c(1:4)
#> [1] 1 2 3 4
-2:3
#> [1] -2 -1  0  1  2  3
4:-1
#> [1]  4  3  2  1  0 -1
```

- `seq()`

``` r
seq(from = 0, to = 5, by = 1)
#> [1] 0 1 2 3 4 5
seq(-5, 5, 2)
#> [1] -5 -3 -1  1  3  5

seq(0, 1, length.out = 3)
#> [1] 0.0 0.5 1.0
seq(0, 1, length.out = 5)
#> [1] 0.00 0.25 0.50 0.75 1.00
seq(0, 1, 5)
#> [1] 0
```

- `rep()`

``` r
rep(2, times= 3)
#> [1] 2 2 2
rep(1:3, 2)
#> [1] 1 2 3 1 2 3
rep(1:3, each = 2)       # not the same.
#> [1] 1 1 2 2 3 3
rep(1:3, times = 3, each = 2)
#>  [1] 1 1 2 2 3 3 1 1 2 2 3 3 1 1 2 2 3 3
rep(1:2, length.out = 9)
#> [1] 1 2 1 2 1 2 1 2 1
```

<br>

# 10. Algunos chunks

1.  Eliminar todos los objetos del Global Environment **EXCEPTO** los que tú decidas.

Para eliminar un objeto de la memoria puedes usar la función `rm()`. Para quitar un objeto solo has de hacer `rm(objeto)`, pero si quieres eliminar todos los objetos excepto los que necesites:

``` r
aa <- 1
bb <- 2
cc <- 3
dd <- 4
quiero_dejar_estos <- c("cc", "dd")                #- fíjate que los nombres de los objetos están entre comillas
rm(list = ls()[!(ls() %in% quiero_dejar_estos)])   #- remueve todo excepto quiero_dejar_estos
```

2.  Función para comparar los elementos de dos vectores.

Inspirados por [este tweet](https://twitter.com/tyluRp/status/1197634755430367235) vamos a crear nuestra primera función:

``` r
my_f_compare <- function(x, y){
  list(
  "Valores de X q. no están en Y:" = setdiff(x, y),
  "Valores de Y q. no están en X:" = setdiff(y, x),
  "Valores comunes en X e Y:" = intersect(x, y),
  "La unión de X e Y sería:" = union(x,y), 
  "Si juntamos X e Y obtenemos:" = c(x, y) )
}
```

Trata de entenderlo Paul

``` r
XX <- c(1:4)
YY <- c(3:6)
aa <- my_f_compare(XX, YY)
names(aa)
#> [1] "Valores de X q. no están en Y:" "Valores de Y q. no están en X:"
#> [3] "Valores comunes en X e Y:"      "La unión de X e Y sería:"      
#> [5] "Si juntamos X e Y obtenemos:"
aa
#> $`Valores de X q. no están en Y:`
#> [1] 1 2
#> 
#> $`Valores de Y q. no están en X:`
#> [1] 5 6
#> 
#> $`Valores comunes en X e Y:`
#> [1] 3 4
#> 
#> $`La unión de X e Y sería:`
#> [1] 1 2 3 4 5 6
#> 
#> $`Si juntamos X e Y obtenemos:`
#> [1] 1 2 3 4 3 4 5 6
```

<br>

# 11. R 4.1.0

Con la llegada de R 4.1.0 se produjo un cambio importante en la comunidad R: apareció la **pipe nativa** `>|`[^18]. Una comparación exhaustiva de la pipe nativa con la pipe de magrittr puede encontrarse [aquí](https://michaelbarrowman.co.uk/post/the-new-base-pipe/)

La pipe original ( %\>% ), la de Stefan Bache en el paquete magrittr, es un operador fundamental para el tidyverse que ha cambiado la forma de escribir código en R. ¿Sustituirá la pipe nativa ( \|\> ) a la original ( %\>% ), ¿lo veremos?

``` r
mtcars |> group_by(cyl) |> summarise(mpg = mean(mpg))
```

Una ventaja evidente del pipe nativa es que es nativa, se puede usar sin tener que instalar ni cargar ningún paquete, menos dependencias!!; además, solo está compuesta de 2 caracteres frente a los 3 de la original.

Una desventaja de la nativa es que no puede usar `.` como placeholder para llevar el objeto de la izquierda a, por ejemplo, el segundo o tercer argumento de la función de la derecha. Por ejemplo, no se puede hacer esto con la pipe nativa:

``` r
2 %>% head(iris, n = .)
```

La forma de solucionarlo es usar funciones anónimas (un poco feo!!):

``` r
2 |> (function(x) head(iris, n = x)
```

Lo anterior mejora un poco (la verdad es que bien poco) si usamos la nueva sintaxis (shorthand) para funciones anónimas o lambda functions[^19]:

``` r
#- estas dos lineas producen idénticos resultados
function(x) x + 1 
\(x) x + 1
```

``` r
2 |> (\(x) head(iris, x = n))()
```

Aunque en [este tweet](https://twitter.com/matthiasgomolka/status/1404821668695007237) se dice que si puedes llevar el objeto de la izquierda aun argumento distinto del primero, si los anteriores argumentos tienen puesto el nombre, ya que “The pipe pipes into the first unnamed argument, I guess.”

# Biblio

- [Base R Cheat Sheet](https://rstudio.com/wp-content/uploads/2016/10/r-cheat-sheet-3.pdf) (https://github.com/saghirb/Getting-Started-in-R). Una buena chuleta de 2 páginas con las principales ideas y funciones para iniciarse con R. Hay muchas más, por ejemplo, [esta]((https://github.com/saghirb/Getting-Started-in-R)) o [esta](http://datasciencefree.com/basicR.pdf).

- [aRrgh: a newcomer’s (angry) guide to R](http://arrgh.tim-smith.us/): un pitonista (programador que usa Phyton) que se queja y describe las cosas de R que él ve raras (gotchas); aunque va admitiendo, poco a poco, que le va empezando a gustar R.

- [forcats for factors](https://craig.rbind.io/post/2020-08-29-asgr-2-4-factors/). Un artículo sencillo y actual sobre factores.

[^1]: De momento no estoy empleando la terminología correcta

[^2]: También se puede utilizar el operador `=` pero, en general, la comunidad R usa **`<-`**.

[^3]: En realidad son 6 porque R tiene también complex y raw types

[^4]: Sin embargo, si elevas un NA a cero, el resultado sera 1, porque todo número elevado a cero es 1. De la misma manera si ejecutas `NA | TRUE` devolverá TRUE

[^5]: R no entiende el concepto de escalar. Entre sus estructuras de datos no están los escalares. para R el número 9 es en realidad un vector con un solo elemento con valor 9

[^6]: Un array es muy similar a matrix, sólo que una matriz solo puede tener 2 dimensiones, filas y columnas, mientras que un array puede tener más de 2 dimensiones; es decir, las array son matrices mutidimensionales

[^7]: Aquí puedes consultar la especificación oficial del lenguaje R: https://cran.r-project.org/doc/manuals/r-release/R-lang.html

[^8]: De hecho en R no existen los escalares: para R un núnico numero es un vector de 1 elemento

[^9]: En realidad 6 si incluimos complex y raw types

[^10]: Augmented porque se construyen, a partir los vectores fundamentales, añadiendo información extra en los atributos del vector original o fundamental!! Si cuesta un poco entenderlo!! Con tener una ligera idea es suficiente

[^11]: Lo importante a saber de un factor es qué se puede hacer con él, lo veremos!!, y no tanto saber que un factor es realidad un vector de integers pero que como tiene un atributo que dice que su class es factor entonces se comporta de forma especial ante algunas funciones.

[^12]: de hecho cuando hacíamos `sqrt(9)` también introducíamos un vector porque, para R, 9 es un vector de un sólo elemento

[^13]: Esta sección se me ocurrió introducirla tras leer el libro <https://smac-group.github.io/ds/data.html#useful-functions-with-vectors>

[^14]: Esta historia os la contaré en clase

[^15]: Se usan para representar variables categóricas, pero internamente la información se almacena en un vector de enteros, PERO tienen también un vector de caracteres o `levels` que se utiliza para mostrar la información. Buff, lo explicaré en clase

[^16]: Aunque en realidad las listas se construye por la agrupación recursiva de vectores.

[^17]: Hadley nos avisa que esta forma de hacer subsetting por nombre es mejor porque `$` hace partial matching.

[^18]: Como se dice [aquí](https://eliocamp.github.io/codigo-r/en/2021/05/r-pipa-nativa/), la versión 4.0 ya vino con un cambio histórico: se acabo con `stringAsFactors = TRUE`. Además el post sugiere una solución para la falta de placeholder en la pipe nativa

[^19]: [Aquí](https://twitter.com/rabaath/status/1335226691304775681) un hilo de Twitter sobre las lambda functions
