---
title: 'Tema 8: Tablas en documentos Rmarkdown'
author: Edison Achalma Mendoza
date: '2023-01-07'
slug: tema-8-tablas-en-documentos-rmarkdown
categories: []
tags: []
---

<script src="{{< blogdown/postref >}}index_files/clipboard/clipboard.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/primer-tooltips/build.css" rel="stylesheet" />
<link href="{{< blogdown/postref >}}index_files/klippy/css/klippy.min.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/klippy/js/klippy.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/kePrint/kePrint.js"></script>
<link href="{{< blogdown/postref >}}index_files/lightable/lightable.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/kePrint/kePrint.js"></script>
<link href="{{< blogdown/postref >}}index_files/lightable/lightable.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/kePrint/kePrint.js"></script>
<link href="{{< blogdown/postref >}}index_files/lightable/lightable.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/kePrint/kePrint.js"></script>
<link href="{{< blogdown/postref >}}index_files/lightable/lightable.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/kePrint/kePrint.js"></script>
<link href="{{< blogdown/postref >}}index_files/lightable/lightable.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/kePrint/kePrint.js"></script>
<link href="{{< blogdown/postref >}}index_files/lightable/lightable.css" rel="stylesheet" />
<link href="{{< blogdown/postref >}}index_files/tabwid/tabwid.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/htmlwidgets/htmlwidgets.js"></script>
<script src="{{< blogdown/postref >}}index_files/jquery/jquery.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/datatables-css/datatables-crosstalk.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/datatables-binding/datatables.js"></script>
<link href="{{< blogdown/postref >}}index_files/dt-core/css/jquery.dataTables.min.css" rel="stylesheet" />
<link href="{{< blogdown/postref >}}index_files/dt-core/css/jquery.dataTables.extra.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/dt-core/js/jquery.dataTables.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/crosstalk/css/crosstalk.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/crosstalk/js/crosstalk.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/htmlwidgets/htmlwidgets.js"></script>
<script src="{{< blogdown/postref >}}index_files/jquery/jquery.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/datatables-css/datatables-crosstalk.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/datatables-binding/datatables.js"></script>
<link href="{{< blogdown/postref >}}index_files/dt-core/css/jquery.dataTables.min.css" rel="stylesheet" />
<link href="{{< blogdown/postref >}}index_files/dt-core/css/jquery.dataTables.extra.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/dt-core/js/jquery.dataTables.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/nouislider/jquery.nouislider.min.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/nouislider/jquery.nouislider.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/selectize/selectize.bootstrap3.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/selectize/selectize.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/crosstalk/css/crosstalk.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/crosstalk/js/crosstalk.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/htmlwidgets/htmlwidgets.js"></script>
<script src="{{< blogdown/postref >}}index_files/jquery/jquery.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/datatables-css/datatables-crosstalk.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/datatables-binding/datatables.js"></script>
<link href="{{< blogdown/postref >}}index_files/dt-core/css/jquery.dataTables.min.css" rel="stylesheet" />
<link href="{{< blogdown/postref >}}index_files/dt-core/css/jquery.dataTables.extra.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/dt-core/js/jquery.dataTables.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/jszip/jszip.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pdfmake/pdfmake.js"></script>
<script src="{{< blogdown/postref >}}index_files/pdfmake/vfs_fonts.js"></script>
<link href="{{< blogdown/postref >}}index_files/dt-ext-buttons/css/buttons.dataTables.min.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/dt-ext-buttons/js/dataTables.buttons.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/dt-ext-buttons/js/buttons.html5.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/dt-ext-buttons/js/buttons.colVis.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/dt-ext-buttons/js/buttons.print.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/crosstalk/css/crosstalk.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/crosstalk/js/crosstalk.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/core-js/shim.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/react/react.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/react/react-dom.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/reactwidget/react-tools.js"></script>
<script src="{{< blogdown/postref >}}index_files/htmlwidgets/htmlwidgets.js"></script>
<link href="{{< blogdown/postref >}}index_files/reactable/reactable.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/reactable-binding/reactable.js"></script>
<script src="{{< blogdown/postref >}}index_files/kePrint/kePrint.js"></script>
<link href="{{< blogdown/postref >}}index_files/lightable/lightable.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/htmlwidgets/htmlwidgets.js"></script>
<script src="{{< blogdown/postref >}}index_files/jquery/jquery.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/jquery-ui/jquery-ui.min.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/jquery-ui/jquery-ui.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/jquery-ui/jquery.ui.touch-punch.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/c3/c3.min.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/c3/c3.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/d3/d3.v3.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/pivottable/pivot.min.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/d3_renderers.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/c3_renderers.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.cs.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.da.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.de.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.es.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.fr.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.it.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.nl.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.pl.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.pt.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.ru.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.sq.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.tr.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/pivottable/pivot.zh.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/subtotal/subtotal.min.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/subtotal/subtotal.min.js"></script>
<script src="{{< blogdown/postref >}}index_files/polyfill/polyfill.min.js"></script>
<link href="{{< blogdown/postref >}}index_files/rpivotTable_style/rpivotTable.css" rel="stylesheet" />
<script src="{{< blogdown/postref >}}index_files/rpivotTable-binding/rpivotTable.js"></script>
<script>
  addClassKlippyTo("pre.r, pre.markdown");
  addKlippy('right', 'top', 'auto', '1', 'Copy code', 'Copied!');
</script>

------------------------------------------------------------------------

<br>

# 1. Introducci??n

Hacer cuadros/tablas para mostrar resultados es una parte importante (y time consuming) de cualquier informe o investigaci??n. En este tutorial explicar?? como presentar nuestros resultados en tablas en documentos (ya sean estos .html, .pdf etc..) creados a partir de archivos `.Rmd`.

Veremos que presentar los resultados (previamente almacenados en un df) como un cuadro en el documento final es muy sencillo, s??lo tenemos que llamar a la funci??n `kable()`, pero si queremos tener m??s flexibilidad y opciones para mejorar nuestras tablas tendremos que usar otros paquetes como `kableextra`, `formatable`, `flextable`, `DT` o m??s recientemente `gt` y `reactable`

En [este hilo](https://twitter.com/GoldbergData/status/1292935454195511302) de Twitter se habl?? sobre cuales eran los mejores paquetes R para hacer tablas. En [este post](https://rfortherestofus.com/2019/11/how-to-make-beautiful-tables-in-r/), David Keyes hace un muy buen tutorial sobre los paquetes disponibles para hacer tablas en R.

Al igual que con los gr??ficos, para hacer buenas tablas [^1] hace falta tener en cuenta algunos aspectos. Este [post](https://paulvanderlaken.com/2020/09/01/10-guidelines-to-better-table-design/) proporciona 10 reglas o consejos para generar tablas efectivas. En este otro [post](https://themockup.blog/posts/2020-09-04-10-table-rules-in-r/#guidelines-with-gt), Thomas Mock implementa esas 10 reglas con el paquete `gt`.

En el siguiente apartado utilizaremos unos datos de ejemplo para obtener unos resultados que queremos mostrar como tablas en nuestro informe. Esto nos servir?? para practicar un poco m??s con `dplyr` y aprender a crear tablas desde documentos .Rmd, ya que una vez tengamos los resultados que queremos mostrar, presentaremos distintas posibilidades para mostrarlos en tablas/cuadros good-looking.

------------------------------------------------------------------------

<br>

# 2. Resultados para tablas

En esta secci??n utilizaremos lo que hemos aprendido de **dplyr** para obtener los resultados que queremos mostrar en los cuadros. Con dplyr calcularemos los estad??sticos que queremos mostrar almacen??ndolos en un dataframe/tibble. Una vez tengamos los resultados en un dataframe nos quedar?? la tarea de presentarlos como cuadros en el documento final. En un primer momento (esta secci??n) utilizaremos la funci??n `knitr::kable()` para hacer tablas y en los siguientes apartados presentaremos paquetes especialmente dise??ados para hacer tablas.

## 2.1 Datos que usaremos

Ilustraremos la creaci??n de tablas con datos de la segunda ronda de **PIACC** (Programa para la Evaluaci??n Internacional de las Competencias de los adultos de la OCDE. Informaci??n detallada sobre el programa PIAAC puede encontrarse en su pagina web <http://www.oecd.org/skills/piaac/>. Los datos se obtuvieron a partir del paquete [RPIAAC](https://github.com/jcpernias/RPIAAC) creado Por Jose C. Pernias, para finalmente seleccionar 10 variables de 4 pa??ses: ESP, FRA, GBR, ITA. No recuerdo el a??o de los datos!!

Cargamos los datos que vamos a utilizar:

``` r
my_url <- "https://raw.githubusercontent.com/perezp44/iris_data/master/data/PIAAC_data_small.csv"
df <- read_csv(my_url)
```

Miramos un poco los datos:

``` r
#- remotes::install_github("perezp44/pjpv2020.01")
df_aa <- pjpv2020.01::pjp_f_estadisticos_basicos(df) #- estad??sticos b??sicos del df
df_bb <- pjpv2020.01::pjp_f_unique_values(df)        #- valores ??nicos de cada variable de df
```

<br>

## 2.2 Obteniendo resultados (con dplyr)

Para iniciar nuestra andadura con las tablas, intentaremos mostrar en tablas algunos resultados. Por ejemplo:

<br>

- 1.  Cuadro con el n??mero de observaciones de cada pa??s (lo hacemos de 2 formas)

``` r
df_tt_1 <- df %>% 
           count(Country)

df_tt_1 <- df %>% 
           group_by(Country) %>% 
           summarise(NN = n())

knitr::kable(df_tt_1)
```

| Country |   NN |
|:--------|-----:|
| ESP     | 1991 |
| FRA     | 3346 |
| GBR     | 1075 |
| ITA     | 1610 |

<br>

- 2.  A??adir a la tabla el % que representa cada pa??s en el Total (tambi??n lo hacemos de 2 formas)

``` r
df_tt_2 <- df %>% 
           group_by(Country) %>% 
           summarise(NN = n(), percent = n()/nrow(.) )

df_tt_2 <- df %>% 
           group_by(Country) %>%
           summarise (NN = n()) %>%
           mutate(percent = NN / sum(NN))

knitr::kable(df_tt_2)
```

| Country |   NN |   percent |
|:--------|-----:|----------:|
| ESP     | 1991 | 0.2481925 |
| FRA     | 3346 | 0.4171030 |
| GBR     | 1075 | 0.1340065 |
| ITA     | 1610 | 0.2006981 |

<br>

- 3.  Porcentaje de Hombres y Mujeres en cada pa??s

``` r
df_tt_3 <- df %>% 
          count(Country, Gender) %>%
          group_by(Country) %>%
          mutate(percent = n / sum(n)) %>%
          select(-n) %>%
          pivot_wider(names_from = Gender, 
                      values_from = percent) %>% 
          ungroup()

knitr::kable(df_tt_3)
```

| Country |    Female |      Male |
|:--------|----------:|----------:|
| ESP     | 0.4841788 | 0.5158212 |
| FRA     | 0.5065750 | 0.4934250 |
| GBR     | 0.6893023 | 0.3106977 |
| ITA     | 0.4850932 | 0.5149068 |

<br>

- 4.  Porcentaje de Hombres y Mujeres en cada nivel educativo

``` r
df_tt_4 <- df %>% 
           count(Education, Gender) %>% 
           group_by(Education) %>%
           mutate(percent = n / sum(n)) %>%
           select(-n) %>%
           pivot_wider(names_from = Education, 
                       values_from = percent) %>% 
           ungroup()

knitr::kable(df_tt_4)
```

| Gender |   Primary | Secondary |  Tertiary | Upper_second |  NA |
|:-------|----------:|----------:|----------:|-------------:|----:|
| Female | 0.4377224 | 0.4804831 | 0.6159875 |     0.579646 | 0.8 |
| Male   | 0.5622776 | 0.5195169 | 0.3840125 |     0.420354 | 0.2 |

<br>

- 5.  Calculamos el salario medio por pa??s

``` r
df_tt_5 <- df %>% 
           group_by(Country) %>% 
           summarise(W_hora_medio = mean(Wage_hour , na.rm = TRUE), 
                     W_mes_medio  = mean(Wage_month, na.rm = TRUE)) %>% ungroup()


knitr::kable(df_tt_5)
```

| Country | W_hora_medio | W_mes_medio |
|:--------|-------------:|------------:|
| ESP     |     9.386217 |    1437.340 |
| FRA     |    12.850094 |    1992.606 |
| GBR     |    10.624071 |    1507.472 |
| ITA     |    11.746581 |    1808.500 |

<br>

- 6.  Calculamos la media, el m??nimo, el m??ximo y la desviaci??n t??pica de Wage_month

``` r
df_tt_6 <- df %>% 
           group_by(Country) %>% 
           summarise(W_medio  = mean(Wage_month, na.rm = TRUE) ,
                     W_minimo = min(Wage_month, na.rm = TRUE)  ,
                     W_maximo = max(Wage_month, na.rm = TRUE)  ,
                     W_sd = sd(Wage_month, na.rm = TRUE) ) %>% 
          ungroup()

knitr::kable(df_tt_6)
```

| Country |  W_medio | W_minimo | W_maximo |      W_sd |
|:--------|---------:|---------:|---------:|----------:|
| ESP     | 1437.340 |      110 |     3800 |  702.6642 |
| FRA     | 1992.606 |      115 |     5850 |  906.5507 |
| GBR     | 1507.472 |      116 |    10000 | 1003.7897 |
| ITA     | 1808.500 |      150 |     5000 |  819.6863 |

<br>

- 7.  Salario medio en Espa??a (Hombres y Mujeres)

``` r
df_tt_7 <- df %>% 
           filter(Country == "ESP") %>% 
           group_by(Gender) %>% 
           summarise(W_hora_medio = mean(Wage_hour, na.rm = TRUE), 
                     W_mes_medio = mean(Wage_month, na.rm = TRUE) ) %>%
           ungroup()

knitr::kable(df_tt_7)
```

| Gender | W_hora_medio | W_mes_medio |
|:-------|-------------:|------------:|
| Female |     8.789178 |    1245.076 |
| Male   |     9.946525 |    1617.810 |

<br>

- 8.  Salario medio en los 4 los pa??ses (Hombres y Mujeres)

``` r
df_tt_8 <- df %>% 
           group_by(Country, Gender) %>% 
           summarise(W_hora_medio = mean(Wage_hour, na.rm = TRUE), 
                     W_mes_medio = mean(Wage_month, na.rm = TRUE) ) %>% 
           ungroup()

knitr::kable(df_tt_8)
```

| Country | Gender | W_hora_medio | W_mes_medio |
|:--------|:-------|-------------:|------------:|
| ESP     | Female |     8.789178 |    1245.076 |
| ESP     | Male   |     9.946525 |    1617.810 |
| FRA     | Female |    12.443723 |    1802.254 |
| FRA     | Male   |    13.266840 |    2188.032 |
| GBR     | Female |    10.609256 |    1377.953 |
| GBR     | Male   |    10.656991 |    1794.817 |
| ITA     | Female |    11.584393 |    1629.828 |
| ITA     | Male   |    11.898988 |    1976.826 |

<br>

- 9.  ??Cuanto m??s cobran los hombres (en %)?

``` r
df_tt_9 <- df %>% 
           group_by(Country, Gender) %>% 
           summarise(W_mes_medio = mean(Wage_month, na.rm = TRUE)) %>% 
           ungroup() %>% 
           pivot_wider(names_from = Gender, values_from = W_mes_medio) %>% 
           mutate(dif_W = Male-Female, dif_percent_W = dif_W/Female)

knitr::kable(df_tt_9)
```

| Country |   Female |     Male |    dif_W | dif_percent_W |
|:--------|---------:|---------:|---------:|--------------:|
| ESP     | 1245.076 | 1617.810 | 372.7344 |     0.2993669 |
| FRA     | 1802.254 | 2188.032 | 385.7784 |     0.2140533 |
| GBR     | 1377.953 | 1794.817 | 416.8640 |     0.3025240 |
| ITA     | 1629.828 | 1976.826 | 346.9983 |     0.2129048 |

<br>

- 10. Numeracy Score por pa??s y nivel de estudios. La tabla nos va a salir alargada

``` r
df_tt_10 <- df %>% 
            group_by(Country, Education) %>% 
            summarise(Numeracy_media = mean(Numeracy_score, na.rm = TRUE)) %>% 
            ungroup() 

knitr::kable(df_tt_10)
```

| Country | Education    | Numeracy_media |
|:--------|:-------------|---------------:|
| ESP     | Primary      |       213.0135 |
| ESP     | Secondary    |       245.1109 |
| ESP     | Tertiary     |       282.1070 |
| ESP     | Upper_second |       265.7699 |
| FRA     | Primary      |       184.9306 |
| FRA     | Secondary    |       246.6609 |
| FRA     | Tertiary     |       304.0075 |
| FRA     | Upper_second |       289.0088 |
| FRA     | NA           |       197.6502 |
| GBR     | Primary      |       207.3143 |
| GBR     | Secondary    |       252.9237 |
| GBR     | Tertiary     |       286.1454 |
| GBR     | Upper_second |       263.2052 |
| GBR     | NA           |       213.1912 |
| ITA     | Primary      |       200.7297 |
| ITA     | Secondary    |       257.5339 |
| ITA     | Tertiary     |       279.7166 |
| ITA     | Upper_second |       271.6400 |

- 11. Hagamos la anterior tabla m??s ancha (Una columna para cada pa??s)

``` r
df_tt_11 <- df_tt_10 %>% 
            pivot_wider(names_from = Education, 
                        values_from = Numeracy_media)

knitr::kable(df_tt_11)
```

| Country |  Primary | Secondary | Tertiary | Upper_second |       NA |
|:--------|---------:|----------:|---------:|-------------:|---------:|
| ESP     | 213.0135 |  245.1109 | 282.1070 |     265.7699 |       NA |
| FRA     | 184.9306 |  246.6609 | 304.0075 |     289.0088 | 197.6502 |
| GBR     | 207.3143 |  252.9237 | 286.1454 |     263.2052 | 213.1912 |
| ITA     | 200.7297 |  257.5339 | 279.7166 |     271.6400 |       NA |

<br>

Bien, no est?? mal, pero quiero ordenar la tabla de menor a mayor nivelo educativo

- 12. Reordenando la tabla 11

Resulta que en el cuadro, las categor??as de niveles de estudio se han ordenado alfab??ticamente pero quiero ordenarla de menor a mayor nivel de estudios. Se puede hacer de otras maneras, pero lo haremos usando **factores**.

La variable Education tiene 4 categor??as: Primary, Secondary, Upper-second y Tertiary; **ADEM??S** estas categor??as est??n/son fijas, no cambian. En estos casos es mejor tratar esas variables como **factores**; PERO si miramos la clase de la variable ???Education??? con `class(df$Education)` veremos que es character, as?? que vamos a convertir la variable ???Education??? a factor.

Podr??amos usar la funci??n `as.factor()`, pero una vez m??s usaremos pkgs del tidyverse; en este caso el pkg ???**forcats**??? y la funci??n `as_factor()`

``` r
df <- df %>% 
      mutate(Education = forcats::as_factor(Education))

levels(df$Education)
#> [1] "Primary"      "Tertiary"     "Secondary"    "Upper_second"
```

<br>

Como vemos, la variable `Education`, que ahora es un factor, tiene cuatro categor??as o ???levels???

Resulta que el nombre de las 4 categor??as est?? en ingl??s y lo queremos en castellano. Lo haremos con `forcats::fct_recode()`. Para saber un poco m??s sobre como manipular factores debes ir [aqu??](http://r4ds.had.co.nz/factors.html)

``` r
df <- df %>% 
      mutate(Education = forcats::fct_recode(Education,
                    "Primaria"         = "Primary",
                    "Secundaria"       = "Secondary", 
                    "Secundaria_post"  = "Upper_second",
                    "Terciaria"        = "Tertiary" )) 

df %>% count(Education)
#> # A tibble: 5 ?? 2
#>   Education           n
#>   <fct>           <int>
#> 1 Primaria          562
#> 2 Terciaria        1914
#> 3 Secundaria       4637
#> 4 Secundaria_post   904
#> 5 <NA>                5
```

<br>

Como volvemos a ver, la variable ???Education???, que ahora es un factor tiene 4 ???levels??? pero est??n ordenados de forma que no nos conviene, queremos cambiar el orden de los factores con `forcast::fct_relevel()` para que se muestren los cuatro grupos educativos de menor a mayor nivel.

``` r
df <- df %>% 
      mutate(Education = forcats::fct_relevel(Education, 
                             "Primaria", "Secundaria", "Secundaria_post")) 

df %>% count(Education)
#> # A tibble: 5 ?? 2
#>   Education           n
#>   <fct>           <int>
#> 1 Primaria          562
#> 2 Secundaria       4637
#> 3 Secundaria_post   904
#> 4 Terciaria        1914
#> 5 <NA>                5
```

Como se puede ver en el cuadro de arriba, ya hemos cambiado el orden de los ???levels??? para que se muestren de menor a mayor nivel educativo, as?? que volvamos a rehacer el cuadro con el Numeracy Score por pa??ses:

``` r
df_tt_12 <- df %>% 
            group_by(Country, Education) %>% 
            summarise(Numeracy_media = mean(Numeracy_score, na.rm = TRUE)) %>% 
            ungroup() %>%  
            pivot_wider(names_from = Education, 
                        values_from = Numeracy_media) 

knitr::kable(df_tt_12)
```

| Country | Primaria | Secundaria | Secundaria_post | Terciaria |       NA |
|:--------|---------:|-----------:|----------------:|----------:|---------:|
| ESP     | 213.0135 |   245.1109 |        265.7699 |  282.1070 |       NA |
| FRA     | 184.9306 |   246.6609 |        289.0088 |  304.0075 | 197.6502 |
| GBR     | 207.3143 |   252.9237 |        263.2052 |  286.1454 | 213.1912 |
| ITA     | 200.7297 |   257.5339 |        271.6400 |  279.7166 |       NA |

<br>

## 2.3 Obteniendo resultados (con janitor)

Si los resultados que queremos mostrar son cosas b??sicas como porcentajes, frecuencias etc??? obviamente podemos calcularlos nosotros con `dplyr`, pero para estos casos el paquete `janitor`, concretamente la funci??n `janitor::tabyl()` nos facilita mucho la tarea[^2]. Para ver todas las posibilidades que tiene el paquete `janitor` puedes ir a su p??gina web <a href="http://sfirke.github.io/janitor/" target="_blank">aqu??</a>.

1 y 2. Cuadro con el n??mero de observaciones de cada pa??s

``` r
df_tt_1_j <- df %>% janitor::tabyl(Country)
knitr::kable(df_tt_1_j)
```

| Country |    n |   percent |
|:--------|-----:|----------:|
| ESP     | 1991 | 0.2481925 |
| FRA     | 3346 | 0.4171030 |
| GBR     | 1075 | 0.1340065 |
| ITA     | 1610 | 0.2006981 |

3.  Porcentaje de Hombres y Mujeres en cada pa??s

``` r
df_tt_3_j <- df %>% janitor::tabyl(Country, Gender)

df_tt_3_j <- df %>% janitor::tabyl(Country, Gender) %>% 
                    janitor::adorn_percentages(denominator = "row")
df_tt_3_j
#>  Country    Female      Male
#>      ESP 0.4841788 0.5158212
#>      FRA 0.5065750 0.4934250
#>      GBR 0.6893023 0.3106977
#>      ITA 0.4850932 0.5149068
```

4.  Porcentaje de Hombres y Mujeres en cada nivel educativo

``` r
df_tt_4_j <- df %>% janitor::tabyl(Gender, Education) %>% 
                    janitor:: adorn_percentages(denominator = "col")
df_tt_4_j
#>  Gender  Primaria Secundaria Secundaria_post Terciaria NA_
#>  Female 0.4377224  0.4804831        0.579646 0.6159875 0.8
#>    Male 0.5622776  0.5195169        0.420354 0.3840125 0.2
```

Para ver todas las posibilidades que tiene el paquete `janitor` puedes ir a su p??gina web [aqu??](http://sfirke.github.io/janitor/)

<br>
Hay otros paquetes con funcionalidades parecidas a `janitor`. Por ejemplo, el paquete [`freqtables`](https://github.com/brad-cannell/freqtables) o el paquete [`sjmisc`](https://strengejacke.github.io/sjmisc/index.html).

------------------------------------------------------------------------

<br>

# 3. Tablas con `knitr::kable()`

<br>

Bueno, ya sabemos, aunque en realidad lo vimos al presentar `dplyr` y `tidyr`, como ir generando un dataframe con los estad??sticos descriptivos que nos interesa mostrar. En realidad esos df ya son tablas de datos que puedo exportar a Excel para trabajarlas a nuestro gusto; pero en el curso hacemos todo desde R.

Ya hab??is visto que con la funci??n `knitr::kable()` puedo mostrarlas en mi documento final s??lo tengo que ejecutar lo siguiente: `knitr::kable(my_df)`.

<br>

En los pr??ximos apartados mostraremos algunos paquetes espec??ficos para formatear los cuadros y hacerlos BONITOS, pero tambi??n conviene saber que **kable() tambi??n tiene opciones** para personalizar un poco nuestras tablas. Por ejemplo:

``` r
knitr::kable(df_tt_12, 
             align = "c", 
             caption = "Numeracy Score por pa??s",
             digits = 2, 
             format.args = list(decimal.mark = ",", big.mark = "."))
```

| Country | Primaria | Secundaria | Secundaria_post | Terciaria |   NA   |
|:-------:|:--------:|:----------:|:---------------:|:---------:|:------:|
|   ESP   |  213,01  |   245,11   |     265,77      |  282,11   |   NA   |
|   FRA   |  184,93  |   246,66   |     289,01      |  304,01   | 197,65 |
|   GBR   |  207,31  |   252,92   |     263,21      |  286,15   | 213,19 |
|   ITA   |  200,73  |   257,53   |     271,64      |  279,72   |   NA   |

Table 1: Numeracy Score por pa??s

------------------------------------------------------------------------

<br>

## 3.1 `kableExtra` pkg

[`kableExtra`](http://haozhu233.github.io/kableExtra/) es un package de que permite mejorar las tablas creadas con `knitr::kable()`.

La descripci??n de `kableExtra` en CRAN es:

> Build complex HTML or ???LaTeX??? tables using ???kable()??? from ???knitr??? and the piping syntax from ???magrittr???. Function ???kable()??? is a light weight table generator coming from ???knitr???. This package simplifies the way to manipulate the HTML or ???LaTeX??? codes generated by ???kable()??? and allows users to construct complex tables and customize styles using a readable syntax.

[Aqu??](https://cran.r-project.org/web/packages/kableExtra/vignettes/awesome_table_in_html.html) tienes la vignette para elaborar tablas para documentos html.

Para mejorar las tablas usaremos la funci??n `kableExtra::kable_styling()`:

``` r
knitr::kable(df_tt_12) %>% 
  kableExtra::kable_styling(bootstrap_options = c("striped", "hover"))
```

<table class="table table-striped table-hover" style="margin-left: auto; margin-right: auto;">
<thead>
<tr>
<th style="text-align:left;">
Country
</th>
<th style="text-align:right;">
Primaria
</th>
<th style="text-align:right;">
Secundaria
</th>
<th style="text-align:right;">
Secundaria_post
</th>
<th style="text-align:right;">
Terciaria
</th>
<th style="text-align:right;">
NA
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
ESP
</td>
<td style="text-align:right;">
213.0135
</td>
<td style="text-align:right;">
245.1109
</td>
<td style="text-align:right;">
265.7699
</td>
<td style="text-align:right;">
282.1070
</td>
<td style="text-align:right;">
NA
</td>
</tr>
<tr>
<td style="text-align:left;">
FRA
</td>
<td style="text-align:right;">
184.9306
</td>
<td style="text-align:right;">
246.6609
</td>
<td style="text-align:right;">
289.0088
</td>
<td style="text-align:right;">
304.0075
</td>
<td style="text-align:right;">
197.6502
</td>
</tr>
<tr>
<td style="text-align:left;">
GBR
</td>
<td style="text-align:right;">
207.3143
</td>
<td style="text-align:right;">
252.9237
</td>
<td style="text-align:right;">
263.2052
</td>
<td style="text-align:right;">
286.1454
</td>
<td style="text-align:right;">
213.1912
</td>
</tr>
<tr>
<td style="text-align:left;">
ITA
</td>
<td style="text-align:right;">
200.7297
</td>
<td style="text-align:right;">
257.5339
</td>
<td style="text-align:right;">
271.6400
</td>
<td style="text-align:right;">
279.7166
</td>
<td style="text-align:right;">
NA
</td>
</tr>
</tbody>
</table>

Se le puede poner un scroll:

``` r
df_tt_12 %>%
  knitr::kable() %>%
  kableExtra::kable_styling(font_size = 11) %>%
  kableExtra::scroll_box(width = "50%", height = "60%")
```

<div style="border: 1px solid #ddd; padding: 0px; overflow-y: scroll; height:60%; overflow-x: scroll; width:50%; ">

<table class="table" style="font-size: 11px; margin-left: auto; margin-right: auto;">
<thead>
<tr>
<th style="text-align:left;position: sticky; top:0; background-color: #FFFFFF;">
Country
</th>
<th style="text-align:right;position: sticky; top:0; background-color: #FFFFFF;">
Primaria
</th>
<th style="text-align:right;position: sticky; top:0; background-color: #FFFFFF;">
Secundaria
</th>
<th style="text-align:right;position: sticky; top:0; background-color: #FFFFFF;">
Secundaria_post
</th>
<th style="text-align:right;position: sticky; top:0; background-color: #FFFFFF;">
Terciaria
</th>
<th style="text-align:right;position: sticky; top:0; background-color: #FFFFFF;">
NA
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
ESP
</td>
<td style="text-align:right;">
213.0135
</td>
<td style="text-align:right;">
245.1109
</td>
<td style="text-align:right;">
265.7699
</td>
<td style="text-align:right;">
282.1070
</td>
<td style="text-align:right;">
NA
</td>
</tr>
<tr>
<td style="text-align:left;">
FRA
</td>
<td style="text-align:right;">
184.9306
</td>
<td style="text-align:right;">
246.6609
</td>
<td style="text-align:right;">
289.0088
</td>
<td style="text-align:right;">
304.0075
</td>
<td style="text-align:right;">
197.6502
</td>
</tr>
<tr>
<td style="text-align:left;">
GBR
</td>
<td style="text-align:right;">
207.3143
</td>
<td style="text-align:right;">
252.9237
</td>
<td style="text-align:right;">
263.2052
</td>
<td style="text-align:right;">
286.1454
</td>
<td style="text-align:right;">
213.1912
</td>
</tr>
<tr>
<td style="text-align:left;">
ITA
</td>
<td style="text-align:right;">
200.7297
</td>
<td style="text-align:right;">
257.5339
</td>
<td style="text-align:right;">
271.6400
</td>
<td style="text-align:right;">
279.7166
</td>
<td style="text-align:right;">
NA
</td>
</tr>
</tbody>
</table>

</div>

<br>

Se puede incluso poner las tablas junto con el texto.

``` r
knitr::kable(df_tt_12) %>% 
  kableExtra::kable_styling(bootstrap_options = "striped", 
                            full_width = F, 
                            position = "float_right")
```

<table class="table table-striped" style="width: auto !important; float: right; margin-left: 10px;">
<thead>
<tr>
<th style="text-align:left;">
Country
</th>
<th style="text-align:right;">
Primaria
</th>
<th style="text-align:right;">
Secundaria
</th>
<th style="text-align:right;">
Secundaria_post
</th>
<th style="text-align:right;">
Terciaria
</th>
<th style="text-align:right;">
NA
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
ESP
</td>
<td style="text-align:right;">
213.0135
</td>
<td style="text-align:right;">
245.1109
</td>
<td style="text-align:right;">
265.7699
</td>
<td style="text-align:right;">
282.1070
</td>
<td style="text-align:right;">
NA
</td>
</tr>
<tr>
<td style="text-align:left;">
FRA
</td>
<td style="text-align:right;">
184.9306
</td>
<td style="text-align:right;">
246.6609
</td>
<td style="text-align:right;">
289.0088
</td>
<td style="text-align:right;">
304.0075
</td>
<td style="text-align:right;">
197.6502
</td>
</tr>
<tr>
<td style="text-align:left;">
GBR
</td>
<td style="text-align:right;">
207.3143
</td>
<td style="text-align:right;">
252.9237
</td>
<td style="text-align:right;">
263.2052
</td>
<td style="text-align:right;">
286.1454
</td>
<td style="text-align:right;">
213.1912
</td>
</tr>
<tr>
<td style="text-align:left;">
ITA
</td>
<td style="text-align:right;">
200.7297
</td>
<td style="text-align:right;">
257.5339
</td>
<td style="text-align:right;">
271.6400
</td>
<td style="text-align:right;">
279.7166
</td>
<td style="text-align:right;">
NA
</td>
</tr>
</tbody>
</table>

<br><br>

Para ello tienes que usar la opci??n `position = "float_right` dentro de `kableExtra::kable_styling()`.

<br><br><br>

Si tenemos una tabla muy larga, podemos fijar el encabezamiento de la tabla con `fixed_thead`

``` r
knitr::kable(df_tt_12) %>%
  kableExtra::kable_styling(fixed_thead = list(enabled = T, 
                                               background = "lightblue"))
```

<table class="table" style="margin-left: auto; margin-right: auto;">
<thead>
<tr>
<th style="text-align:left;position: sticky; top:0; background-color: lightblue;">
Country
</th>
<th style="text-align:right;position: sticky; top:0; background-color: lightblue;">
Primaria
</th>
<th style="text-align:right;position: sticky; top:0; background-color: lightblue;">
Secundaria
</th>
<th style="text-align:right;position: sticky; top:0; background-color: lightblue;">
Secundaria_post
</th>
<th style="text-align:right;position: sticky; top:0; background-color: lightblue;">
Terciaria
</th>
<th style="text-align:right;position: sticky; top:0; background-color: lightblue;">
NA
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
ESP
</td>
<td style="text-align:right;">
213.0135
</td>
<td style="text-align:right;">
245.1109
</td>
<td style="text-align:right;">
265.7699
</td>
<td style="text-align:right;">
282.1070
</td>
<td style="text-align:right;">
NA
</td>
</tr>
<tr>
<td style="text-align:left;">
FRA
</td>
<td style="text-align:right;">
184.9306
</td>
<td style="text-align:right;">
246.6609
</td>
<td style="text-align:right;">
289.0088
</td>
<td style="text-align:right;">
304.0075
</td>
<td style="text-align:right;">
197.6502
</td>
</tr>
<tr>
<td style="text-align:left;">
GBR
</td>
<td style="text-align:right;">
207.3143
</td>
<td style="text-align:right;">
252.9237
</td>
<td style="text-align:right;">
263.2052
</td>
<td style="text-align:right;">
286.1454
</td>
<td style="text-align:right;">
213.1912
</td>
</tr>
<tr>
<td style="text-align:left;">
ITA
</td>
<td style="text-align:right;">
200.7297
</td>
<td style="text-align:right;">
257.5339
</td>
<td style="text-align:right;">
271.6400
</td>
<td style="text-align:right;">
279.7166
</td>
<td style="text-align:right;">
NA
</td>
</tr>
</tbody>
</table>

Se pueden formatear columnas por separado con `kableExtra::column_spec()`, o las filas con `kableExtra::row_spec()`. La tabla no nos saldr?? muy chula pero nos sirve para ver las posibilidades de `kable_styling()`.

``` r
library(kableExtra)
knitr::kable(df_tt_12) %>%
  kableExtra::kable_styling(full_width = F) %>%
  column_spec(1, bold = T, border_right = T) %>%
  column_spec(3, width = "20em", background = "yellow") %>% 
  row_spec(3:4, bold = T, color = "white", background = "#D7261E") %>% 
  row_spec(0, angle = 10)
```

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
<thead>
<tr>
<th style="text-align:left;-webkit-transform: rotate(10deg); -moz-transform: rotate(10deg); -ms-transform: rotate(10deg); -o-transform: rotate(10deg); transform: rotate(10deg);">
Country
</th>
<th style="text-align:right;-webkit-transform: rotate(10deg); -moz-transform: rotate(10deg); -ms-transform: rotate(10deg); -o-transform: rotate(10deg); transform: rotate(10deg);">
Primaria
</th>
<th style="text-align:right;-webkit-transform: rotate(10deg); -moz-transform: rotate(10deg); -ms-transform: rotate(10deg); -o-transform: rotate(10deg); transform: rotate(10deg);">
Secundaria
</th>
<th style="text-align:right;-webkit-transform: rotate(10deg); -moz-transform: rotate(10deg); -ms-transform: rotate(10deg); -o-transform: rotate(10deg); transform: rotate(10deg);">
Secundaria_post
</th>
<th style="text-align:right;-webkit-transform: rotate(10deg); -moz-transform: rotate(10deg); -ms-transform: rotate(10deg); -o-transform: rotate(10deg); transform: rotate(10deg);">
Terciaria
</th>
<th style="text-align:right;-webkit-transform: rotate(10deg); -moz-transform: rotate(10deg); -ms-transform: rotate(10deg); -o-transform: rotate(10deg); transform: rotate(10deg);">
NA
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;font-weight: bold;border-right:1px solid;">
ESP
</td>
<td style="text-align:right;">
213.0135
</td>
<td style="text-align:right;width: 20em; background-color: yellow !important;">
245.1109
</td>
<td style="text-align:right;">
265.7699
</td>
<td style="text-align:right;">
282.1070
</td>
<td style="text-align:right;">
NA
</td>
</tr>
<tr>
<td style="text-align:left;font-weight: bold;border-right:1px solid;">
FRA
</td>
<td style="text-align:right;">
184.9306
</td>
<td style="text-align:right;width: 20em; background-color: yellow !important;">
246.6609
</td>
<td style="text-align:right;">
289.0088
</td>
<td style="text-align:right;">
304.0075
</td>
<td style="text-align:right;">
197.6502
</td>
</tr>
<tr>
<td style="text-align:left;font-weight: bold;border-right:1px solid;font-weight: bold;color: white !important;background-color: #D7261E !important;">
GBR
</td>
<td style="text-align:right;font-weight: bold;color: white !important;background-color: #D7261E !important;">
207.3143
</td>
<td style="text-align:right;width: 20em; background-color: yellow !important;font-weight: bold;color: white !important;background-color: #D7261E !important;">
252.9237
</td>
<td style="text-align:right;font-weight: bold;color: white !important;background-color: #D7261E !important;">
263.2052
</td>
<td style="text-align:right;font-weight: bold;color: white !important;background-color: #D7261E !important;">
286.1454
</td>
<td style="text-align:right;font-weight: bold;color: white !important;background-color: #D7261E !important;">
213.1912
</td>
</tr>
<tr>
<td style="text-align:left;font-weight: bold;border-right:1px solid;font-weight: bold;color: white !important;background-color: #D7261E !important;">
ITA
</td>
<td style="text-align:right;font-weight: bold;color: white !important;background-color: #D7261E !important;">
200.7297
</td>
<td style="text-align:right;width: 20em; background-color: yellow !important;font-weight: bold;color: white !important;background-color: #D7261E !important;">
257.5339
</td>
<td style="text-align:right;font-weight: bold;color: white !important;background-color: #D7261E !important;">
271.6400
</td>
<td style="text-align:right;font-weight: bold;color: white !important;background-color: #D7261E !important;">
279.7166
</td>
<td style="text-align:right;font-weight: bold;color: white !important;background-color: #D7261E !important;">
NA
</td>
</tr>
</tbody>
</table>

Puedes ver las posibilidades de este pkg en su [vignette](https://cran.r-project.org/web/packages/kableExtra/vignettes/awesome_table_in_html.html). Fijate que tabla m??s chula hay all??:

``` r
mtcars[1:8, 1:8] %>%
  kbl() %>%
  kable_paper(full_width = F) %>%
  column_spec(2, color = spec_color(mtcars$mpg[1:8]),
              link = "https://haozhu233.github.io/kableExtra/") %>%
  column_spec(6, color = "white",
              background = spec_color(mtcars$drat[1:8], end = 0.7),
              popover = paste("am:", mtcars$am[1:8]))
```

<table class=" lightable-paper" style="font-family: &quot;Arial Narrow&quot;, arial, helvetica, sans-serif; width: auto !important; margin-left: auto; margin-right: auto;">
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:right;">
mpg
</th>
<th style="text-align:right;">
cyl
</th>
<th style="text-align:right;">
disp
</th>
<th style="text-align:right;">
hp
</th>
<th style="text-align:right;">
drat
</th>
<th style="text-align:right;">
wt
</th>
<th style="text-align:right;">
qsec
</th>
<th style="text-align:right;">
vs
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
Mazda RX4
</td>
<td style="text-align:right;color: rgba(52, 182, 121, 1) !important;">
<a href="https://haozhu233.github.io/kableExtra/" style="color: rgba(52, 182, 121, 1) !important;"> 21.0 </a>
</td>
<td style="text-align:right;">
6
</td>
<td style="text-align:right;">
160.0
</td>
<td style="text-align:right;">
110
</td>
<td style="text-align:right;color: white !important;background-color: rgba(67, 191, 113, 1) !important;" data-toggle="popover" data-container="body" data-trigger="hover" data-placement="right" data-content="am: 1">
3.90
</td>
<td style="text-align:right;">
2.620
</td>
<td style="text-align:right;">
16.46
</td>
<td style="text-align:right;">
0
</td>
</tr>
<tr>
<td style="text-align:left;">
Mazda RX4 Wag
</td>
<td style="text-align:right;color: rgba(52, 182, 121, 1) !important;">
<a href="https://haozhu233.github.io/kableExtra/" style="color: rgba(52, 182, 121, 1) !important;"> 21.0 </a>
</td>
<td style="text-align:right;">
6
</td>
<td style="text-align:right;">
160.0
</td>
<td style="text-align:right;">
110
</td>
<td style="text-align:right;color: white !important;background-color: rgba(67, 191, 113, 1) !important;" data-toggle="popover" data-container="body" data-trigger="hover" data-placement="right" data-content="am: 1">
3.90
</td>
<td style="text-align:right;">
2.875
</td>
<td style="text-align:right;">
17.02
</td>
<td style="text-align:right;">
0
</td>
</tr>
<tr>
<td style="text-align:left;">
Datsun 710
</td>
<td style="text-align:right;color: rgba(149, 216, 64, 1) !important;">
<a href="https://haozhu233.github.io/kableExtra/" style="color: rgba(149, 216, 64, 1) !important;"> 22.8 </a>
</td>
<td style="text-align:right;">
4
</td>
<td style="text-align:right;">
108.0
</td>
<td style="text-align:right;">
93
</td>
<td style="text-align:right;color: white !important;background-color: rgba(55, 184, 120, 1) !important;" data-toggle="popover" data-container="body" data-trigger="hover" data-placement="right" data-content="am: 1">
3.85
</td>
<td style="text-align:right;">
2.320
</td>
<td style="text-align:right;">
18.61
</td>
<td style="text-align:right;">
1
</td>
</tr>
<tr>
<td style="text-align:left;">
Hornet 4 Drive
</td>
<td style="text-align:right;color: rgba(68, 191, 112, 1) !important;">
<a href="https://haozhu233.github.io/kableExtra/" style="color: rgba(68, 191, 112, 1) !important;"> 21.4 </a>
</td>
<td style="text-align:right;">
6
</td>
<td style="text-align:right;">
258.0
</td>
<td style="text-align:right;">
110
</td>
<td style="text-align:right;color: white !important;background-color: rgba(65, 67, 135, 1) !important;" data-toggle="popover" data-container="body" data-trigger="hover" data-placement="right" data-content="am: 0">
3.08
</td>
<td style="text-align:right;">
3.215
</td>
<td style="text-align:right;">
19.44
</td>
<td style="text-align:right;">
1
</td>
</tr>
<tr>
<td style="text-align:left;">
Hornet Sportabout
</td>
<td style="text-align:right;color: rgba(38, 129, 142, 1) !important;">
<a href="https://haozhu233.github.io/kableExtra/" style="color: rgba(38, 129, 142, 1) !important;"> 18.7 </a>
</td>
<td style="text-align:right;">
8
</td>
<td style="text-align:right;">
360.0
</td>
<td style="text-align:right;">
175
</td>
<td style="text-align:right;color: white !important;background-color: rgba(60, 79, 138, 1) !important;" data-toggle="popover" data-container="body" data-trigger="hover" data-placement="right" data-content="am: 0">
3.15
</td>
<td style="text-align:right;">
3.440
</td>
<td style="text-align:right;">
17.02
</td>
<td style="text-align:right;">
0
</td>
</tr>
<tr>
<td style="text-align:left;">
Valiant
</td>
<td style="text-align:right;color: rgba(44, 114, 142, 1) !important;">
<a href="https://haozhu233.github.io/kableExtra/" style="color: rgba(44, 114, 142, 1) !important;"> 18.1 </a>
</td>
<td style="text-align:right;">
6
</td>
<td style="text-align:right;">
225.0
</td>
<td style="text-align:right;">
105
</td>
<td style="text-align:right;color: white !important;background-color: rgba(68, 1, 84, 1) !important;" data-toggle="popover" data-container="body" data-trigger="hover" data-placement="right" data-content="am: 0">
2.76
</td>
<td style="text-align:right;">
3.460
</td>
<td style="text-align:right;">
20.22
</td>
<td style="text-align:right;">
1
</td>
</tr>
<tr>
<td style="text-align:left;">
Duster 360
</td>
<td style="text-align:right;color: rgba(68, 1, 84, 1) !important;">
<a href="https://haozhu233.github.io/kableExtra/" style="color: rgba(68, 1, 84, 1) !important;"> 14.3 </a>
</td>
<td style="text-align:right;">
8
</td>
<td style="text-align:right;">
360.0
</td>
<td style="text-align:right;">
245
</td>
<td style="text-align:right;color: white !important;background-color: rgba(55, 90, 140, 1) !important;" data-toggle="popover" data-container="body" data-trigger="hover" data-placement="right" data-content="am: 0">
3.21
</td>
<td style="text-align:right;">
3.570
</td>
<td style="text-align:right;">
15.84
</td>
<td style="text-align:right;">
0
</td>
</tr>
<tr>
<td style="text-align:left;">
Merc 240D
</td>
<td style="text-align:right;color: rgba(253, 231, 37, 1) !important;">
<a href="https://haozhu233.github.io/kableExtra/" style="color: rgba(253, 231, 37, 1) !important;"> 24.4 </a>
</td>
<td style="text-align:right;">
4
</td>
<td style="text-align:right;">
146.7
</td>
<td style="text-align:right;">
62
</td>
<td style="text-align:right;color: white !important;background-color: rgba(31, 161, 135, 1) !important;" data-toggle="popover" data-container="body" data-trigger="hover" data-placement="right" data-content="am: 0">
3.69
</td>
<td style="text-align:right;">
3.190
</td>
<td style="text-align:right;">
20.00
</td>
<td style="text-align:right;">
1
</td>
</tr>
</tbody>
</table>

<br>

------------------------------------------------------------------------

<br>

# 4. Otros paquetes para tablas

Uno de los paquetes que se pueden usar para generar tablas es [`pander`](http://rapporter.github.io/pander/), pero no lo incluyo en el tutorial porque en realidad, su objetivo es m??s general, su objetivo es facilitar la exportaci??n de objetos R a `pandoc`. De hecho, `pander` puede ser una alternativa a `knitr`; de hecho, el t??tulo de su pagina web es: `pander: An R Pandoc Writer`.

Si presento, de forma sencilla los paquetes `formatable` y dos paquetes muy prometedores como `flextable` y `gt`, pero existen m??s posibilidades, m??s paquetes para hacer tablas en R.

------------------------------------------------------------------------

<br>

## 4.1 `formatable` pkg

El paquete [`formattable`](https://github.com/renkun-ken/formattable)

> is designed for applying formatting on vectors and data frames to make data presentation easier, richer, more flexible and hopefully convey more information.

En estos dos post: [aqu??](https://www.displayr.com/formattable/?utm_medium=Feed&utm_source=Syndication) y [aqu??](https://www.littlemissdata.com/blog/prettytables) explican con detalle las posibilidades del paquete `formattable.`

Para ilustrar las posibilidades de `formattable` utilizo uno de los ejemplos de su [p??gina web](https://renkun-ken.github.io/formattable/):

``` r
library(formattable)
df %>% formattable(list(
  age = color_tile("white", "orange"),
  grade = formatter("span", style = x ~ ifelse(x == "A", 
    style(color = "green", font.weight = "bold"), NA)),
  area(col = c(test1_score, test2_score)) ~ normalize_bar("pink", 0.2),
  final_score = formatter("span",
    style = x ~ style(color = ifelse(rank(-x) <= 3, "green", "gray")),
    x ~ sprintf("%.2f (rank: %02d)", x, rank(-x))),
  registered = formatter("span",
    style = x ~ style(color = ifelse(x, "green", "red")),
    x ~ icontext(ifelse(x, "ok", "remove"), ifelse(x, "Yes", "No")))
))
```

<table class="table table-condensed">
<thead>
<tr>
<th style="text-align:right;">
id
</th>
<th style="text-align:right;">
name
</th>
<th style="text-align:right;">
age
</th>
<th style="text-align:right;">
grade
</th>
<th style="text-align:right;">
test1_score
</th>
<th style="text-align:right;">
test2_score
</th>
<th style="text-align:right;">
final_score
</th>
<th style="text-align:right;">
registered
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
Bob
</td>
<td style="text-align:right;">
<span style="display: block; padding: 0 4px; border-radius: 4px; background-color: #ffe8bf">28</span>
</td>
<td style="text-align:right;">
C
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 42.86%">8.9</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 54.29%">9.1</span>
</td>
<td style="text-align:right;">
<span style="color: gray">9.00 (rank: 06)</span>
</td>
<td style="text-align:right;">
<span style="color: green">
<i class="glyphicon glyphicon-ok"></i>
Yes
</span>
</td>
</tr>
<tr>
<td style="text-align:right;">
2
</td>
<td style="text-align:right;">
Ashley
</td>
<td style="text-align:right;">
<span style="display: block; padding: 0 4px; border-radius: 4px; background-color: #ffffff">27</span>
</td>
<td style="text-align:right;">
<span style="color: green; font-weight: bold">A</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 77.14%">9.5</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 54.29%">9.1</span>
</td>
<td style="text-align:right;">
<span style="color: green">9.30 (rank: 03)</span>
</td>
<td style="text-align:right;">
<span style="color: red">
<i class="glyphicon glyphicon-remove"></i>
No
</span>
</td>
</tr>
<tr>
<td style="text-align:right;">
3
</td>
<td style="text-align:right;">
James
</td>
<td style="text-align:right;">
<span style="display: block; padding: 0 4px; border-radius: 4px; background-color: #ffbb3f">30</span>
</td>
<td style="text-align:right;">
<span style="color: green; font-weight: bold">A</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 82.86%">9.6</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 60.00%">9.2</span>
</td>
<td style="text-align:right;">
<span style="color: green">9.40 (rank: 02)</span>
</td>
<td style="text-align:right;">
<span style="color: green">
<i class="glyphicon glyphicon-ok"></i>
Yes
</span>
</td>
</tr>
<tr>
<td style="text-align:right;">
4
</td>
<td style="text-align:right;">
David
</td>
<td style="text-align:right;">
<span style="display: block; padding: 0 4px; border-radius: 4px; background-color: #ffe8bf">28</span>
</td>
<td style="text-align:right;">
C
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 42.86%">8.9</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 54.29%">9.1</span>
</td>
<td style="text-align:right;">
<span style="color: gray">9.00 (rank: 06)</span>
</td>
<td style="text-align:right;">
<span style="color: red">
<i class="glyphicon glyphicon-remove"></i>
No
</span>
</td>
</tr>
<tr>
<td style="text-align:right;">
5
</td>
<td style="text-align:right;">
Jenny
</td>
<td style="text-align:right;">
<span style="display: block; padding: 0 4px; border-radius: 4px; background-color: #ffd27f">29</span>
</td>
<td style="text-align:right;">
B
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 54.29%">9.1</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 42.86%">8.9</span>
</td>
<td style="text-align:right;">
<span style="color: gray">9.00 (rank: 06)</span>
</td>
<td style="text-align:right;">
<span style="color: green">
<i class="glyphicon glyphicon-ok"></i>
Yes
</span>
</td>
</tr>
<tr>
<td style="text-align:right;">
6
</td>
<td style="text-align:right;">
Hans
</td>
<td style="text-align:right;">
<span style="display: block; padding: 0 4px; border-radius: 4px; background-color: #ffd27f">29</span>
</td>
<td style="text-align:right;">
B
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 65.71%">9.3</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 20.00%">8.5</span>
</td>
<td style="text-align:right;">
<span style="color: gray">8.90 (rank: 08)</span>
</td>
<td style="text-align:right;">
<span style="color: green">
<i class="glyphicon glyphicon-ok"></i>
Yes
</span>
</td>
</tr>
<tr>
<td style="text-align:right;">
7
</td>
<td style="text-align:right;">
Leo
</td>
<td style="text-align:right;">
<span style="display: block; padding: 0 4px; border-radius: 4px; background-color: #ffffff">27</span>
</td>
<td style="text-align:right;">
B
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 65.71%">9.3</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 60.00%">9.2</span>
</td>
<td style="text-align:right;">
<span style="color: gray">9.25 (rank: 04)</span>
</td>
<td style="text-align:right;">
<span style="color: green">
<i class="glyphicon glyphicon-ok"></i>
Yes
</span>
</td>
</tr>
<tr>
<td style="text-align:right;">
8
</td>
<td style="text-align:right;">
John
</td>
<td style="text-align:right;">
<span style="display: block; padding: 0 4px; border-radius: 4px; background-color: #ffffff">27</span>
</td>
<td style="text-align:right;">
<span style="color: green; font-weight: bold">A</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 100.00%">9.9</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 65.71%">9.3</span>
</td>
<td style="text-align:right;">
<span style="color: green">9.60 (rank: 01)</span>
</td>
<td style="text-align:right;">
<span style="color: red">
<i class="glyphicon glyphicon-remove"></i>
No
</span>
</td>
</tr>
<tr>
<td style="text-align:right;">
9
</td>
<td style="text-align:right;">
Emily
</td>
<td style="text-align:right;">
<span style="display: block; padding: 0 4px; border-radius: 4px; background-color: #ffa500">31</span>
</td>
<td style="text-align:right;">
C
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 20.00%">8.5</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 54.29%">9.1</span>
</td>
<td style="text-align:right;">
<span style="color: gray">8.80 (rank: 09)</span>
</td>
<td style="text-align:right;">
<span style="color: red">
<i class="glyphicon glyphicon-remove"></i>
No
</span>
</td>
</tr>
<tr>
<td style="text-align:right;">
10
</td>
<td style="text-align:right;">
Lee
</td>
<td style="text-align:right;">
<span style="display: block; padding: 0 4px; border-radius: 4px; background-color: #ffbb3f">30</span>
</td>
<td style="text-align:right;">
C
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 25.71%">8.6</span>
</td>
<td style="text-align:right;">
<span style="display: inline-block; direction: rtl; unicode-bidi: plaintext; border-radius: 4px; padding-right: 2px; background-color: pink; width: 37.14%">8.8</span>
</td>
<td style="text-align:right;">
<span style="color: gray">8.70 (rank: 10)</span>
</td>
<td style="text-align:right;">
<span style="color: red">
<i class="glyphicon glyphicon-remove"></i>
No
</span>
</td>
</tr>
</tbody>
</table>

------------------------------------------------------------------------

<br>

## 4.2 `flextable` pkg

El paquete [`flextable`](https://davidgohel.github.io/flextable/articles/overview.html) es relativamente nuevo y tiene la ventaja de que provee un entorno para crear de forma relativamente sencilla tablas estad??sticas para informes. Una de sus ventajas es que puede generar tablas para documentos html, Word, Powerpoint y pdf. [Aqu??](https://ardata-fr.github.io/flextable-book/) tienes un bookdown sobre flextable.

Las tablas hechas con `flextable` pueden exportarse a :

- Documentos html, Word y PowerPoint hechos a trav??s de ficheros Rmarkdown  
- Documentos Word y Powerpoint hechos con el paquete [`officer`](https://davidgohel.github.io/officer/)
- Documentos pdf a trav??s del paquete [`pagedown`](https://github.com/rstudio/pagedown)  
- Adem??s las flextables pueden ser transformadas a gr??ficos R o como im??genes (png, pdf y jpeg).

Si quieres ver las posibilidades de este paquete tendr??s que ir a su [p??gina web](https://davidgohel.github.io/flextable/articles/overview.html). Como ejemplo:

``` r
library(flextable)

ft <- flextable::flextable(head(iris), col_keys = c("Sepal.Length", "Sepal.Width", "Petal.Length", "Petal.Width", "Species" ))

ft %>% autofit() %>%  align(align = "center", part = "all")
```

<template id="d1655575-fde9-4747-a108-e3f5a15dcd0e"><style>
.tabwid table{
  border-spacing:0px !important;
  border-collapse:collapse;
  line-height:1;
  margin-left:auto;
  margin-right:auto;
  border-width: 0;
  border-color: transparent;
  caption-side: top;
}
.tabwid-caption-bottom table{
  caption-side: bottom;
}
.tabwid_left table{
  margin-left:0;
}
.tabwid_right table{
  margin-right:0;
}
.tabwid td, .tabwid th {
    padding: 0;
}
.tabwid a {
  text-decoration: none;
}
.tabwid thead {
    background-color: transparent;
}
.tabwid tfoot {
    background-color: transparent;
}
.tabwid table tr {
background-color: transparent;
}
.katex-display {
    margin: 0 0 !important;
}
</style><div class="tabwid"><style>.cl-e6e84ffe{}.cl-e6e1f4f6{font-family:'DejaVu Sans';font-size:11pt;font-weight:normal;font-style:normal;text-decoration:none;color:rgba(0, 0, 0, 1.00);background-color:transparent;}.cl-e6e48a2c{margin:0;text-align:center;border-bottom: 0 solid rgba(0, 0, 0, 1.00);border-top: 0 solid rgba(0, 0, 0, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);padding-bottom:5pt;padding-top:5pt;padding-left:5pt;padding-right:5pt;line-height: 1;background-color:transparent;}.cl-e6e49b70{width:1.287in;background-color:transparent;vertical-align: middle;border-bottom: 2pt solid rgba(102, 102, 102, 1.00);border-top: 2pt solid rgba(102, 102, 102, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49b7a{width:1.205in;background-color:transparent;vertical-align: middle;border-bottom: 2pt solid rgba(102, 102, 102, 1.00);border-top: 2pt solid rgba(102, 102, 102, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49b7b{width:1.245in;background-color:transparent;vertical-align: middle;border-bottom: 2pt solid rgba(102, 102, 102, 1.00);border-top: 2pt solid rgba(102, 102, 102, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49b84{width:1.163in;background-color:transparent;vertical-align: middle;border-bottom: 2pt solid rgba(102, 102, 102, 1.00);border-top: 2pt solid rgba(102, 102, 102, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49b85{width:0.873in;background-color:transparent;vertical-align: middle;border-bottom: 2pt solid rgba(102, 102, 102, 1.00);border-top: 2pt solid rgba(102, 102, 102, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49b86{width:1.287in;background-color:transparent;vertical-align: middle;border-bottom: 0 solid rgba(0, 0, 0, 1.00);border-top: 0 solid rgba(0, 0, 0, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49b8e{width:1.205in;background-color:transparent;vertical-align: middle;border-bottom: 0 solid rgba(0, 0, 0, 1.00);border-top: 0 solid rgba(0, 0, 0, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49b98{width:1.245in;background-color:transparent;vertical-align: middle;border-bottom: 0 solid rgba(0, 0, 0, 1.00);border-top: 0 solid rgba(0, 0, 0, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49b99{width:1.163in;background-color:transparent;vertical-align: middle;border-bottom: 0 solid rgba(0, 0, 0, 1.00);border-top: 0 solid rgba(0, 0, 0, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49b9a{width:0.873in;background-color:transparent;vertical-align: middle;border-bottom: 0 solid rgba(0, 0, 0, 1.00);border-top: 0 solid rgba(0, 0, 0, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49ba2{width:1.287in;background-color:transparent;vertical-align: middle;border-bottom: 2pt solid rgba(102, 102, 102, 1.00);border-top: 0 solid rgba(0, 0, 0, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49ba3{width:1.205in;background-color:transparent;vertical-align: middle;border-bottom: 2pt solid rgba(102, 102, 102, 1.00);border-top: 0 solid rgba(0, 0, 0, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49bac{width:1.245in;background-color:transparent;vertical-align: middle;border-bottom: 2pt solid rgba(102, 102, 102, 1.00);border-top: 0 solid rgba(0, 0, 0, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49bad{width:1.163in;background-color:transparent;vertical-align: middle;border-bottom: 2pt solid rgba(102, 102, 102, 1.00);border-top: 0 solid rgba(0, 0, 0, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}.cl-e6e49bae{width:0.873in;background-color:transparent;vertical-align: middle;border-bottom: 2pt solid rgba(102, 102, 102, 1.00);border-top: 0 solid rgba(0, 0, 0, 1.00);border-left: 0 solid rgba(0, 0, 0, 1.00);border-right: 0 solid rgba(0, 0, 0, 1.00);margin-bottom:0;margin-top:0;margin-left:0;margin-right:0;}</style><table class='cl-e6e84ffe'><thead><tr style="overflow-wrap:break-word;"><th class="cl-e6e49b70"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">Sepal.Length</span></p></th><th class="cl-e6e49b7a"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">Sepal.Width</span></p></th><th class="cl-e6e49b7b"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">Petal.Length</span></p></th><th class="cl-e6e49b84"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">Petal.Width</span></p></th><th class="cl-e6e49b85"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">Species</span></p></th></tr></thead><tbody><tr style="overflow-wrap:break-word;"><td class="cl-e6e49b86"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">5.1</span></p></td><td class="cl-e6e49b8e"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">3.5</span></p></td><td class="cl-e6e49b98"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">1.4</span></p></td><td class="cl-e6e49b99"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">0.2</span></p></td><td class="cl-e6e49b9a"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">setosa</span></p></td></tr><tr style="overflow-wrap:break-word;"><td class="cl-e6e49b86"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">4.9</span></p></td><td class="cl-e6e49b8e"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">3.0</span></p></td><td class="cl-e6e49b98"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">1.4</span></p></td><td class="cl-e6e49b99"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">0.2</span></p></td><td class="cl-e6e49b9a"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">setosa</span></p></td></tr><tr style="overflow-wrap:break-word;"><td class="cl-e6e49b86"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">4.7</span></p></td><td class="cl-e6e49b8e"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">3.2</span></p></td><td class="cl-e6e49b98"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">1.3</span></p></td><td class="cl-e6e49b99"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">0.2</span></p></td><td class="cl-e6e49b9a"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">setosa</span></p></td></tr><tr style="overflow-wrap:break-word;"><td class="cl-e6e49b86"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">4.6</span></p></td><td class="cl-e6e49b8e"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">3.1</span></p></td><td class="cl-e6e49b98"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">1.5</span></p></td><td class="cl-e6e49b99"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">0.2</span></p></td><td class="cl-e6e49b9a"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">setosa</span></p></td></tr><tr style="overflow-wrap:break-word;"><td class="cl-e6e49b86"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">5.0</span></p></td><td class="cl-e6e49b8e"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">3.6</span></p></td><td class="cl-e6e49b98"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">1.4</span></p></td><td class="cl-e6e49b99"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">0.2</span></p></td><td class="cl-e6e49b9a"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">setosa</span></p></td></tr><tr style="overflow-wrap:break-word;"><td class="cl-e6e49ba2"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">5.4</span></p></td><td class="cl-e6e49ba3"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">3.9</span></p></td><td class="cl-e6e49bac"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">1.7</span></p></td><td class="cl-e6e49bad"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">0.4</span></p></td><td class="cl-e6e49bae"><p class="cl-e6e48a2c"><span class="cl-e6e1f4f6">setosa</span></p></td></tr></tbody></table></div></template>
<div class="flextable-shadow-host" id="9c94771d-d326-4ad3-81b0-627e7cd5cb49"></div>
<script>
var dest = document.getElementById("9c94771d-d326-4ad3-81b0-627e7cd5cb49");
var template = document.getElementById("d1655575-fde9-4747-a108-e3f5a15dcd0e");
var fantome = dest.attachShadow({mode: 'open'});
var templateContent = template.content;
fantome.appendChild(templateContent);
</script>

------------------------------------------------------------------------

<br>

## 4.3 `gt` package

El paquete `gt` tambi??n es relativamente nuevo pero creo que se est?? convirtiendo en el paquete de referencia para hacer tablas en R. Su p??gina web est?? [aqu??](https://gt.rstudio.com/). Hay que entender un poco su terminolog??a, pero una vez lo haces, hacer tablas con `gt` es muy sencillo.

Podemos empezar con una web con [algunos ejemplos](https://frm1789.github.io/gt_examples/index.html) de tablas hechas con `gt` o ir a su [p??gina web](https://gt.rstudio.com/) o a su [vignette introductoria](https://gt.rstudio.com/articles/intro-creating-gt-tables.html), o a [este post](https://blog.rstudio.com/2020/04/08/great-looking-tables-gt-0-2/) donde se anuncia la aparici??n de `gt(v0.2)`.

Por su parte, [Thomas Mock](https://twitter.com/thomas_mock?lang=es) ha realizado una serie de fant??sticos post y presentaciones acerca del paquete `gt`; por ejemplo: [Beautiful tables in R](https://themockup.blog/static/slides/intro-tables.html#1), [10+ Guidelines for Better Tables in R](https://themockup.blog/posts/2020-09-04-10-table-rules-in-r/), [Functions and Themes for gt tables](https://themockup.blog/posts/2020-09-26-functions-and-themes-for-gt-tables/), [Embedding custom HTML in gt tables](https://themockup.blog/posts/2020-10-31-embedding-custom-features-in-gt-tables/) y [gt - a (G)rammar of (T)ables](https://themockup.blog/posts/2020-05-16-gt-a-grammer-of-tables/).

Si quieres ver el material de un tutorial de `gt` dise??ado por su desarrollador, [Richard Iannone](https://github.com/rich-iannone), puedes encontrarlo en [este repo](https://github.com/rich-iannone/gt-workshop-2020).

Hacer una tabla b??sica con `gt` es tan f??cil como hacer `gt(my_df)`. Ve??moslo:

``` r
library(gt) #-remotes::install_github("rstudio/gt")
df_tt_4 %>% gt()
```

<div id="wqoqqillrp" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#wqoqqillrp .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#wqoqqillrp .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#wqoqqillrp .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#wqoqqillrp .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#wqoqqillrp .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#wqoqqillrp .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#wqoqqillrp .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#wqoqqillrp .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#wqoqqillrp .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#wqoqqillrp .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#wqoqqillrp .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#wqoqqillrp .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#wqoqqillrp .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#wqoqqillrp .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#wqoqqillrp .gt_from_md > :first-child {
  margin-top: 0;
}

#wqoqqillrp .gt_from_md > :last-child {
  margin-bottom: 0;
}

#wqoqqillrp .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#wqoqqillrp .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#wqoqqillrp .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#wqoqqillrp .gt_row_group_first td {
  border-top-width: 2px;
}

#wqoqqillrp .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#wqoqqillrp .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#wqoqqillrp .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#wqoqqillrp .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#wqoqqillrp .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#wqoqqillrp .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#wqoqqillrp .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#wqoqqillrp .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#wqoqqillrp .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#wqoqqillrp .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-left: 4px;
  padding-right: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#wqoqqillrp .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#wqoqqillrp .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#wqoqqillrp .gt_left {
  text-align: left;
}

#wqoqqillrp .gt_center {
  text-align: center;
}

#wqoqqillrp .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#wqoqqillrp .gt_font_normal {
  font-weight: normal;
}

#wqoqqillrp .gt_font_bold {
  font-weight: bold;
}

#wqoqqillrp .gt_font_italic {
  font-style: italic;
}

#wqoqqillrp .gt_super {
  font-size: 65%;
}

#wqoqqillrp .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 75%;
  vertical-align: 0.4em;
}

#wqoqqillrp .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#wqoqqillrp .gt_indent_1 {
  text-indent: 5px;
}

#wqoqqillrp .gt_indent_2 {
  text-indent: 10px;
}

#wqoqqillrp .gt_indent_3 {
  text-indent: 15px;
}

#wqoqqillrp .gt_indent_4 {
  text-indent: 20px;
}

#wqoqqillrp .gt_indent_5 {
  text-indent: 25px;
}
</style>
<table class="gt_table">
  
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="Gender">Gender</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Primary">Primary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Secondary">Secondary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Tertiary">Tertiary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Upper_second">Upper_second</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="NA">NA</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="Gender" class="gt_row gt_left">Female</td>
<td headers="Primary" class="gt_row gt_right">0.4377224</td>
<td headers="Secondary" class="gt_row gt_right">0.4804831</td>
<td headers="Tertiary" class="gt_row gt_right">0.6159875</td>
<td headers="Upper_second" class="gt_row gt_right">0.579646</td>
<td headers="NA" class="gt_row gt_right">0.8</td></tr>
    <tr><td headers="Gender" class="gt_row gt_left">Male</td>
<td headers="Primary" class="gt_row gt_right">0.5622776</td>
<td headers="Secondary" class="gt_row gt_right">0.5195169</td>
<td headers="Tertiary" class="gt_row gt_right">0.3840125</td>
<td headers="Upper_second" class="gt_row gt_right">0.420354</td>
<td headers="NA" class="gt_row gt_right">0.2</td></tr>
  </tbody>
  
  
</table>
</div>

<br>

Nos queda arreglar/tunear/a??adir elementos a nuestra tabla. Para ello, lo primero es conocer como se llaman los distintos elementos de una tabla hecha con `gt`:

<br>

La tabla que hemos hecho antes con `gt`, es una tabla muy b??sica, s??lo tiene dos elementos: the ???Column Labels??? y the ???Table Body??? (que es donde est??n los valores). Vamos a a??adir m??s elementos a nuestra tabla:

- A??adimos una parte m??s, ???Table header???, con la funci??n `tab_header()`. Con ella podemos a??adir un t??tulo y subtitulo a la tabla. Adem??s podemos dar formato al t??tulo, **usando markdown!!**, con la funci??n `md()`

``` r
gt_tbl <- df_tt_4 %>% gt()

gt_tbl <- gt_tbl %>% tab_header(title = md("**Genero y nivel educativo**"),
                      subtitle = md("Porcentaje de *H y M* en cada nivel educativo"))
gt_tbl
```

<div id="famtnhzvde" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#famtnhzvde .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#famtnhzvde .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#famtnhzvde .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#famtnhzvde .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#famtnhzvde .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#famtnhzvde .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#famtnhzvde .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#famtnhzvde .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#famtnhzvde .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#famtnhzvde .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#famtnhzvde .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#famtnhzvde .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#famtnhzvde .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#famtnhzvde .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#famtnhzvde .gt_from_md > :first-child {
  margin-top: 0;
}

#famtnhzvde .gt_from_md > :last-child {
  margin-bottom: 0;
}

#famtnhzvde .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#famtnhzvde .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#famtnhzvde .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#famtnhzvde .gt_row_group_first td {
  border-top-width: 2px;
}

#famtnhzvde .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#famtnhzvde .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#famtnhzvde .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#famtnhzvde .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#famtnhzvde .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#famtnhzvde .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#famtnhzvde .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#famtnhzvde .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#famtnhzvde .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#famtnhzvde .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-left: 4px;
  padding-right: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#famtnhzvde .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#famtnhzvde .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#famtnhzvde .gt_left {
  text-align: left;
}

#famtnhzvde .gt_center {
  text-align: center;
}

#famtnhzvde .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#famtnhzvde .gt_font_normal {
  font-weight: normal;
}

#famtnhzvde .gt_font_bold {
  font-weight: bold;
}

#famtnhzvde .gt_font_italic {
  font-style: italic;
}

#famtnhzvde .gt_super {
  font-size: 65%;
}

#famtnhzvde .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 75%;
  vertical-align: 0.4em;
}

#famtnhzvde .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#famtnhzvde .gt_indent_1 {
  text-indent: 5px;
}

#famtnhzvde .gt_indent_2 {
  text-indent: 10px;
}

#famtnhzvde .gt_indent_3 {
  text-indent: 15px;
}

#famtnhzvde .gt_indent_4 {
  text-indent: 20px;
}

#famtnhzvde .gt_indent_5 {
  text-indent: 25px;
}
</style>
<table class="gt_table">
  <thead class="gt_header">
    <tr>
      <td colspan="6" class="gt_heading gt_title gt_font_normal" style><strong>Genero y nivel educativo</strong></td>
    </tr>
    <tr>
      <td colspan="6" class="gt_heading gt_subtitle gt_font_normal gt_bottom_border" style>Porcentaje de <em>H y M</em> en cada nivel educativo</td>
    </tr>
  </thead>
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="Gender">Gender</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Primary">Primary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Secondary">Secondary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Tertiary">Tertiary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Upper_second">Upper_second</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="NA">NA</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="Gender" class="gt_row gt_left">Female</td>
<td headers="Primary" class="gt_row gt_right">0.4377224</td>
<td headers="Secondary" class="gt_row gt_right">0.4804831</td>
<td headers="Tertiary" class="gt_row gt_right">0.6159875</td>
<td headers="Upper_second" class="gt_row gt_right">0.579646</td>
<td headers="NA" class="gt_row gt_right">0.8</td></tr>
    <tr><td headers="Gender" class="gt_row gt_left">Male</td>
<td headers="Primary" class="gt_row gt_right">0.5622776</td>
<td headers="Secondary" class="gt_row gt_right">0.5195169</td>
<td headers="Tertiary" class="gt_row gt_right">0.3840125</td>
<td headers="Upper_second" class="gt_row gt_right">0.420354</td>
<td headers="NA" class="gt_row gt_right">0.2</td></tr>
  </tbody>
  
  
</table>
</div>

<br>

- A??adimos una nota al pie (???source note???) en ???Table footer??? con la funci??n `tab_source_note()`. Se pueden poner varias notas al pie.

``` r
gt_tbl <- gt_tbl %>% 
          tab_source_note(md("Fuente: datos de [PIAAC](http://www.oecd.org/skills/piaac/)")) %>%
          tab_source_note(md("Obtenidos a partir del paquete RPIAAC"))
  
gt_tbl  
```

<div id="zbbtlrlmsr" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#zbbtlrlmsr .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#zbbtlrlmsr .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#zbbtlrlmsr .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#zbbtlrlmsr .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#zbbtlrlmsr .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#zbbtlrlmsr .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#zbbtlrlmsr .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#zbbtlrlmsr .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#zbbtlrlmsr .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#zbbtlrlmsr .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#zbbtlrlmsr .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#zbbtlrlmsr .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#zbbtlrlmsr .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#zbbtlrlmsr .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#zbbtlrlmsr .gt_from_md > :first-child {
  margin-top: 0;
}

#zbbtlrlmsr .gt_from_md > :last-child {
  margin-bottom: 0;
}

#zbbtlrlmsr .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#zbbtlrlmsr .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#zbbtlrlmsr .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#zbbtlrlmsr .gt_row_group_first td {
  border-top-width: 2px;
}

#zbbtlrlmsr .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#zbbtlrlmsr .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#zbbtlrlmsr .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#zbbtlrlmsr .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#zbbtlrlmsr .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#zbbtlrlmsr .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#zbbtlrlmsr .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#zbbtlrlmsr .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#zbbtlrlmsr .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#zbbtlrlmsr .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-left: 4px;
  padding-right: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#zbbtlrlmsr .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#zbbtlrlmsr .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#zbbtlrlmsr .gt_left {
  text-align: left;
}

#zbbtlrlmsr .gt_center {
  text-align: center;
}

#zbbtlrlmsr .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#zbbtlrlmsr .gt_font_normal {
  font-weight: normal;
}

#zbbtlrlmsr .gt_font_bold {
  font-weight: bold;
}

#zbbtlrlmsr .gt_font_italic {
  font-style: italic;
}

#zbbtlrlmsr .gt_super {
  font-size: 65%;
}

#zbbtlrlmsr .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 75%;
  vertical-align: 0.4em;
}

#zbbtlrlmsr .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#zbbtlrlmsr .gt_indent_1 {
  text-indent: 5px;
}

#zbbtlrlmsr .gt_indent_2 {
  text-indent: 10px;
}

#zbbtlrlmsr .gt_indent_3 {
  text-indent: 15px;
}

#zbbtlrlmsr .gt_indent_4 {
  text-indent: 20px;
}

#zbbtlrlmsr .gt_indent_5 {
  text-indent: 25px;
}
</style>
<table class="gt_table">
  <thead class="gt_header">
    <tr>
      <td colspan="6" class="gt_heading gt_title gt_font_normal" style><strong>Genero y nivel educativo</strong></td>
    </tr>
    <tr>
      <td colspan="6" class="gt_heading gt_subtitle gt_font_normal gt_bottom_border" style>Porcentaje de <em>H y M</em> en cada nivel educativo</td>
    </tr>
  </thead>
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="Gender">Gender</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Primary">Primary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Secondary">Secondary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Tertiary">Tertiary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Upper_second">Upper_second</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="NA">NA</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="Gender" class="gt_row gt_left">Female</td>
<td headers="Primary" class="gt_row gt_right">0.4377224</td>
<td headers="Secondary" class="gt_row gt_right">0.4804831</td>
<td headers="Tertiary" class="gt_row gt_right">0.6159875</td>
<td headers="Upper_second" class="gt_row gt_right">0.579646</td>
<td headers="NA" class="gt_row gt_right">0.8</td></tr>
    <tr><td headers="Gender" class="gt_row gt_left">Male</td>
<td headers="Primary" class="gt_row gt_right">0.5622776</td>
<td headers="Secondary" class="gt_row gt_right">0.5195169</td>
<td headers="Tertiary" class="gt_row gt_right">0.3840125</td>
<td headers="Upper_second" class="gt_row gt_right">0.420354</td>
<td headers="NA" class="gt_row gt_right">0.2</td></tr>
  </tbody>
  <tfoot class="gt_sourcenotes">
    <tr>
      <td class="gt_sourcenote" colspan="6">Fuente: datos de <a href="http://www.oecd.org/skills/piaac/">PIAAC</a></td>
    </tr>
    <tr>
      <td class="gt_sourcenote" colspan="6">Obtenidos a partir del paquete RPIAAC</td>
    </tr>
  </tfoot>
  
</table>
</div>

<br>

- Podemos a??adir notas (al pie) en los valores de la tabla. Para ello se usa la funci??n `tab_footnote()`. La funci??n auxiliar `cells_body()` se usa para especificar que celdas de datos tendr??n la marca de la llamada al pie de p??gina. Se puede incluso usar condiciones para seleccionar que celdas llevar??n la footnote.

``` r
# A??adimos la misma nota al pie a dos celdas de la tabla
# Para seleccionar las celdas que llevar??n la footnote se usa la f. `cell_body()`
gt_tbl <- gt_tbl %>% tab_footnote("Por encima del 60%", cells_body(c(Tertiary, `NA`), rows = 1) )

# Show the gt Table
gt_tbl
```

<div id="esnftioiii" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#esnftioiii .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#esnftioiii .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#esnftioiii .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#esnftioiii .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#esnftioiii .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#esnftioiii .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#esnftioiii .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#esnftioiii .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#esnftioiii .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#esnftioiii .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#esnftioiii .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#esnftioiii .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#esnftioiii .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#esnftioiii .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#esnftioiii .gt_from_md > :first-child {
  margin-top: 0;
}

#esnftioiii .gt_from_md > :last-child {
  margin-bottom: 0;
}

#esnftioiii .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#esnftioiii .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#esnftioiii .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#esnftioiii .gt_row_group_first td {
  border-top-width: 2px;
}

#esnftioiii .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#esnftioiii .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#esnftioiii .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#esnftioiii .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#esnftioiii .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#esnftioiii .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#esnftioiii .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#esnftioiii .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#esnftioiii .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#esnftioiii .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-left: 4px;
  padding-right: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#esnftioiii .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#esnftioiii .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#esnftioiii .gt_left {
  text-align: left;
}

#esnftioiii .gt_center {
  text-align: center;
}

#esnftioiii .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#esnftioiii .gt_font_normal {
  font-weight: normal;
}

#esnftioiii .gt_font_bold {
  font-weight: bold;
}

#esnftioiii .gt_font_italic {
  font-style: italic;
}

#esnftioiii .gt_super {
  font-size: 65%;
}

#esnftioiii .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 75%;
  vertical-align: 0.4em;
}

#esnftioiii .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#esnftioiii .gt_indent_1 {
  text-indent: 5px;
}

#esnftioiii .gt_indent_2 {
  text-indent: 10px;
}

#esnftioiii .gt_indent_3 {
  text-indent: 15px;
}

#esnftioiii .gt_indent_4 {
  text-indent: 20px;
}

#esnftioiii .gt_indent_5 {
  text-indent: 25px;
}
</style>
<table class="gt_table">
  <thead class="gt_header">
    <tr>
      <td colspan="6" class="gt_heading gt_title gt_font_normal" style><strong>Genero y nivel educativo</strong></td>
    </tr>
    <tr>
      <td colspan="6" class="gt_heading gt_subtitle gt_font_normal gt_bottom_border" style>Porcentaje de <em>H y M</em> en cada nivel educativo</td>
    </tr>
  </thead>
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="Gender">Gender</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Primary">Primary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Secondary">Secondary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Tertiary">Tertiary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Upper_second">Upper_second</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="NA">NA</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="Gender" class="gt_row gt_left">Female</td>
<td headers="Primary" class="gt_row gt_right">0.4377224</td>
<td headers="Secondary" class="gt_row gt_right">0.4804831</td>
<td headers="Tertiary" class="gt_row gt_right"><sup class="gt_footnote_marks">1</sup>??0.6159875</td>
<td headers="Upper_second" class="gt_row gt_right">0.579646</td>
<td headers="NA" class="gt_row gt_right"><sup class="gt_footnote_marks">1</sup>??0.8</td></tr>
    <tr><td headers="Gender" class="gt_row gt_left">Male</td>
<td headers="Primary" class="gt_row gt_right">0.5622776</td>
<td headers="Secondary" class="gt_row gt_right">0.5195169</td>
<td headers="Tertiary" class="gt_row gt_right">0.3840125</td>
<td headers="Upper_second" class="gt_row gt_right">0.420354</td>
<td headers="NA" class="gt_row gt_right">0.2</td></tr>
  </tbody>
  <tfoot class="gt_sourcenotes">
    <tr>
      <td class="gt_sourcenote" colspan="6">Fuente: datos de <a href="http://www.oecd.org/skills/piaac/">PIAAC</a></td>
    </tr>
    <tr>
      <td class="gt_sourcenote" colspan="6">Obtenidos a partir del paquete RPIAAC</td>
    </tr>
  </tfoot>
  <tfoot class="gt_footnotes">
    <tr>
      <td class="gt_footnote" colspan="6"><sup class="gt_footnote_marks">1</sup> Por encima del 60%</td>
    </tr>
  </tfoot>
</table>
</div>

<br>

- The ???Stub??? es el ??rea a la derecha de la tabla que contiene los nombres de filas. Se puede generar f??cilmente un stub con `gt(rowname_col = "nombre")`

An easy way to generate a Stub part is by specifying a stub column in the gt() function with the rowname_col argument. Alternatively, we can have an input dataset with a column named rowname???this magic column will signal to gt that that column should be used as the stub, making row labels. Let???s add a stub with our islands_tbl dataset by modifying the call to gt():

``` r
gt_tbl <- df_tt_4 %>% 
          gt(rowname_col = "Gender") %>% 
          tab_stubhead(label = md("**G??nero**"))

gt_tbl
```

<div id="kraglghkak" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#kraglghkak .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#kraglghkak .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#kraglghkak .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#kraglghkak .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#kraglghkak .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#kraglghkak .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#kraglghkak .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#kraglghkak .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#kraglghkak .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#kraglghkak .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#kraglghkak .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#kraglghkak .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#kraglghkak .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#kraglghkak .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#kraglghkak .gt_from_md > :first-child {
  margin-top: 0;
}

#kraglghkak .gt_from_md > :last-child {
  margin-bottom: 0;
}

#kraglghkak .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#kraglghkak .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#kraglghkak .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#kraglghkak .gt_row_group_first td {
  border-top-width: 2px;
}

#kraglghkak .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#kraglghkak .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#kraglghkak .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#kraglghkak .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#kraglghkak .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#kraglghkak .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#kraglghkak .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#kraglghkak .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#kraglghkak .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#kraglghkak .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-left: 4px;
  padding-right: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#kraglghkak .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#kraglghkak .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#kraglghkak .gt_left {
  text-align: left;
}

#kraglghkak .gt_center {
  text-align: center;
}

#kraglghkak .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#kraglghkak .gt_font_normal {
  font-weight: normal;
}

#kraglghkak .gt_font_bold {
  font-weight: bold;
}

#kraglghkak .gt_font_italic {
  font-style: italic;
}

#kraglghkak .gt_super {
  font-size: 65%;
}

#kraglghkak .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 75%;
  vertical-align: 0.4em;
}

#kraglghkak .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#kraglghkak .gt_indent_1 {
  text-indent: 5px;
}

#kraglghkak .gt_indent_2 {
  text-indent: 10px;
}

#kraglghkak .gt_indent_3 {
  text-indent: 15px;
}

#kraglghkak .gt_indent_4 {
  text-indent: 20px;
}

#kraglghkak .gt_indent_5 {
  text-indent: 25px;
}
</style>
<table class="gt_table">
  
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="&lt;strong&gt;G??nero&lt;/strong&gt;"><strong>G??nero</strong></th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Primary">Primary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Secondary">Secondary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Tertiary">Tertiary</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Upper_second">Upper_second</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="NA">NA</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><th id="stub_1_1" scope="row" class="gt_row gt_left gt_stub">Female</th>
<td headers="stub_1_1 Primary" class="gt_row gt_right">0.4377224</td>
<td headers="stub_1_1 Secondary" class="gt_row gt_right">0.4804831</td>
<td headers="stub_1_1 Tertiary" class="gt_row gt_right">0.6159875</td>
<td headers="stub_1_1 Upper_second" class="gt_row gt_right">0.579646</td>
<td headers="stub_1_1 NA" class="gt_row gt_right">0.8</td></tr>
    <tr><th id="stub_1_2" scope="row" class="gt_row gt_left gt_stub">Male</th>
<td headers="stub_1_2 Primary" class="gt_row gt_right">0.5622776</td>
<td headers="stub_1_2 Secondary" class="gt_row gt_right">0.5195169</td>
<td headers="stub_1_2 Tertiary" class="gt_row gt_right">0.3840125</td>
<td headers="stub_1_2 Upper_second" class="gt_row gt_right">0.420354</td>
<td headers="stub_1_2 NA" class="gt_row gt_right">0.2</td></tr>
  </tbody>
  
  
</table>
</div>

<br>

Con `gt` se pueden hacer muchas m??s cosas, puedes verlas en su [`p??gina web`](https://gt.rstudio.com/), o en esta secuencia de posts de Thomas Mock: [10+ Guidelines for Better Tables in R](https://themockup.blog/posts/2020-09-04-10-table-rules-in-r/), [Functions and Themes for gt tables](https://themockup.blog/posts/2020-09-26-functions-and-themes-for-gt-tables/), [Embedding custom HTML in gt tables](https://themockup.blog/posts/2020-10-31-embedding-custom-features-in-gt-tables/) y [gt - a (G)rammar of (T)ables](https://themockup.blog/posts/2020-05-16-gt-a-grammer-of-tables/).

<br>

Un ejemplo que me ha gustado es [este](https://github.com/sharlagelfand/twofunctionsmostdays/tree/master/2020/05/16) de [Sharla Gelfand](https://github.com/sharlagelfand) en el que a??ade una columna de im??genes a su tabla. Voy a hacerlo yo con 3 im??genes de Wikimedia Commons y una tabla con datos del data.frame iris.

Para ello, primero, a??ado una columna con los url???s de las fotos al data.frame `iris`:

``` r
urls_lirios <- c("https://upload.wikimedia.org/wikipedia/commons/thumb/2/2d/Iris_latifolia-Lac_Aule-Laruns-2522~2013_07_29.JPG/1280px-Iris_latifolia-Lac_Aule-Laruns-2522~2013_07_29.JPG",
                 "https://upload.wikimedia.org/wikipedia/commons/thumb/2/21/Lilium_michiganense_2.jpg/310px-Lilium_michiganense_2.jpg",
                 "https://upload.wikimedia.org/wikipedia/commons/thumb/b/bd/Nacho_Vegas_Fib.jpg/800px-Nacho_Vegas_Fib.jpg")

iris_con_urls <- iris %>% group_by(Species) %>% slice_max(Sepal.Length, n = 1) %>% add_column(urls_lirios) %>% ungroup()
```

Para despu??s transformar los urls a im??genes con:

``` r
iris_con_urls %>% gt() %>% 
  gt::text_transform(locations = cells_body(columns = c(urls_lirios)),
                     fn = function(x) {gt::web_image(x, height = 30)})
```

<div id="xlknlidank" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#xlknlidank .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#xlknlidank .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#xlknlidank .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#xlknlidank .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#xlknlidank .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#xlknlidank .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#xlknlidank .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#xlknlidank .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#xlknlidank .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#xlknlidank .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#xlknlidank .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#xlknlidank .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#xlknlidank .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#xlknlidank .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#xlknlidank .gt_from_md > :first-child {
  margin-top: 0;
}

#xlknlidank .gt_from_md > :last-child {
  margin-bottom: 0;
}

#xlknlidank .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#xlknlidank .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#xlknlidank .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#xlknlidank .gt_row_group_first td {
  border-top-width: 2px;
}

#xlknlidank .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#xlknlidank .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#xlknlidank .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#xlknlidank .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#xlknlidank .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#xlknlidank .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#xlknlidank .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#xlknlidank .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#xlknlidank .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#xlknlidank .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-left: 4px;
  padding-right: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#xlknlidank .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#xlknlidank .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#xlknlidank .gt_left {
  text-align: left;
}

#xlknlidank .gt_center {
  text-align: center;
}

#xlknlidank .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#xlknlidank .gt_font_normal {
  font-weight: normal;
}

#xlknlidank .gt_font_bold {
  font-weight: bold;
}

#xlknlidank .gt_font_italic {
  font-style: italic;
}

#xlknlidank .gt_super {
  font-size: 65%;
}

#xlknlidank .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 75%;
  vertical-align: 0.4em;
}

#xlknlidank .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#xlknlidank .gt_indent_1 {
  text-indent: 5px;
}

#xlknlidank .gt_indent_2 {
  text-indent: 10px;
}

#xlknlidank .gt_indent_3 {
  text-indent: 15px;
}

#xlknlidank .gt_indent_4 {
  text-indent: 20px;
}

#xlknlidank .gt_indent_5 {
  text-indent: 25px;
}
</style>
<table class="gt_table">
  
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Sepal.Length">Sepal.Length</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Sepal.Width">Sepal.Width</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Petal.Length">Petal.Length</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="Petal.Width">Petal.Width</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1" scope="col" id="Species">Species</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="urls_lirios">urls_lirios</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="Sepal.Length" class="gt_row gt_right">5.8</td>
<td headers="Sepal.Width" class="gt_row gt_right">4.0</td>
<td headers="Petal.Length" class="gt_row gt_right">1.2</td>
<td headers="Petal.Width" class="gt_row gt_right">0.2</td>
<td headers="Species" class="gt_row gt_center">setosa</td>
<td headers="urls_lirios" class="gt_row gt_left"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2d/Iris_latifolia-Lac_Aule-Laruns-2522~2013_07_29.JPG/1280px-Iris_latifolia-Lac_Aule-Laruns-2522~2013_07_29.JPG" style="height:30px;"></td></tr>
    <tr><td headers="Sepal.Length" class="gt_row gt_right">7.0</td>
<td headers="Sepal.Width" class="gt_row gt_right">3.2</td>
<td headers="Petal.Length" class="gt_row gt_right">4.7</td>
<td headers="Petal.Width" class="gt_row gt_right">1.4</td>
<td headers="Species" class="gt_row gt_center">versicolor</td>
<td headers="urls_lirios" class="gt_row gt_left"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/21/Lilium_michiganense_2.jpg/310px-Lilium_michiganense_2.jpg" style="height:30px;"></td></tr>
    <tr><td headers="Sepal.Length" class="gt_row gt_right">7.9</td>
<td headers="Sepal.Width" class="gt_row gt_right">3.8</td>
<td headers="Petal.Length" class="gt_row gt_right">6.4</td>
<td headers="Petal.Width" class="gt_row gt_right">2.0</td>
<td headers="Species" class="gt_row gt_center">virginica</td>
<td headers="urls_lirios" class="gt_row gt_left"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/bd/Nacho_Vegas_Fib.jpg/800px-Nacho_Vegas_Fib.jpg" style="height:30px;"></td></tr>
  </tbody>
  
  
</table>
</div>

En [este post](https://bjnnowak.netlify.app/2021/10/04/r-beautiful-tables-with-gt-and-gtextras/) se muestra como incluir, no solo im??genes, sino tambi??n gr??ficos ggplot en una tabla hecha con `gt`. Para ello usa el paquete [`gtExtras`](https://jthomasmock.github.io/gtExtras/index.html). Por ejemplo est?? maravilla de tabla:

tt_08_img_02_tabla-ganadores-tour.png

------------------------------------------------------------------------

<br>

# 5. Tablas interactivas

[Aqu??](https://thinkr.fr/tableaux-interactifs-avec-r-pour-shiny-et-vos-pages-web/) tienes un tutorial exclusivamente dedicado a tablas interactivas. Aqu?? s??lo presentar?? alg??n ejemplo de tabla interactiva con los paquetes `DT`, `reactable` y `rpivottable`.

<br>

## 5.1 `DT` package

El paquete [DT](https://cran.r-project.org/web/packages/DT/index.html) es ???a wrapper of the JavaScript library DataTables???. La mejor forma de aprender a hacer tablas con DT es su [p??gina web](https://rstudio.github.io/DT/).

El autor de `DT` es [Yihui Xie](https://yihui.org/en/) el desarrollador de `knitr`. El principal atractivo del paquete es que permite hacer tablas interactivas con funcionalidades como filtrar, paginar, ordenar, etc??? los valores de las tablas.

Hacer tablas b??sicas con DT es muy sencillo. Por ejemplo:

<br>

``` r
DT::datatable(iris)
```

<div id="htmlwidget-1" style="width:100%;height:auto;" class="datatables html-widget"></div>
<script type="application/json" data-for="htmlwidget-1">{"x":{"filter":"none","data":[["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","31","32","33","34","35","36","37","38","39","40","41","42","43","44","45","46","47","48","49","50","51","52","53","54","55","56","57","58","59","60","61","62","63","64","65","66","67","68","69","70","71","72","73","74","75","76","77","78","79","80","81","82","83","84","85","86","87","88","89","90","91","92","93","94","95","96","97","98","99","100","101","102","103","104","105","106","107","108","109","110","111","112","113","114","115","116","117","118","119","120","121","122","123","124","125","126","127","128","129","130","131","132","133","134","135","136","137","138","139","140","141","142","143","144","145","146","147","148","149","150"],[5.1,4.9,4.7,4.6,5,5.4,4.6,5,4.4,4.9,5.4,4.8,4.8,4.3,5.8,5.7,5.4,5.1,5.7,5.1,5.4,5.1,4.6,5.1,4.8,5,5,5.2,5.2,4.7,4.8,5.4,5.2,5.5,4.9,5,5.5,4.9,4.4,5.1,5,4.5,4.4,5,5.1,4.8,5.1,4.6,5.3,5,7,6.4,6.9,5.5,6.5,5.7,6.3,4.9,6.6,5.2,5,5.9,6,6.1,5.6,6.7,5.6,5.8,6.2,5.6,5.9,6.1,6.3,6.1,6.4,6.6,6.8,6.7,6,5.7,5.5,5.5,5.8,6,5.4,6,6.7,6.3,5.6,5.5,5.5,6.1,5.8,5,5.6,5.7,5.7,6.2,5.1,5.7,6.3,5.8,7.1,6.3,6.5,7.6,4.9,7.3,6.7,7.2,6.5,6.4,6.8,5.7,5.8,6.4,6.5,7.7,7.7,6,6.9,5.6,7.7,6.3,6.7,7.2,6.2,6.1,6.4,7.2,7.4,7.9,6.4,6.3,6.1,7.7,6.3,6.4,6,6.9,6.7,6.9,5.8,6.8,6.7,6.7,6.3,6.5,6.2,5.9],[3.5,3,3.2,3.1,3.6,3.9,3.4,3.4,2.9,3.1,3.7,3.4,3,3,4,4.4,3.9,3.5,3.8,3.8,3.4,3.7,3.6,3.3,3.4,3,3.4,3.5,3.4,3.2,3.1,3.4,4.1,4.2,3.1,3.2,3.5,3.6,3,3.4,3.5,2.3,3.2,3.5,3.8,3,3.8,3.2,3.7,3.3,3.2,3.2,3.1,2.3,2.8,2.8,3.3,2.4,2.9,2.7,2,3,2.2,2.9,2.9,3.1,3,2.7,2.2,2.5,3.2,2.8,2.5,2.8,2.9,3,2.8,3,2.9,2.6,2.4,2.4,2.7,2.7,3,3.4,3.1,2.3,3,2.5,2.6,3,2.6,2.3,2.7,3,2.9,2.9,2.5,2.8,3.3,2.7,3,2.9,3,3,2.5,2.9,2.5,3.6,3.2,2.7,3,2.5,2.8,3.2,3,3.8,2.6,2.2,3.2,2.8,2.8,2.7,3.3,3.2,2.8,3,2.8,3,2.8,3.8,2.8,2.8,2.6,3,3.4,3.1,3,3.1,3.1,3.1,2.7,3.2,3.3,3,2.5,3,3.4,3],[1.4,1.4,1.3,1.5,1.4,1.7,1.4,1.5,1.4,1.5,1.5,1.6,1.4,1.1,1.2,1.5,1.3,1.4,1.7,1.5,1.7,1.5,1,1.7,1.9,1.6,1.6,1.5,1.4,1.6,1.6,1.5,1.5,1.4,1.5,1.2,1.3,1.4,1.3,1.5,1.3,1.3,1.3,1.6,1.9,1.4,1.6,1.4,1.5,1.4,4.7,4.5,4.9,4,4.6,4.5,4.7,3.3,4.6,3.9,3.5,4.2,4,4.7,3.6,4.4,4.5,4.1,4.5,3.9,4.8,4,4.9,4.7,4.3,4.4,4.8,5,4.5,3.5,3.8,3.7,3.9,5.1,4.5,4.5,4.7,4.4,4.1,4,4.4,4.6,4,3.3,4.2,4.2,4.2,4.3,3,4.1,6,5.1,5.9,5.6,5.8,6.6,4.5,6.3,5.8,6.1,5.1,5.3,5.5,5,5.1,5.3,5.5,6.7,6.9,5,5.7,4.9,6.7,4.9,5.7,6,4.8,4.9,5.6,5.8,6.1,6.4,5.6,5.1,5.6,6.1,5.6,5.5,4.8,5.4,5.6,5.1,5.1,5.9,5.7,5.2,5,5.2,5.4,5.1],[0.2,0.2,0.2,0.2,0.2,0.4,0.3,0.2,0.2,0.1,0.2,0.2,0.1,0.1,0.2,0.4,0.4,0.3,0.3,0.3,0.2,0.4,0.2,0.5,0.2,0.2,0.4,0.2,0.2,0.2,0.2,0.4,0.1,0.2,0.2,0.2,0.2,0.1,0.2,0.2,0.3,0.3,0.2,0.6,0.4,0.3,0.2,0.2,0.2,0.2,1.4,1.5,1.5,1.3,1.5,1.3,1.6,1,1.3,1.4,1,1.5,1,1.4,1.3,1.4,1.5,1,1.5,1.1,1.8,1.3,1.5,1.2,1.3,1.4,1.4,1.7,1.5,1,1.1,1,1.2,1.6,1.5,1.6,1.5,1.3,1.3,1.3,1.2,1.4,1.2,1,1.3,1.2,1.3,1.3,1.1,1.3,2.5,1.9,2.1,1.8,2.2,2.1,1.7,1.8,1.8,2.5,2,1.9,2.1,2,2.4,2.3,1.8,2.2,2.3,1.5,2.3,2,2,1.8,2.1,1.8,1.8,1.8,2.1,1.6,1.9,2,2.2,1.5,1.4,2.3,2.4,1.8,1.8,2.1,2.4,2.3,1.9,2.3,2.5,2.3,1.9,2,2.3,1.8],["setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica"]],"container":"<table class=\"display\">\n  <thead>\n    <tr>\n      <th> <\/th>\n      <th>Sepal.Length<\/th>\n      <th>Sepal.Width<\/th>\n      <th>Petal.Length<\/th>\n      <th>Petal.Width<\/th>\n      <th>Species<\/th>\n    <\/tr>\n  <\/thead>\n<\/table>","options":{"columnDefs":[{"className":"dt-right","targets":[1,2,3,4]},{"orderable":false,"targets":0}],"order":[],"autoWidth":false,"orderClasses":false}},"evals":[],"jsHooks":[]}</script>

<br>

Las tablas hechas con DT tienen muchas m??s posibilidades. Como ejemplo la siguiente tabla.La mejor forma de aprender a hacer tablas con DT es su [p??gina web](https://rstudio.github.io/DT/)

``` r
DT::datatable(iris, filter = 'top', 
              options = list(pageLength = 5, autoWidth = TRUE ))
```

<div id="htmlwidget-2" style="width:100%;height:auto;" class="datatables html-widget"></div>
<script type="application/json" data-for="htmlwidget-2">{"x":{"filter":"top","filterHTML":"<tr>\n  <td><\/td>\n  <td data-type=\"number\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"display: none; position: absolute; width: 200px;\">\n      <div data-min=\"4.3\" data-max=\"7.9\" data-scale=\"1\"><\/div>\n      <span style=\"float: left;\"><\/span>\n      <span style=\"float: right;\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"number\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"display: none; position: absolute; width: 200px;\">\n      <div data-min=\"2\" data-max=\"4.4\" data-scale=\"1\"><\/div>\n      <span style=\"float: left;\"><\/span>\n      <span style=\"float: right;\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"number\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"display: none; position: absolute; width: 200px;\">\n      <div data-min=\"1\" data-max=\"6.9\" data-scale=\"1\"><\/div>\n      <span style=\"float: left;\"><\/span>\n      <span style=\"float: right;\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"number\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"display: none; position: absolute; width: 200px;\">\n      <div data-min=\"0.1\" data-max=\"2.5\" data-scale=\"1\"><\/div>\n      <span style=\"float: left;\"><\/span>\n      <span style=\"float: right;\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"factor\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"width: 100%; display: none;\">\n      <select multiple=\"multiple\" style=\"width: 100%;\" data-options=\"[&quot;setosa&quot;,&quot;versicolor&quot;,&quot;virginica&quot;]\"><\/select>\n    <\/div>\n  <\/td>\n<\/tr>","data":[["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","31","32","33","34","35","36","37","38","39","40","41","42","43","44","45","46","47","48","49","50","51","52","53","54","55","56","57","58","59","60","61","62","63","64","65","66","67","68","69","70","71","72","73","74","75","76","77","78","79","80","81","82","83","84","85","86","87","88","89","90","91","92","93","94","95","96","97","98","99","100","101","102","103","104","105","106","107","108","109","110","111","112","113","114","115","116","117","118","119","120","121","122","123","124","125","126","127","128","129","130","131","132","133","134","135","136","137","138","139","140","141","142","143","144","145","146","147","148","149","150"],[5.1,4.9,4.7,4.6,5,5.4,4.6,5,4.4,4.9,5.4,4.8,4.8,4.3,5.8,5.7,5.4,5.1,5.7,5.1,5.4,5.1,4.6,5.1,4.8,5,5,5.2,5.2,4.7,4.8,5.4,5.2,5.5,4.9,5,5.5,4.9,4.4,5.1,5,4.5,4.4,5,5.1,4.8,5.1,4.6,5.3,5,7,6.4,6.9,5.5,6.5,5.7,6.3,4.9,6.6,5.2,5,5.9,6,6.1,5.6,6.7,5.6,5.8,6.2,5.6,5.9,6.1,6.3,6.1,6.4,6.6,6.8,6.7,6,5.7,5.5,5.5,5.8,6,5.4,6,6.7,6.3,5.6,5.5,5.5,6.1,5.8,5,5.6,5.7,5.7,6.2,5.1,5.7,6.3,5.8,7.1,6.3,6.5,7.6,4.9,7.3,6.7,7.2,6.5,6.4,6.8,5.7,5.8,6.4,6.5,7.7,7.7,6,6.9,5.6,7.7,6.3,6.7,7.2,6.2,6.1,6.4,7.2,7.4,7.9,6.4,6.3,6.1,7.7,6.3,6.4,6,6.9,6.7,6.9,5.8,6.8,6.7,6.7,6.3,6.5,6.2,5.9],[3.5,3,3.2,3.1,3.6,3.9,3.4,3.4,2.9,3.1,3.7,3.4,3,3,4,4.4,3.9,3.5,3.8,3.8,3.4,3.7,3.6,3.3,3.4,3,3.4,3.5,3.4,3.2,3.1,3.4,4.1,4.2,3.1,3.2,3.5,3.6,3,3.4,3.5,2.3,3.2,3.5,3.8,3,3.8,3.2,3.7,3.3,3.2,3.2,3.1,2.3,2.8,2.8,3.3,2.4,2.9,2.7,2,3,2.2,2.9,2.9,3.1,3,2.7,2.2,2.5,3.2,2.8,2.5,2.8,2.9,3,2.8,3,2.9,2.6,2.4,2.4,2.7,2.7,3,3.4,3.1,2.3,3,2.5,2.6,3,2.6,2.3,2.7,3,2.9,2.9,2.5,2.8,3.3,2.7,3,2.9,3,3,2.5,2.9,2.5,3.6,3.2,2.7,3,2.5,2.8,3.2,3,3.8,2.6,2.2,3.2,2.8,2.8,2.7,3.3,3.2,2.8,3,2.8,3,2.8,3.8,2.8,2.8,2.6,3,3.4,3.1,3,3.1,3.1,3.1,2.7,3.2,3.3,3,2.5,3,3.4,3],[1.4,1.4,1.3,1.5,1.4,1.7,1.4,1.5,1.4,1.5,1.5,1.6,1.4,1.1,1.2,1.5,1.3,1.4,1.7,1.5,1.7,1.5,1,1.7,1.9,1.6,1.6,1.5,1.4,1.6,1.6,1.5,1.5,1.4,1.5,1.2,1.3,1.4,1.3,1.5,1.3,1.3,1.3,1.6,1.9,1.4,1.6,1.4,1.5,1.4,4.7,4.5,4.9,4,4.6,4.5,4.7,3.3,4.6,3.9,3.5,4.2,4,4.7,3.6,4.4,4.5,4.1,4.5,3.9,4.8,4,4.9,4.7,4.3,4.4,4.8,5,4.5,3.5,3.8,3.7,3.9,5.1,4.5,4.5,4.7,4.4,4.1,4,4.4,4.6,4,3.3,4.2,4.2,4.2,4.3,3,4.1,6,5.1,5.9,5.6,5.8,6.6,4.5,6.3,5.8,6.1,5.1,5.3,5.5,5,5.1,5.3,5.5,6.7,6.9,5,5.7,4.9,6.7,4.9,5.7,6,4.8,4.9,5.6,5.8,6.1,6.4,5.6,5.1,5.6,6.1,5.6,5.5,4.8,5.4,5.6,5.1,5.1,5.9,5.7,5.2,5,5.2,5.4,5.1],[0.2,0.2,0.2,0.2,0.2,0.4,0.3,0.2,0.2,0.1,0.2,0.2,0.1,0.1,0.2,0.4,0.4,0.3,0.3,0.3,0.2,0.4,0.2,0.5,0.2,0.2,0.4,0.2,0.2,0.2,0.2,0.4,0.1,0.2,0.2,0.2,0.2,0.1,0.2,0.2,0.3,0.3,0.2,0.6,0.4,0.3,0.2,0.2,0.2,0.2,1.4,1.5,1.5,1.3,1.5,1.3,1.6,1,1.3,1.4,1,1.5,1,1.4,1.3,1.4,1.5,1,1.5,1.1,1.8,1.3,1.5,1.2,1.3,1.4,1.4,1.7,1.5,1,1.1,1,1.2,1.6,1.5,1.6,1.5,1.3,1.3,1.3,1.2,1.4,1.2,1,1.3,1.2,1.3,1.3,1.1,1.3,2.5,1.9,2.1,1.8,2.2,2.1,1.7,1.8,1.8,2.5,2,1.9,2.1,2,2.4,2.3,1.8,2.2,2.3,1.5,2.3,2,2,1.8,2.1,1.8,1.8,1.8,2.1,1.6,1.9,2,2.2,1.5,1.4,2.3,2.4,1.8,1.8,2.1,2.4,2.3,1.9,2.3,2.5,2.3,1.9,2,2.3,1.8],["setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica"]],"container":"<table class=\"display\">\n  <thead>\n    <tr>\n      <th> <\/th>\n      <th>Sepal.Length<\/th>\n      <th>Sepal.Width<\/th>\n      <th>Petal.Length<\/th>\n      <th>Petal.Width<\/th>\n      <th>Species<\/th>\n    <\/tr>\n  <\/thead>\n<\/table>","options":{"pageLength":5,"autoWidth":true,"columnDefs":[{"className":"dt-right","targets":[1,2,3,4]},{"orderable":false,"targets":0}],"order":[],"orderClasses":false,"orderCellsTop":true,"lengthMenu":[5,10,25,50,100]}},"evals":[],"jsHooks":[]}</script>

<br>

Una posibilidad de las tablas hechas con `DT` es que se pueden descargar. Lo explican en detalle [aqu??](https://martinctc.github.io/blog/vignette-downloadable-tables-in-rmarkdown-with-the-dt-package/):

``` r
iris %>% DT::datatable(extensions = 'Buttons', 
               options = list(dom = 'Blfrtip', 
                              buttons = c('copy', 'csv', 'excel', 'pdf', 'print'), 
                              pageLength = 5, autoWidth = TRUE ))
```

<div id="htmlwidget-3" style="width:100%;height:auto;" class="datatables html-widget"></div>
<script type="application/json" data-for="htmlwidget-3">{"x":{"filter":"none","extensions":["Buttons"],"data":[["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","31","32","33","34","35","36","37","38","39","40","41","42","43","44","45","46","47","48","49","50","51","52","53","54","55","56","57","58","59","60","61","62","63","64","65","66","67","68","69","70","71","72","73","74","75","76","77","78","79","80","81","82","83","84","85","86","87","88","89","90","91","92","93","94","95","96","97","98","99","100","101","102","103","104","105","106","107","108","109","110","111","112","113","114","115","116","117","118","119","120","121","122","123","124","125","126","127","128","129","130","131","132","133","134","135","136","137","138","139","140","141","142","143","144","145","146","147","148","149","150"],[5.1,4.9,4.7,4.6,5,5.4,4.6,5,4.4,4.9,5.4,4.8,4.8,4.3,5.8,5.7,5.4,5.1,5.7,5.1,5.4,5.1,4.6,5.1,4.8,5,5,5.2,5.2,4.7,4.8,5.4,5.2,5.5,4.9,5,5.5,4.9,4.4,5.1,5,4.5,4.4,5,5.1,4.8,5.1,4.6,5.3,5,7,6.4,6.9,5.5,6.5,5.7,6.3,4.9,6.6,5.2,5,5.9,6,6.1,5.6,6.7,5.6,5.8,6.2,5.6,5.9,6.1,6.3,6.1,6.4,6.6,6.8,6.7,6,5.7,5.5,5.5,5.8,6,5.4,6,6.7,6.3,5.6,5.5,5.5,6.1,5.8,5,5.6,5.7,5.7,6.2,5.1,5.7,6.3,5.8,7.1,6.3,6.5,7.6,4.9,7.3,6.7,7.2,6.5,6.4,6.8,5.7,5.8,6.4,6.5,7.7,7.7,6,6.9,5.6,7.7,6.3,6.7,7.2,6.2,6.1,6.4,7.2,7.4,7.9,6.4,6.3,6.1,7.7,6.3,6.4,6,6.9,6.7,6.9,5.8,6.8,6.7,6.7,6.3,6.5,6.2,5.9],[3.5,3,3.2,3.1,3.6,3.9,3.4,3.4,2.9,3.1,3.7,3.4,3,3,4,4.4,3.9,3.5,3.8,3.8,3.4,3.7,3.6,3.3,3.4,3,3.4,3.5,3.4,3.2,3.1,3.4,4.1,4.2,3.1,3.2,3.5,3.6,3,3.4,3.5,2.3,3.2,3.5,3.8,3,3.8,3.2,3.7,3.3,3.2,3.2,3.1,2.3,2.8,2.8,3.3,2.4,2.9,2.7,2,3,2.2,2.9,2.9,3.1,3,2.7,2.2,2.5,3.2,2.8,2.5,2.8,2.9,3,2.8,3,2.9,2.6,2.4,2.4,2.7,2.7,3,3.4,3.1,2.3,3,2.5,2.6,3,2.6,2.3,2.7,3,2.9,2.9,2.5,2.8,3.3,2.7,3,2.9,3,3,2.5,2.9,2.5,3.6,3.2,2.7,3,2.5,2.8,3.2,3,3.8,2.6,2.2,3.2,2.8,2.8,2.7,3.3,3.2,2.8,3,2.8,3,2.8,3.8,2.8,2.8,2.6,3,3.4,3.1,3,3.1,3.1,3.1,2.7,3.2,3.3,3,2.5,3,3.4,3],[1.4,1.4,1.3,1.5,1.4,1.7,1.4,1.5,1.4,1.5,1.5,1.6,1.4,1.1,1.2,1.5,1.3,1.4,1.7,1.5,1.7,1.5,1,1.7,1.9,1.6,1.6,1.5,1.4,1.6,1.6,1.5,1.5,1.4,1.5,1.2,1.3,1.4,1.3,1.5,1.3,1.3,1.3,1.6,1.9,1.4,1.6,1.4,1.5,1.4,4.7,4.5,4.9,4,4.6,4.5,4.7,3.3,4.6,3.9,3.5,4.2,4,4.7,3.6,4.4,4.5,4.1,4.5,3.9,4.8,4,4.9,4.7,4.3,4.4,4.8,5,4.5,3.5,3.8,3.7,3.9,5.1,4.5,4.5,4.7,4.4,4.1,4,4.4,4.6,4,3.3,4.2,4.2,4.2,4.3,3,4.1,6,5.1,5.9,5.6,5.8,6.6,4.5,6.3,5.8,6.1,5.1,5.3,5.5,5,5.1,5.3,5.5,6.7,6.9,5,5.7,4.9,6.7,4.9,5.7,6,4.8,4.9,5.6,5.8,6.1,6.4,5.6,5.1,5.6,6.1,5.6,5.5,4.8,5.4,5.6,5.1,5.1,5.9,5.7,5.2,5,5.2,5.4,5.1],[0.2,0.2,0.2,0.2,0.2,0.4,0.3,0.2,0.2,0.1,0.2,0.2,0.1,0.1,0.2,0.4,0.4,0.3,0.3,0.3,0.2,0.4,0.2,0.5,0.2,0.2,0.4,0.2,0.2,0.2,0.2,0.4,0.1,0.2,0.2,0.2,0.2,0.1,0.2,0.2,0.3,0.3,0.2,0.6,0.4,0.3,0.2,0.2,0.2,0.2,1.4,1.5,1.5,1.3,1.5,1.3,1.6,1,1.3,1.4,1,1.5,1,1.4,1.3,1.4,1.5,1,1.5,1.1,1.8,1.3,1.5,1.2,1.3,1.4,1.4,1.7,1.5,1,1.1,1,1.2,1.6,1.5,1.6,1.5,1.3,1.3,1.3,1.2,1.4,1.2,1,1.3,1.2,1.3,1.3,1.1,1.3,2.5,1.9,2.1,1.8,2.2,2.1,1.7,1.8,1.8,2.5,2,1.9,2.1,2,2.4,2.3,1.8,2.2,2.3,1.5,2.3,2,2,1.8,2.1,1.8,1.8,1.8,2.1,1.6,1.9,2,2.2,1.5,1.4,2.3,2.4,1.8,1.8,2.1,2.4,2.3,1.9,2.3,2.5,2.3,1.9,2,2.3,1.8],["setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica"]],"container":"<table class=\"display\">\n  <thead>\n    <tr>\n      <th> <\/th>\n      <th>Sepal.Length<\/th>\n      <th>Sepal.Width<\/th>\n      <th>Petal.Length<\/th>\n      <th>Petal.Width<\/th>\n      <th>Species<\/th>\n    <\/tr>\n  <\/thead>\n<\/table>","options":{"dom":"Blfrtip","buttons":["copy","csv","excel","pdf","print"],"pageLength":5,"autoWidth":true,"columnDefs":[{"className":"dt-right","targets":[1,2,3,4]},{"orderable":false,"targets":0}],"order":[],"orderClasses":false,"lengthMenu":[5,10,25,50,100]}},"evals":[],"jsHooks":[]}</script>

<br>

------------------------------------------------------------------------

## 5.2 `reactable` package

El paquete [`reactable`](https://glin.github.io/reactable/index.html) tambi??n permite hacer tablas interactivas, esta vez se basa en la librer??a de JS React.

El uso b??sico es tan sencillo como:

``` r
reactable::reactable(iris)
```

<div id="htmlwidget-4" class="reactable html-widget" style="width:auto;height:auto;"></div>
<script type="application/json" data-for="htmlwidget-4">{"x":{"tag":{"name":"Reactable","attribs":{"data":{"Sepal.Length":[5.1,4.9,4.7,4.6,5,5.4,4.6,5,4.4,4.9,5.4,4.8,4.8,4.3,5.8,5.7,5.4,5.1,5.7,5.1,5.4,5.1,4.6,5.1,4.8,5,5,5.2,5.2,4.7,4.8,5.4,5.2,5.5,4.9,5,5.5,4.9,4.4,5.1,5,4.5,4.4,5,5.1,4.8,5.1,4.6,5.3,5,7,6.4,6.9,5.5,6.5,5.7,6.3,4.9,6.6,5.2,5,5.9,6,6.1,5.6,6.7,5.6,5.8,6.2,5.6,5.9,6.1,6.3,6.1,6.4,6.6,6.8,6.7,6,5.7,5.5,5.5,5.8,6,5.4,6,6.7,6.3,5.6,5.5,5.5,6.1,5.8,5,5.6,5.7,5.7,6.2,5.1,5.7,6.3,5.8,7.1,6.3,6.5,7.6,4.9,7.3,6.7,7.2,6.5,6.4,6.8,5.7,5.8,6.4,6.5,7.7,7.7,6,6.9,5.6,7.7,6.3,6.7,7.2,6.2,6.1,6.4,7.2,7.4,7.9,6.4,6.3,6.1,7.7,6.3,6.4,6,6.9,6.7,6.9,5.8,6.8,6.7,6.7,6.3,6.5,6.2,5.9],"Sepal.Width":[3.5,3,3.2,3.1,3.6,3.9,3.4,3.4,2.9,3.1,3.7,3.4,3,3,4,4.4,3.9,3.5,3.8,3.8,3.4,3.7,3.6,3.3,3.4,3,3.4,3.5,3.4,3.2,3.1,3.4,4.1,4.2,3.1,3.2,3.5,3.6,3,3.4,3.5,2.3,3.2,3.5,3.8,3,3.8,3.2,3.7,3.3,3.2,3.2,3.1,2.3,2.8,2.8,3.3,2.4,2.9,2.7,2,3,2.2,2.9,2.9,3.1,3,2.7,2.2,2.5,3.2,2.8,2.5,2.8,2.9,3,2.8,3,2.9,2.6,2.4,2.4,2.7,2.7,3,3.4,3.1,2.3,3,2.5,2.6,3,2.6,2.3,2.7,3,2.9,2.9,2.5,2.8,3.3,2.7,3,2.9,3,3,2.5,2.9,2.5,3.6,3.2,2.7,3,2.5,2.8,3.2,3,3.8,2.6,2.2,3.2,2.8,2.8,2.7,3.3,3.2,2.8,3,2.8,3,2.8,3.8,2.8,2.8,2.6,3,3.4,3.1,3,3.1,3.1,3.1,2.7,3.2,3.3,3,2.5,3,3.4,3],"Petal.Length":[1.4,1.4,1.3,1.5,1.4,1.7,1.4,1.5,1.4,1.5,1.5,1.6,1.4,1.1,1.2,1.5,1.3,1.4,1.7,1.5,1.7,1.5,1,1.7,1.9,1.6,1.6,1.5,1.4,1.6,1.6,1.5,1.5,1.4,1.5,1.2,1.3,1.4,1.3,1.5,1.3,1.3,1.3,1.6,1.9,1.4,1.6,1.4,1.5,1.4,4.7,4.5,4.9,4,4.6,4.5,4.7,3.3,4.6,3.9,3.5,4.2,4,4.7,3.6,4.4,4.5,4.1,4.5,3.9,4.8,4,4.9,4.7,4.3,4.4,4.8,5,4.5,3.5,3.8,3.7,3.9,5.1,4.5,4.5,4.7,4.4,4.1,4,4.4,4.6,4,3.3,4.2,4.2,4.2,4.3,3,4.1,6,5.1,5.9,5.6,5.8,6.6,4.5,6.3,5.8,6.1,5.1,5.3,5.5,5,5.1,5.3,5.5,6.7,6.9,5,5.7,4.9,6.7,4.9,5.7,6,4.8,4.9,5.6,5.8,6.1,6.4,5.6,5.1,5.6,6.1,5.6,5.5,4.8,5.4,5.6,5.1,5.1,5.9,5.7,5.2,5,5.2,5.4,5.1],"Petal.Width":[0.2,0.2,0.2,0.2,0.2,0.4,0.3,0.2,0.2,0.1,0.2,0.2,0.1,0.1,0.2,0.4,0.4,0.3,0.3,0.3,0.2,0.4,0.2,0.5,0.2,0.2,0.4,0.2,0.2,0.2,0.2,0.4,0.1,0.2,0.2,0.2,0.2,0.1,0.2,0.2,0.3,0.3,0.2,0.6,0.4,0.3,0.2,0.2,0.2,0.2,1.4,1.5,1.5,1.3,1.5,1.3,1.6,1,1.3,1.4,1,1.5,1,1.4,1.3,1.4,1.5,1,1.5,1.1,1.8,1.3,1.5,1.2,1.3,1.4,1.4,1.7,1.5,1,1.1,1,1.2,1.6,1.5,1.6,1.5,1.3,1.3,1.3,1.2,1.4,1.2,1,1.3,1.2,1.3,1.3,1.1,1.3,2.5,1.9,2.1,1.8,2.2,2.1,1.7,1.8,1.8,2.5,2,1.9,2.1,2,2.4,2.3,1.8,2.2,2.3,1.5,2.3,2,2,1.8,2.1,1.8,1.8,1.8,2.1,1.6,1.9,2,2.2,1.5,1.4,2.3,2.4,1.8,1.8,2.1,2.4,2.3,1.9,2.3,2.5,2.3,1.9,2,2.3,1.8],"Species":["setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","setosa","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","versicolor","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica","virginica"]},"columns":[{"id":"Sepal.Length","name":"Sepal.Length","type":"numeric"},{"id":"Sepal.Width","name":"Sepal.Width","type":"numeric"},{"id":"Petal.Length","name":"Petal.Length","type":"numeric"},{"id":"Petal.Width","name":"Petal.Width","type":"numeric"},{"id":"Species","name":"Species","type":"factor"}],"dataKey":"1980abf4c53c6ff35ad17d6d5d0650a0"},"children":[]},"class":"reactR_markup"},"evals":[],"jsHooks":[]}</script>

Pero se pueden hacer tablas tan fabulosas como [esta](https://glin.github.io/reactable/articles/twitter-followers/twitter-followers.html) o [esta](https://glin.github.io/reactable/articles/nba-box-score/nba-box-score.html) o [esta](https://glin.github.io/reactable/articles/womens-world-cup/womens-world-cup.html).

<br>

------------------------------------------------------------------------

## 5.3 `rpivotTable` package

> The rpivotTable package is an R htmlwidget built around the pivottable JS library.

El paquete [`rpivotTable`](https://github.com/smartinsightsfromdata/rpivotTable) genera tablas que permiten al usuario generar sus propios resultados.

Como las tablas que genera el paquete `rpivotTable` pueden, seg??n las opciones que utilice el usuario de la tabla, cambiar mucho de tama??o, voy a poner un ejemplo de esta tabla pero al final de este documento, despu??s de la bibliograf??a.

Crear una tabla con `rpivotTable` es muy sencillo. Pod??is verla tabla al final del documento.

``` r
library(rpivotTable) #- remotes::install_github(c("ramnathv/htmlwidgets", "smartinsightsfromdata/rpivotTable"))
rpivotTable(df, rows = "Gender", cols = c("Country"), width = "100%", height = "400px")
```

<br>

------------------------------------------------------------------------

<br>

# 6. Tablas para modelos

R es un lenguaje/entorno para hacer an??lisis estad??sticos, as?? que muchas veces se han de presentar los resultados de estimaci??n de alg??n modelo estad??stico, PERO, los resultados de estimaci??n de estos modelos, en general, no se almacenan en data.frames, sino en listas. ??Es esto importante? S??, si lo queremos es presentar los resultados de estimaci??n en una tabla. La raz??n consiste en que los paquetes para tablas que hemos visto anteriormente (`gt`, `DT`, etc ???) solo generan tablas de resultados almacenados en data.frames, as?? que no los podremos usar, al menos directamente, para hacer tablas de resultados asociados a modelos estad??sticos. Afortunadamente hay unos cuantos paquetes en R cuyo prop??sito es precisamente ese, presentar los resultados de estimaci??n de alg??n modelo o t??cnica estad??stica como tablas.

Por ejemplo, vamos a estimar un modelo de regresi??n lineal. Utilizaremos estos datos:

``` r
urla <- "https://raw.githubusercontent.com/perezp44/iris_data/master/data/PIAAC_data_small.csv"
df <- read_csv(urla)
```

Con ellos estimamos el siguiente modelo lineal:

``` r
my_model <- lm(Wage_hour ~ Numeracy_score + Gender , data = df)
my_model
#> 
#> Call:
#> lm(formula = Wage_hour ~ Numeracy_score + Gender, data = df)
#> 
#> Coefficients:
#>    (Intercept)  Numeracy_score      GenderMale  
#>        3.46022         0.02988         0.52874
```

Generalmente hay funciones espec??ficas para mostrar los resultados de estimaci??n, por ejemplo la funci??n `summary()`:

``` r
summary(my_model)
#> 
#> Call:
#> lm(formula = Wage_hour ~ Numeracy_score + Gender, data = df)
#> 
#> Residuals:
#>     Min      1Q  Median      3Q     Max 
#> -10.903  -3.453  -1.059   2.097 104.179 
#> 
#> Coefficients:
#>                Estimate Std. Error t value             Pr(>|t|)    
#> (Intercept)    3.460222   0.351822   9.835 < 0.0000000000000002 ***
#> Numeracy_score 0.029881   0.001325  22.554 < 0.0000000000000002 ***
#> GenderMale     0.528745   0.134064   3.944            0.0000808 ***
#> ---
#> Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
#> 
#> Residual standard error: 5.973 on 7992 degrees of freedom
#>   (27 observations deleted due to missingness)
#> Multiple R-squared:  0.06324,	Adjusted R-squared:  0.063 
#> F-statistic: 269.8 on 2 and 7992 DF,  p-value: < 0.00000000000000022
```

Los resultados mostrados por `summary()` permiten hacerse una idea de los resultados de la estimaci??n pero no suelen ser adecuados para presentarlos en un informe o en un art??culo cient??fico.

Hay bastantes paquetes que permiten obtener tablas con los resultados de la estimaci??n de modelos estad??sticos, por ejemplo, el paquete [`finalfit`](https://www.datasurg.net/2018/05/16/elegant-regression-results-tables-and-plots-the-finalfit-package/) y muchos otros, sin embargo, en este tutorial solo se mostrar?? alg??n ejemplo para los paquetes [`stargazer`](https://cran.r-project.org/web/packages/stargazer/stargazer.pdf), [`modelsummary`](https://github.com/vincentarelbundock/modelsummary), [`gtsummary`](https://github.com/zabore/gtsummary) y [`sjPlot`](https://strengejacke.github.io/sjPlot/index.html)

------------------------------------------------------------------------

<br>

## 6.1 Tablas con `stargazer`

El paquete [`stargazer`](https://cran.r-project.org/web/packages/stargazer/vignettes/stargazer.pdf) permite f??cilmente presentar tablas con resultados de regresi??n. Permite crear tablas en latex, html o ascii. [Aqu??](https://www.jakeruss.com/cheatsheets/stargazer/) hay una cheatsheet sobre `stargazer`

``` r
stargazer::stargazer(my_model, type = "html")
```

<table style="text-align:center">
<tr>
<td colspan="2" style="border-bottom: 1px solid black">
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
<em>Dependent variable:</em>
</td>
</tr>
<tr>
<td>
</td>
<td colspan="1" style="border-bottom: 1px solid black">
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
Wage_hour
</td>
</tr>
<tr>
<td colspan="2" style="border-bottom: 1px solid black">
</td>
</tr>
<tr>
<td style="text-align:left">
Numeracy_score
</td>
<td>
0.030<sup>\*\*\*</sup>
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
(0.001)
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
</td>
</tr>
<tr>
<td style="text-align:left">
GenderMale
</td>
<td>
0.529<sup>\*\*\*</sup>
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
(0.134)
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
</td>
</tr>
<tr>
<td style="text-align:left">
Constant
</td>
<td>
3.460<sup>\*\*\*</sup>
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
(0.352)
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
</td>
</tr>
<tr>
<td colspan="2" style="border-bottom: 1px solid black">
</td>
</tr>
<tr>
<td style="text-align:left">
Observations
</td>
<td>
7,995
</td>
</tr>
<tr>
<td style="text-align:left">
R<sup>2</sup>
</td>
<td>
0.063
</td>
</tr>
<tr>
<td style="text-align:left">
Adjusted R<sup>2</sup>
</td>
<td>
0.063
</td>
</tr>
<tr>
<td style="text-align:left">
Residual Std. Error
</td>
<td>
5.973 (df = 7992)
</td>
</tr>
<tr>
<td style="text-align:left">
F Statistic
</td>
<td>
269.760<sup>\*\*\*</sup> (df = 2; 7992)
</td>
</tr>
<tr>
<td colspan="2" style="border-bottom: 1px solid black">
</td>
</tr>
<tr>
<td style="text-align:left">
<em>Note:</em>
</td>
<td style="text-align:right">
<sup>*</sup>p\<0.1; <sup>**</sup>p\<0.05; <sup>***</sup>p\<0.01
</td>
</tr>
</table>

<br>

Se pueden presentar los resultados de varios modelos en una tabla. Ve??moslo. Para ello vamos a estimar tres modelos y los almacenaremos en una lista:

``` r
df <- df %>% mutate(Numeracy_score_b = ifelse(Numeracy_score > mean(Numeracy_score, na.rm = TRUE), 1, 0)) #- binary variable for logit model

my_models <- list()
my_models[['W:  OLS 1']]   <- lm( Wage_hour         ~ Numeracy_score + Gender , df)
my_models[['Nu: OLS 2']]   <- lm( Numeracy_score    ~ Education + Gender , df)
my_models[['Nu: Logit 1']] <- glm( Numeracy_score_b ~ Education + Gender , df, family = binomial())
```

Una vez hemos estimado los 3 modelos y almacenado sus resultados de estimaci??n en la lista `my_models`

``` r
stargazer::stargazer(my_models, type = "html", title = "Results", align = TRUE)
```

<table style="text-align:center">
<caption>
<strong>Results</strong>
</caption>
<tr>
<td colspan="4" style="border-bottom: 1px solid black">
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td colspan="3">
<em>Dependent variable:</em>
</td>
</tr>
<tr>
<td>
</td>
<td colspan="3" style="border-bottom: 1px solid black">
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
Wage_hour
</td>
<td>
Numeracy_score
</td>
<td>
Numeracy_score_b
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
<em>OLS</em>
</td>
<td>
<em>OLS</em>
</td>
<td>
<em>logistic</em>
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
\(1\)
</td>
<td>
\(2\)
</td>
<td>
\(3\)
</td>
</tr>
<tr>
<td colspan="4" style="border-bottom: 1px solid black">
</td>
</tr>
<tr>
<td style="text-align:left">
Numeracy_score
</td>
<td>
0.030<sup>\*\*\*</sup>
</td>
<td>
</td>
<td>
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
(0.001)
</td>
<td>
</td>
<td>
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
</td>
<td>
</td>
<td>
</td>
</tr>
<tr>
<td style="text-align:left">
EducationSecondary
</td>
<td>
</td>
<td>
46.752<sup>\*\*\*</sup>
</td>
<td>
1.788<sup>\*\*\*</sup>
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
</td>
<td>
(1.983)
</td>
<td>
(0.134)
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
</td>
<td>
</td>
<td>
</td>
</tr>
<tr>
<td style="text-align:left">
EducationTertiary
</td>
<td>
</td>
<td>
89.531<sup>\*\*\*</sup>
</td>
<td>
3.424<sup>\*\*\*</sup>
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
</td>
<td>
(2.137)
</td>
<td>
(0.143)
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
</td>
<td>
</td>
<td>
</td>
</tr>
<tr>
<td style="text-align:left">
EducationUpper_second
</td>
<td>
</td>
<td>
75.903<sup>\*\*\*</sup>
</td>
<td>
2.857<sup>\*\*\*</sup>
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
</td>
<td>
(2.388)
</td>
<td>
(0.150)
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
</td>
<td>
</td>
<td>
</td>
</tr>
<tr>
<td style="text-align:left">
GenderMale
</td>
<td>
0.529<sup>\*\*\*</sup>
</td>
<td>
12.947<sup>\*\*\*</sup>
</td>
<td>
0.448<sup>\*\*\*</sup>
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
(0.134)
</td>
<td>
(1.000)
</td>
<td>
(0.049)
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
</td>
<td>
</td>
<td>
</td>
</tr>
<tr>
<td style="text-align:left">
Constant
</td>
<td>
3.460<sup>\*\*\*</sup>
</td>
<td>
196.447<sup>\*\*\*</sup>
</td>
<td>
-2.270<sup>\*\*\*</sup>
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
(0.352)
</td>
<td>
(1.955)
</td>
<td>
(0.134)
</td>
</tr>
<tr>
<td style="text-align:left">
</td>
<td>
</td>
<td>
</td>
<td>
</td>
</tr>
<tr>
<td colspan="4" style="border-bottom: 1px solid black">
</td>
</tr>
<tr>
<td style="text-align:left">
Observations
</td>
<td>
7,995
</td>
<td>
8,014
</td>
<td>
8,014
</td>
</tr>
<tr>
<td style="text-align:left">
R<sup>2</sup>
</td>
<td>
0.063
</td>
<td>
0.229
</td>
<td>
</td>
</tr>
<tr>
<td style="text-align:left">
Adjusted R<sup>2</sup>
</td>
<td>
0.063
</td>
<td>
0.229
</td>
<td>
</td>
</tr>
<tr>
<td style="text-align:left">
Log Likelihood
</td>
<td>
</td>
<td>
</td>
<td>
-4,894.853
</td>
</tr>
<tr>
<td style="text-align:left">
Akaike Inf. Crit.
</td>
<td>
</td>
<td>
</td>
<td>
9,799.706
</td>
</tr>
<tr>
<td style="text-align:left">
Residual Std. Error
</td>
<td>
5.973 (df = 7992)
</td>
<td>
44.382 (df = 8009)
</td>
<td>
</td>
</tr>
<tr>
<td style="text-align:left">
F Statistic
</td>
<td>
269.760<sup>\*\*\*</sup> (df = 2; 7992)
</td>
<td>
596.336<sup>\*\*\*</sup> (df = 4; 8009)
</td>
<td>
</td>
</tr>
<tr>
<td colspan="4" style="border-bottom: 1px solid black">
</td>
</tr>
<tr>
<td style="text-align:left">
<em>Note:</em>
</td>
<td colspan="3" style="text-align:right">
<sup>*</sup>p\<0.1; <sup>**</sup>p\<0.05; <sup>***</sup>p\<0.01
</td>
</tr>
</table>

------------------------------------------------------------------------

<br>

## 6.2 Tablas con `modelsummary`

El paquete [`modelsummary`](https://vincentarelbundock.github.io/modelsummary/) es m??s moderno, y tambi??n permite hacer tablas resumen de estimaciones de modelos. Por ejemplo:

``` r
library(modelsummary) #- remotes::install_github('vincentarelbundock/modelsummary')

mm <- modelsummary::msummary(my_models, title = "Resultados de estimaci??n")
mm
```

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
<caption>
Table 2: Resultados de estimaci??n
</caption>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:center;">
W: OLS 1
</th>
<th style="text-align:center;">
??Nu: OLS 2
</th>
<th style="text-align:center;">
Nu: Logit 1
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
(Intercept)
</td>
<td style="text-align:center;">
3.460
</td>
<td style="text-align:center;">
196.447
</td>
<td style="text-align:center;">
-2.270
</td>
</tr>
<tr>
<td style="text-align:left;">
</td>
<td style="text-align:center;">
(0.352)
</td>
<td style="text-align:center;">
(1.955)
</td>
<td style="text-align:center;">
(0.134)
</td>
</tr>
<tr>
<td style="text-align:left;">
Numeracy_score
</td>
<td style="text-align:center;">
0.030
</td>
<td style="text-align:center;">
</td>
<td style="text-align:center;">
</td>
</tr>
<tr>
<td style="text-align:left;">
</td>
<td style="text-align:center;">
(0.001)
</td>
<td style="text-align:center;">
</td>
<td style="text-align:center;">
</td>
</tr>
<tr>
<td style="text-align:left;">
GenderMale
</td>
<td style="text-align:center;">
0.529
</td>
<td style="text-align:center;">
12.947
</td>
<td style="text-align:center;">
0.448
</td>
</tr>
<tr>
<td style="text-align:left;">
</td>
<td style="text-align:center;">
(0.134)
</td>
<td style="text-align:center;">
(1.000)
</td>
<td style="text-align:center;">
(0.049)
</td>
</tr>
<tr>
<td style="text-align:left;">
EducationSecondary
</td>
<td style="text-align:center;">
</td>
<td style="text-align:center;">
46.752
</td>
<td style="text-align:center;">
1.788
</td>
</tr>
<tr>
<td style="text-align:left;">
</td>
<td style="text-align:center;">
</td>
<td style="text-align:center;">
(1.983)
</td>
<td style="text-align:center;">
(0.134)
</td>
</tr>
<tr>
<td style="text-align:left;">
EducationTertiary
</td>
<td style="text-align:center;">
</td>
<td style="text-align:center;">
89.531
</td>
<td style="text-align:center;">
3.424
</td>
</tr>
<tr>
<td style="text-align:left;">
</td>
<td style="text-align:center;">
</td>
<td style="text-align:center;">
(2.137)
</td>
<td style="text-align:center;">
(0.143)
</td>
</tr>
<tr>
<td style="text-align:left;">
EducationUpper_second
</td>
<td style="text-align:center;">
</td>
<td style="text-align:center;">
75.903
</td>
<td style="text-align:center;">
2.857
</td>
</tr>
<tr>
<td style="text-align:left;box-shadow: 0px 1px">
</td>
<td style="text-align:center;box-shadow: 0px 1px">
</td>
<td style="text-align:center;box-shadow: 0px 1px">
(2.388)
</td>
<td style="text-align:center;box-shadow: 0px 1px">
(0.150)
</td>
</tr>
<tr>
<td style="text-align:left;">
Num.Obs.
</td>
<td style="text-align:center;">
7995
</td>
<td style="text-align:center;">
8014
</td>
<td style="text-align:center;">
8014
</td>
</tr>
<tr>
<td style="text-align:left;">
R2
</td>
<td style="text-align:center;">
0.063
</td>
<td style="text-align:center;">
0.229
</td>
<td style="text-align:center;">
</td>
</tr>
<tr>
<td style="text-align:left;">
R2 Adj.
</td>
<td style="text-align:center;">
0.063
</td>
<td style="text-align:center;">
0.229
</td>
<td style="text-align:center;">
</td>
</tr>
<tr>
<td style="text-align:left;">
AIC
</td>
<td style="text-align:center;">
51272.9
</td>
<td style="text-align:center;">
83541.3
</td>
<td style="text-align:center;">
9799.7
</td>
</tr>
<tr>
<td style="text-align:left;">
BIC
</td>
<td style="text-align:center;">
51300.8
</td>
<td style="text-align:center;">
83583.2
</td>
<td style="text-align:center;">
9834.7
</td>
</tr>
<tr>
<td style="text-align:left;">
Log.Lik.
</td>
<td style="text-align:center;">
-25632.432
</td>
<td style="text-align:center;">
-41764.631
</td>
<td style="text-align:center;">
-4894.853
</td>
</tr>
<tr>
<td style="text-align:left;">
RMSE
</td>
<td style="text-align:center;">
5.97
</td>
<td style="text-align:center;">
44.37
</td>
<td style="text-align:center;">
0.46
</td>
</tr>
</tbody>
</table>

Tiene muchas m??s posibilidades.

------------------------------------------------------------------------

<br>

## 6.3 Tablas con `gtsummary`

El paquete [`gtsummary`](https://github.com/zabore/gtsummary) permite, adem??s de realizar tablas resumen de data.frames, confeccionar tablas de modelos de regresi??n de forma sencilla y muy configurables.

Como he dicho `gtsummary` tiene muchas posibilidades, algunas de ellas puedes verlas en este [video](https://youtu.be/U2S6LbMN42I), en estas [transparencias](https://www.emilyzabor.com/cleveland-r-gtsummary/), o en este [post](https://education.rstudio.com/blog/2020/07/gtsummary/).

Como ejemplos de su uso, una tabla resumen de un data.frame:

``` r
iris %>% gtsummary::tbl_summary()
```

<div id="radwfjercb" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#radwfjercb .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#radwfjercb .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#radwfjercb .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#radwfjercb .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#radwfjercb .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#radwfjercb .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#radwfjercb .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#radwfjercb .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#radwfjercb .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#radwfjercb .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#radwfjercb .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#radwfjercb .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#radwfjercb .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#radwfjercb .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#radwfjercb .gt_from_md > :first-child {
  margin-top: 0;
}

#radwfjercb .gt_from_md > :last-child {
  margin-bottom: 0;
}

#radwfjercb .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#radwfjercb .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#radwfjercb .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#radwfjercb .gt_row_group_first td {
  border-top-width: 2px;
}

#radwfjercb .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#radwfjercb .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#radwfjercb .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#radwfjercb .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#radwfjercb .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#radwfjercb .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#radwfjercb .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#radwfjercb .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#radwfjercb .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#radwfjercb .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-left: 4px;
  padding-right: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#radwfjercb .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#radwfjercb .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#radwfjercb .gt_left {
  text-align: left;
}

#radwfjercb .gt_center {
  text-align: center;
}

#radwfjercb .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#radwfjercb .gt_font_normal {
  font-weight: normal;
}

#radwfjercb .gt_font_bold {
  font-weight: bold;
}

#radwfjercb .gt_font_italic {
  font-style: italic;
}

#radwfjercb .gt_super {
  font-size: 65%;
}

#radwfjercb .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 75%;
  vertical-align: 0.4em;
}

#radwfjercb .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#radwfjercb .gt_indent_1 {
  text-indent: 5px;
}

#radwfjercb .gt_indent_2 {
  text-indent: 10px;
}

#radwfjercb .gt_indent_3 {
  text-indent: 15px;
}

#radwfjercb .gt_indent_4 {
  text-indent: 20px;
}

#radwfjercb .gt_indent_5 {
  text-indent: 25px;
}
</style>
<table class="gt_table">
  
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="&lt;strong&gt;Characteristic&lt;/strong&gt;"><strong>Characteristic</strong></th>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1" scope="col" id="&lt;strong&gt;N = 150&lt;/strong&gt;&lt;sup class=&quot;gt_footnote_marks&quot;&gt;1&lt;/sup&gt;"><strong>N = 150</strong><sup class="gt_footnote_marks">1</sup></th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="label" class="gt_row gt_left">Sepal.Length</td>
<td headers="stat_0" class="gt_row gt_center">5.80 (5.10, 6.40)</td></tr>
    <tr><td headers="label" class="gt_row gt_left">Sepal.Width</td>
<td headers="stat_0" class="gt_row gt_center">3.00 (2.80, 3.30)</td></tr>
    <tr><td headers="label" class="gt_row gt_left">Petal.Length</td>
<td headers="stat_0" class="gt_row gt_center">4.35 (1.60, 5.10)</td></tr>
    <tr><td headers="label" class="gt_row gt_left">Petal.Width</td>
<td headers="stat_0" class="gt_row gt_center">1.30 (0.30, 1.80)</td></tr>
    <tr><td headers="label" class="gt_row gt_left">Species</td>
<td headers="stat_0" class="gt_row gt_center"></td></tr>
    <tr><td headers="label" class="gt_row gt_left">????????setosa</td>
<td headers="stat_0" class="gt_row gt_center">50 (33%)</td></tr>
    <tr><td headers="label" class="gt_row gt_left">????????versicolor</td>
<td headers="stat_0" class="gt_row gt_center">50 (33%)</td></tr>
    <tr><td headers="label" class="gt_row gt_left">????????virginica</td>
<td headers="stat_0" class="gt_row gt_center">50 (33%)</td></tr>
  </tbody>
  
  <tfoot class="gt_footnotes">
    <tr>
      <td class="gt_footnote" colspan="2"><sup class="gt_footnote_marks">1</sup> Median (IQR); n (%)</td>
    </tr>
  </tfoot>
</table>
</div>

<br>

Ahora una tabla de un modelo de regresi??n:

``` r
gtsummary::tbl_regression(my_model)
```

<div id="egfipaypff" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#egfipaypff .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#egfipaypff .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#egfipaypff .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}

#egfipaypff .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#egfipaypff .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#egfipaypff .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#egfipaypff .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#egfipaypff .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#egfipaypff .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#egfipaypff .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#egfipaypff .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#egfipaypff .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#egfipaypff .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}

#egfipaypff .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#egfipaypff .gt_from_md > :first-child {
  margin-top: 0;
}

#egfipaypff .gt_from_md > :last-child {
  margin-bottom: 0;
}

#egfipaypff .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#egfipaypff .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
}

#egfipaypff .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}

#egfipaypff .gt_row_group_first td {
  border-top-width: 2px;
}

#egfipaypff .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#egfipaypff .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}

#egfipaypff .gt_first_summary_row.thick {
  border-top-width: 2px;
}

#egfipaypff .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#egfipaypff .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#egfipaypff .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#egfipaypff .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#egfipaypff .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#egfipaypff .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#egfipaypff .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-left: 4px;
  padding-right: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#egfipaypff .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#egfipaypff .gt_sourcenote {
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}

#egfipaypff .gt_left {
  text-align: left;
}

#egfipaypff .gt_center {
  text-align: center;
}

#egfipaypff .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#egfipaypff .gt_font_normal {
  font-weight: normal;
}

#egfipaypff .gt_font_bold {
  font-weight: bold;
}

#egfipaypff .gt_font_italic {
  font-style: italic;
}

#egfipaypff .gt_super {
  font-size: 65%;
}

#egfipaypff .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 75%;
  vertical-align: 0.4em;
}

#egfipaypff .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}

#egfipaypff .gt_indent_1 {
  text-indent: 5px;
}

#egfipaypff .gt_indent_2 {
  text-indent: 10px;
}

#egfipaypff .gt_indent_3 {
  text-indent: 15px;
}

#egfipaypff .gt_indent_4 {
  text-indent: 20px;
}

#egfipaypff .gt_indent_5 {
  text-indent: 25px;
}
</style>
<table class="gt_table">
  
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="&lt;strong&gt;Characteristic&lt;/strong&gt;"><strong>Characteristic</strong></th>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1" scope="col" id="&lt;strong&gt;Beta&lt;/strong&gt;"><strong>Beta</strong></th>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1" scope="col" id="&lt;strong&gt;95% CI&lt;/strong&gt;&lt;sup class=&quot;gt_footnote_marks&quot;&gt;1&lt;/sup&gt;"><strong>95% CI</strong><sup class="gt_footnote_marks">1</sup></th>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1" scope="col" id="&lt;strong&gt;p-value&lt;/strong&gt;"><strong>p-value</strong></th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="label" class="gt_row gt_left">Numeracy_score</td>
<td headers="estimate" class="gt_row gt_center">0.03</td>
<td headers="ci" class="gt_row gt_center">0.03, 0.03</td>
<td headers="p.value" class="gt_row gt_center"><0.001</td></tr>
    <tr><td headers="label" class="gt_row gt_left">Gender</td>
<td headers="estimate" class="gt_row gt_center"></td>
<td headers="ci" class="gt_row gt_center"></td>
<td headers="p.value" class="gt_row gt_center"></td></tr>
    <tr><td headers="label" class="gt_row gt_left">????????Female</td>
<td headers="estimate" class="gt_row gt_center">???</td>
<td headers="ci" class="gt_row gt_center">???</td>
<td headers="p.value" class="gt_row gt_center"></td></tr>
    <tr><td headers="label" class="gt_row gt_left">????????Male</td>
<td headers="estimate" class="gt_row gt_center">0.53</td>
<td headers="ci" class="gt_row gt_center">0.27, 0.79</td>
<td headers="p.value" class="gt_row gt_center"><0.001</td></tr>
  </tbody>
  
  <tfoot class="gt_footnotes">
    <tr>
      <td class="gt_footnote" colspan="4"><sup class="gt_footnote_marks">1</sup> CI = Confidence Interval</td>
    </tr>
  </tfoot>
</table>
</div>

------------------------------------------------------------------------

<br>

## 6.4 Tablas con `sjPlot`

El paquete [`sjPlot`](https://strengejacke.github.io/sjPlot/) tiene muchas posibilidades, pero en concreto puede hacer tablas de modelos:

``` r
#sjPlot::tab_model(my_model)
```

Tiene otras utilidades, por ejemplo:

``` r
#sjPlot::plot_model(my_model)
```

------------------------------------------------------------------------

<br>

## 6.5 Otros paquetes

Hay muchos m??s paquetes especializados en hacer tablas con resultados de la estimaci??n de modelos. Aqu?? solo mostrar?? algo de 3 de ellos, los paquetes `report` y `apaTables`, pero existen otros paquetes como:

- [`flipRegression`](https://github.com/Displayr/flipRegression). En [este post](https://www.displayr.com/5-alternatives-to-the-default-r-outputs-for-glms-and-linear-models/) explican como usar sus funciones.

- [`papaja`](https://github.com/crsh/papaja), es un paquete para producir documentos y tablas conformes a la American Psychological Association (APA) manuscript guidelines (6th Edition).

- [`academicWriteR`](https://www.jvcasillas.com/academicWriteR/), est?? relacionado con `papaja`. Es un paquete con algunas funciones ??tiles para escribir informes estad??sticos. Por ejemplo la funci??n `count_word()`.

<br>

### paquete `report`

Seg??n pone en su [p??gina web](https://easystats.github.io/report/):

> It automatically produces reports of models and dataframes according to best practice guidelines (e.g., APA???s style guide), ensuring standardization and quality in results reporting.

``` r
library(report) #- devtools::install_github("neuropsychology/report")
rr <- report(my_model)
```

<br>

``` r
as.report_table(rr)
#> Parameter      | Coefficient |       95% CI | t(7992) |      p | Std. Coef. | Std. Coef. 95% CI |      Fit
#> ----------------------------------------------------------------------------------------------------------
#> (Intercept)    |        3.46 | [2.77, 4.15] |    9.84 | < .001 |      -0.04 |    [-0.07, -0.01] |         
#> Numeracy score |        0.03 | [0.03, 0.03] |   22.55 | < .001 |       0.24 |    [ 0.22,  0.27] |         
#> Gender [Male]  |        0.53 | [0.27, 0.79] |    3.94 | < .001 |       0.09 |    [ 0.04,  0.13] |         
#>                |             |              |         |        |            |                   |         
#> AIC            |             |              |         |        |            |                   | 51272.86
#> AICc           |             |              |         |        |            |                   | 51272.87
#> BIC            |             |              |         |        |            |                   | 51300.81
#> R2             |             |              |         |        |            |                   |     0.06
#> R2 (adj.)      |             |              |         |        |            |                   |     0.06
#> Sigma          |             |              |         |        |            |                   |     5.97
```

<br>

Tambi??n permite obtener una descripci??n verbal de los resultados en texto:

``` r
as.report_text(rr)
#> We fitted a linear model (estimated using OLS) to predict Wage_hour with
#> Numeracy_score (formula: Wage_hour ~ Numeracy_score + Gender). The model
#> explains a statistically significant and weak proportion of variance (R2 =
#> 0.06, F(2, 7992) = 269.76, p < .001, adj. R2 = 0.06). The model's intercept,
#> corresponding to Numeracy_score = 0, is at 3.46 (95% CI [2.77, 4.15], t(7992) =
#> 9.84, p < .001). Within this model:
#> 
#>   - The effect of Numeracy score is statistically significant and positive (beta
#> = 0.03, 95% CI [0.03, 0.03], t(7992) = 22.55, p < .001; Std. beta = 0.24, 95%
#> CI [0.22, 0.27])
#>   - The effect of Gender [Male] is statistically significant and positive (beta =
#> 0.53, 95% CI [0.27, 0.79], t(7992) = 3.94, p < .001; Std. beta = 0.09, 95% CI
#> [0.04, 0.13])
#> 
#> Standardized parameters were obtained by fitting the model on a standardized
#> version of the dataset. 95% Confidence Intervals (CIs) and p-values were
#> computed using a Wald t-distribution approximation. and We fitted a linear
#> model (estimated using OLS) to predict Wage_hour with Gender (formula:
#> Wage_hour ~ Numeracy_score + Gender). The model explains a statistically
#> significant and weak proportion of variance (R2 = 0.06, F(2, 7992) = 269.76, p
#> < .001, adj. R2 = 0.06). The model's intercept, corresponding to Gender =
#> Female, is at 3.46 (95% CI [2.77, 4.15], t(7992) = 9.84, p < .001). Within this
#> model:
#> 
#>   - The effect of Numeracy score is statistically significant and positive (beta
#> = 0.03, 95% CI [0.03, 0.03], t(7992) = 22.55, p < .001; Std. beta = 0.24, 95%
#> CI [0.22, 0.27])
#>   - The effect of Gender [Male] is statistically significant and positive (beta =
#> 0.53, 95% CI [0.27, 0.79], t(7992) = 3.94, p < .001; Std. beta = 0.09, 95% CI
#> [0.04, 0.13])
#> 
#> Standardized parameters were obtained by fitting the model on a standardized
#> version of the dataset. 95% Confidence Intervals (CIs) and p-values were
#> computed using a Wald t-distribution approximation.
```

<br>

### paquete `apaTables`

Seg??n su [p??gina web](https://dstanley4.github.io/apaTables/index.html):

> This package creates Word files (.doc files) containing APA style tables for several types of analyses. Using this package minimizes transcription errors and reduces the number commands needed by the user.

``` r
library(apaTables) #- install.packages("apaTables",dep = TRUE)
apa.reg.table(my_model)
```

<br>

------------------------------------------------------------------------

<br>

# 7. Bibliograf??a/Recursos:

- En [este hilo](https://twitter.com/GoldbergData/status/1292935454195511302) de Twitter se habla sobre los mejores paquetes R para hacer tablas.

- [David Keyes](https://rfortherestofus.com/author/dgkeyes/) se??ala [aqu??](https://rfortherestofus.com/2019/11/how-to-make-beautiful-tables-in-r/), que quieres hacer tablas para Word, posiblemente la mejor opci??n sea el paquete [flextable](https://davidgohel.github.io/flextable/index.html)

- Si lo que necesitas es hacer tablas para documentos pdf, puedes empezar por [aqu??](https://sharleenw.rbind.io/post/tables_in_pdf/making-pdf-tables-in-r/). Al final remite a [este otro documento](https://haozhu233.github.io/kableExtra/awesome_table_in_pdf.pdf). Tambi??n puedes usar este [generador de tablas](https://www.tablesgenerator.com/).

- Si quieres tablas de porcentajes etc??? [aqu??](https://dabblingwithdata.wordpress.com/2017/12/20/my-favourite-r-package-for-frequency-tables/) plantean varias posibilidades para hacerlas.

- Si quieres hacer tablas parecidas a las que se hacen con PROC FREQ de SAS o CROSSTABS en SPSS puedes usar la funci??n `CrossTable()` del paquete `gmodels`. En [este post](https://dabblingwithdata.wordpress.com/2018/02/26/r-packages-for-summarising-data-part-2/) muestran otras alternativas.

- Si necesitas hacer **3-way tables**, puedes hacerlas con `stats::xtabs()`. Para despu??s imprimirla con `ftable(my_table)`. Lo explican[aqu??](https://rstudio-pubs-static.s3.amazonaws.com/308591_6dff566d383946c881cb5b6a735a79fd.html) y [aqu??](https://www.statmethods.net/stats/frequencies.html). Por ejemplo:

``` r
my_table <- stats::xtabs(~ Education + Country + Gender, data = df)
stats::ftable(my_table) 
```

Otra alternativa para tablas de frecuencias de 3 variables es usar `janitor::tabyl(X1, X2, X3)`. Lo explican [aqu??](https://cran.r-project.org/web/packages/janitor/vignettes/tabyls.html)

``` r
df %>% janitor::tabyl(Education, Country, Gender)
```

- M??s paquetes relacionados con tablas: [printr](https://yihui.name/printr/), [questionr](https://juba.github.io/questionr/), ???

- Los paquetes [`rhandsontable`](https://jrowen.github.io/rhandsontable/) y [`excelR`](https://swechhya.github.io/excelR/) permiten crear tablas editables por el usuario.

- El paquete [`expss`](https://cran.r-project.org/web/packages/expss/vignettes/tables-with-labels.html) hace tablas similares a las de SPSS.

- En este [post](https://appsilon.com/forget-about-excel-use-r-shiny-packages-instead/) hacen un repaso de paquetes que permiten crear tablas con caracter??sticas especiales como que sus valores sean editables por el usuario, que tengan formato condicionado a los valores de las tablas, que se puedan ordenar y filtrar sus valores etc ???

- Un [post](https://blog.rstudio.com/2020/12/23/winners-of-the-2020-rstudio-table-contest/) con las tablas ganadoras del ???2020 RStudio Table Contest???.

<br><br>

------------------------------------------------------------------------

<br>

# 5.3 Drag & drop pivot tables: `rpivotTable`

El paquete [`rpivotTable`](https://github.com/smartinsightsfromdata/rpivotTable):

> The rpivotTable package is an R htmlwidget built around the pivottable library.

<br>

``` r
rpivotTable::rpivotTable(df, rows = "Gender", cols = c("Country"), width = "100%", height = "400px")
```

<div id="htmlwidget-5" style="width:100%;height:400px;" class="rpivotTable html-widget"></div>
<script type="application/json" data-for="htmlwidget-5">{"x":{"data":{"Country":["ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","ESP","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","FRA","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","GBR","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA","ITA"],"Gender":["Male","Female","Female","Female","Female","Male","Female","Female","Female","Male","Male","Female","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Female","Female","Female","Female","Male","Male","Female","Male","Male","Male","Female","Male","Male","Male","Male","Male","Male","Female","Female","Male","Female","Male","Female","Male","Female","Female","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Male","Male","Male","Male","Male","Female","Male","Male","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Male","Male","Female","Female","Female","Male","Male","Male","Female","Male","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Male","Male","Male","Female","Male","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Male","Male","Female","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Male","Female","Male","Female","Male","Female","Male","Female","Male","Female","Male","Male","Male","Female","Male","Female","Female","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Female","Female","Male","Female","Male","Male","Female","Male","Male","Female","Male","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Female","Female","Male","Female","Female","Male","Male","Female","Female","Male","Male","Male","Female","Male","Female","Male","Female","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Male","Male","Male","Male","Male","Female","Female","Female","Male","Male","Male","Female","Female","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Male","Male","Male","Female","Female","Female","Female","Male","Female","Female","Male","Female","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Female","Male","Male","Female","Male","Male","Female","Female","Female","Female","Male","Female","Female","Male","Female","Female","Male","Female","Male","Male","Male","Female","Female","Female","Male","Female","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Female","Female","Female","Male","Female","Male","Female","Female","Male","Male","Male","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Female","Male","Male","Male","Male","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Female","Male","Male","Male","Female","Male","Female","Male","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Female","Male","Male","Male","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Male","Male","Male","Male","Male","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Female","Male","Male","Female","Female","Female","Female","Male","Male","Female","Male","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Female","Male","Female","Male","Male","Female","Female","Male","Male","Male","Male","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Female","Female","Female","Female","Male","Female","Male","Male","Male","Male","Female","Female","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Male","Male","Male","Female","Male","Male","Female","Male","Female","Male","Female","Male","Female","Male","Male","Male","Female","Male","Female","Male","Male","Female","Male","Female","Male","Male","Male","Female","Female","Female","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Female","Female","Male","Male","Female","Male","Male","Male","Female","Female","Female","Female","Male","Male","Male","Male","Male","Male","Female","Female","Male","Female","Male","Female","Female","Female","Male","Male","Male","Female","Female","Male","Female","Female","Male","Female","Female","Male","Female","Male","Male","Male","Male","Female","Male","Female","Female","Female","Male","Male","Male","Female","Male","Female","Female","Female","Male","Male","Male","Male","Male","Female","Male","Female","Male","Female","Male","Male","Female","Female","Female","Male","Male","Female","Male","Female","Male","Male","Male","Female","Male","Female","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Female","Female","Female","Male","Female","Male","Male","Female","Male","Male","Female","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Female","Male","Male","Male","Female","Female","Female","Female","Male","Female","Female","Female","Male","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Female","Male","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Female","Female","Female","Male","Male","Male","Female","Male","Female","Female","Male","Male","Male","Female","Female","Female","Male","Male","Male","Female","Male","Female","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Male","Male","Female","Female","Male","Female","Male","Male","Male","Female","Male","Male","Female","Male","Male","Male","Male","Male","Male","Female","Female","Male","Male","Male","Female","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Male","Female","Male","Female","Male","Female","Male","Female","Male","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Female","Male","Male","Male","Male","Female","Female","Female","Female","Male","Female","Male","Female","Female","Male","Male","Male","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Female","Female","Male","Female","Male","Male","Female","Female","Male","Female","Male","Female","Male","Female","Male","Female","Male","Female","Female","Male","Female","Female","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Male","Male","Female","Male","Male","Female","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Male","Male","Female","Male","Male","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Male","Male","Female","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Male","Male","Female","Male","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Male","Male","Male","Male","Female","Female","Female","Male","Male","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Male","Female","Male","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Male","Female","Female","Female","Female","Female","Male","Female","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Male","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Female","Male","Female","Male","Male","Male","Female","Male","Male","Male","Male","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Male","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Female","Male","Male","Female","Female","Female","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Female","Male","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Female","Male","Female","Female","Male","Male","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Male","Male","Female","Female","Female","Female","Male","Male","Female","Male","Female","Female","Male","Male","Male","Male","Female","Female","Female","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Male","Male","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Female","Female","Male","Female","Male","Male","Female","Female","Female","Female","Male","Male","Female","Male","Male","Female","Female","Female","Male","Male","Male","Male","Female","Male","Female","Female","Female","Male","Male","Male","Female","Male","Female","Male","Male","Female","Male","Female","Female","Male","Male","Male","Female","Male","Male","Male","Female","Female","Male","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Male","Female","Male","Male","Female","Male","Male","Female","Female","Male","Female","Female","Female","Male","Male","Male","Female","Male","Female","Female","Male","Female","Male","Male","Female","Male","Female","Male","Male","Male","Female","Male","Female","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Male","Female","Female","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Female","Male","Male","Female","Male","Male","Female","Female","Male","Female","Male","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Male","Female","Female","Male","Female","Male","Female","Female","Female","Male","Male","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Female","Male","Male","Female","Male","Female","Female","Female","Female","Female","Male","Male","Female","Female","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Female","Male","Male","Male","Female","Male","Male","Female","Male","Male","Male","Male","Female","Male","Male","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Female","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Male","Male","Female","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Female","Female","Male","Female","Female","Male","Female","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Male","Male","Female","Female","Male","Female","Male","Female","Female","Male","Male","Male","Male","Male","Female","Female","Male","Female","Male","Female","Female","Male","Female","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Female","Male","Male","Female","Male","Female","Female","Male","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Female","Male","Female","Female","Female","Male","Male","Female","Female","Male","Female","Male","Female","Female","Male","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Female","Male","Female","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Male","Female","Female","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Female","Male","Male","Female","Male","Female","Female","Male","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Female","Female","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Female","Male","Female","Female","Male","Female","Female","Male","Male","Female","Female","Male","Female","Male","Female","Male","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Male","Male","Male","Female","Male","Female","Male","Female","Male","Male","Female","Female","Female","Male","Female","Female","Female","Male","Female","Male","Female","Female","Female","Male","Female","Female","Female","Male","Male","Male","Male","Male","Male","Female","Female","Male","Female","Male","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Male","Female","Male","Male","Female","Female","Female","Male","Male","Female","Female","Male","Female","Female","Male","Female","Male","Female","Female","Male","Male","Male","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Male","Male","Female","Female","Male","Female","Male","Female","Female","Female","Female","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Male","Female","Female","Male","Male","Female","Female","Female","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Male","Female","Male","Male","Male","Female","Female","Female","Male","Male","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Male","Female","Female","Female","Male","Male","Female","Female","Male","Male","Male","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Male","Female","Male","Female","Female","Female","Male","Male","Female","Male","Female","Female","Female","Male","Female","Female","Male","Female","Male","Male","Female","Male","Male","Male","Female","Female","Female","Female","Female","Male","Female","Male","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Male","Male","Female","Female","Female","Male","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Female","Male","Male","Female","Female","Female","Female","Male","Male","Female","Male","Male","Male","Female","Male","Female","Male","Female","Female","Female","Male","Female","Male","Male","Female","Female","Female","Female","Male","Female","Male","Female","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Male","Female","Male","Male","Male","Female","Male","Female","Female","Male","Female","Male","Male","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Female","Male","Female","Female","Male","Female","Male","Female","Male","Female","Female","Female","Female","Male","Female","Male","Female","Male","Female","Male","Female","Female","Male","Female","Male","Male","Female","Male","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Female","Male","Female","Female","Male","Female","Male","Female","Female","Male","Female","Male","Male","Female","Female","Female","Male","Female","Female","Male","Female","Female","Female","Female","Male","Male","Female","Female","Female","Male","Male","Male","Female","Male","Female","Male","Female","Male","Male","Female","Male","Male","Male","Male","Female","Male","Male","Female","Male","Female","Female","Male","Male","Male","Male","Male","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Male","Female","Male","Female","Male","Male","Female","Male","Female","Female","Female","Male","Male","Male","Female","Male","Female","Male","Female","Male","Female","Female","Male","Female","Female","Male","Male","Female","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Female","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Female","Female","Male","Male","Female","Male","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Male","Male","Female","Male","Male","Female","Male","Female","Female","Male","Male","Female","Female","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Female","Male","Female","Male","Female","Male","Male","Female","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Male","Female","Male","Male","Male","Male","Female","Male","Female","Female","Female","Female","Male","Female","Female","Male","Male","Female","Female","Male","Male","Female","Female","Female","Female","Female","Male","Female","Male","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Female","Female","Male","Male","Male","Female","Male","Male","Male","Male","Female","Male","Male","Male","Male","Male","Female","Female","Male","Male","Male","Female","Male","Male","Female","Male","Male","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Female","Male","Male","Male","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Male","Male","Female","Female","Female","Male","Male","Male","Male","Male","Male","Female","Female","Female","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Female","Male","Female","Male","Male","Male","Female","Female","Female","Male","Female","Male","Female","Male","Female","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Male","Male","Female","Male","Male","Male","Male","Male","Male","Female","Female","Male","Female","Male","Female","Female","Male","Male","Female","Female","Female","Female","Male","Male","Male","Female","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Male","Male","Female","Male","Male","Female","Female","Female","Female","Male","Female","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Male","Male","Male","Male","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Male","Male","Male","Female","Male","Female","Male","Male","Female","Female","Female","Male","Female","Male","Male","Male","Male","Female","Male","Male","Female","Male","Female","Female","Male","Male","Male","Male","Female","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Male","Male","Male","Male","Female","Female","Male","Female","Female","Male","Female","Female","Female","Male","Male","Female","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Male","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Female","Male","Male","Male","Female","Male","Female","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Female","Female","Male","Female","Male","Female","Male","Female","Female","Female","Male","Female","Male","Female","Male","Female","Female","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Male","Female","Male","Female","Male","Male","Female","Female","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Female","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Male","Male","Female","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Female","Female","Female","Female","Male","Female","Female","Female","Male","Male","Male","Female","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Female","Male","Male","Female","Female","Female","Female","Female","Male","Male","Female","Male","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Female","Male","Male","Female","Male","Female","Female","Female","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Female","Male","Male","Female","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Female","Male","Female","Female","Female","Female","Female","Female","Male","Male","Female","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Female","Female","Male","Male","Female","Female","Female","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Female","Male","Male","Female","Female","Male","Male","Male","Female","Female","Male","Female","Female","Male","Male","Male","Male","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Male","Male","Female","Female","Male","Male","Female","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Male","Male","Male","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Female","Female","Male","Female","Male","Male","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Male","Male","Male","Male","Female","Female","Female","Female","Male","Male","Male","Female","Male","Female","Female","Male","Male","Female","Female","Male","Female","Female","Male","Female","Male","Male","Male","Female","Male","Female","Female","Female","Male","Female","Female","Female","Male","Female","Female","Male","Female","Male","Female","Male","Female","Female","Female","Male","Female","Male","Male","Female","Male","Male","Female","Female","Female","Male","Female","Male","Female","Male","Male","Male","Female","Male","Female","Male","Male","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Male","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Female","Female","Female","Male","Female","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Male","Female","Male","Male","Male","Male","Female","Male","Female","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Male","Male","Female","Female","Female","Male","Male","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Male","Female","Female","Male","Female","Male","Female","Female","Female","Male","Female","Male","Female","Male","Female","Female","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Female","Female","Male","Female","Male","Male","Female","Male","Female","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Male","Male","Female","Male","Female","Male","Female","Male","Female","Female","Female","Male","Female","Female","Male","Female","Female","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Male","Male","Female","Male","Female","Female","Male","Female","Female","Male","Female","Female","Male","Male","Male","Male","Male","Male","Female","Male","Male","Male","Male","Female","Female","Female","Female","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Female","Female","Female","Male","Female","Male","Male","Female","Female","Female","Female","Male","Female","Male","Male","Male","Male","Female","Female","Female","Female","Female","Male","Male","Male","Female","Female","Female","Female","Female","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Female","Female","Female","Male","Male","Female","Female","Female","Female","Male","Female","Male","Female","Male","Male","Female","Male","Male","Male","Male","Male","Male","Male","Male","Female","Male","Female","Male","Female","Male","Male","Female","Male","Male","Female","Female","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Male","Female","Female","Male","Female","Female","Male","Male","Female","Female","Female","Male","Female","Male","Male","Male","Male","Female","Female","Female","Male","Male","Male","Male","Male","Female","Female","Male","Male","Female","Male","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Female","Male","Female","Male","Male","Female","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Female","Female","Male","Male","Female","Female","Male","Male","Female","Female","Female","Male","Female","Female","Male","Female","Female","Male","Male","Male","Female","Male","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Male","Female","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Female","Female","Female","Male","Female","Male","Female","Male","Female","Male","Male","Male","Female","Male","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Female","Female","Male","Female","Male","Male","Female","Male","Female","Male","Male","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Female","Female","Female","Male","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Female","Male","Male","Male","Male","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Male","Female","Female","Female","Male","Female","Female","Female","Male","Male","Male","Female","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Male","Male","Female","Female","Male","Female","Male","Male","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Female","Male","Female","Female","Male","Male","Male","Male","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Female","Female","Female","Male","Male","Female","Female","Male","Male","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Male","Female","Male","Male","Female","Female","Female","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Male","Male","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Female","Female","Male","Male","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Male","Female","Female","Female","Male","Female","Female","Male","Female","Male","Female","Female","Female","Male","Male","Male","Male","Male","Male","Male","Female","Female","Female","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Male","Male","Male","Female","Female","Male","Male","Female","Female","Female","Male","Male","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Female","Male","Female","Female","Male","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Female","Male","Male","Male","Female","Male","Female","Female","Female","Male","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Female","Male","Female","Female","Male","Male","Male","Female","Male","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Male","Male","Male","Female","Female","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Male","Female","Female","Female","Male","Female","Female","Female","Female","Male","Male","Female","Female","Female","Male","Male","Female","Male","Female","Male","Male","Male","Female","Male","Female","Male","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Male","Male","Male","Female","Male","Female","Male","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Male","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Female","Female","Male","Male","Female","Male","Male","Female","Male","Male","Male","Female","Female","Female","Female","Male","Male","Female","Male","Female","Male","Female","Male","Male","Male","Female","Male","Female","Male","Female","Male","Female","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Female","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Female","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Male","Female","Female","Male","Male","Male","Female","Female","Female","Male","Male","Female","Male","Male","Male","Female","Female","Male","Male","Male","Female","Female","Female","Female","Male","Male","Female","Female","Male","Male","Female","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Female","Male","Female","Female","Male","Female","Male","Male","Male","Female","Male","Male","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Male","Female","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Female","Female","Male","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Male","Male","Female","Male","Female","Female","Male","Female","Female","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Male","Male","Female","Male","Male","Female","Male","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Female","Male","Male","Male","Male","Female","Male","Female","Male","Male","Male","Female","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Male","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Male","Female","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Female","Female","Female","Male","Male","Male","Male","Female","Male","Male","Male","Male","Male","Female","Female","Male","Female","Male","Male","Female","Male","Female","Male","Female","Male","Male","Female","Male","Female","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Female","Female","Male","Female","Female","Female","Male","Male","Male","Male","Male","Female","Female","Male","Male","Female","Male","Female","Female","Female","Male","Female","Female","Female","Male","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Female","Female","Male","Male","Female","Female","Male","Male","Female","Male","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Female","Male","Female","Female","Female","Female","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Male","Male","Female","Female","Male","Male","Male","Male","Female","Male","Female","Female","Male","Female","Male","Male","Male","Male","Female","Female","Female","Male","Male","Female","Male","Female","Male","Female","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Female","Male","Male","Male","Male","Male","Female","Male","Female","Female","Female","Male","Male","Female","Female","Male","Male","Female","Male","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Female","Male","Female","Male","Female","Male","Male","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Female","Male","Male","Male","Male","Male","Male","Female","Male","Female","Male","Male","Male","Female","Female","Male","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Male","Male","Male","Female","Male","Male","Male","Female","Male","Female","Female","Male","Female","Female","Female","Female","Male","Male","Female","Male","Male","Male","Female","Male","Male","Male","Male","Female","Male","Female","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Male","Female","Female","Female","Female","Male","Male","Female","Female","Female","Female","Male","Female","Female","Male","Female","Female","Female","Male","Male","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Male","Female","Male","Male","Female","Male","Male","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Female","Male","Female","Female","Female","Male","Female","Male","Male","Female","Male","Male","Female","Female","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Female","Male","Male","Male","Male","Male","Female","Male","Female","Female","Female","Male","Female","Female","Male","Female","Male","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Female","Male","Female","Male","Female","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Male","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Female","Male","Female","Male","Male","Female","Male","Male","Male","Male","Female","Female","Female","Female","Male","Male","Female","Male","Female","Female","Female","Female","Female","Male","Male","Male","Female","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Female","Male","Male","Male","Female","Male","Female","Female","Female","Male","Male","Male","Female","Male","Male","Female","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Male","Female","Female","Male","Female","Female","Female","Female","Female","Male","Male","Male","Female","Male","Male","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Female","Male","Female","Female","Female","Male","Female","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Male","Female","Female","Male","Female","Female","Female","Male","Male","Male","Female","Female","Female","Female","Female","Male","Female","Male","Female","Female","Female","Male","Female","Male","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Male","Female","Female","Male","Female","Male","Male","Male","Female","Male","Male","Male","Male","Female","Male","Male","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Male","Female","Female","Male","Male","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Female","Male","Male","Male","Female","Female","Male","Male","Male","Male","Female","Male","Male","Female","Male","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Male","Female","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Male","Male","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Female","Female","Male","Female","Female","Male","Female","Male","Male","Female","Female","Female","Female","Female","Male","Female","Male","Female","Male","Female","Male","Female","Male","Male","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Male","Male","Female","Female","Male","Male","Male","Female","Male","Female","Female","Female","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Male","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Male","Male","Female","Male","Male","Male","Male","Male","Female","Female","Male","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Female","Male","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Female","Female","Female","Female","Male","Female","Female","Male","Male","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Male","Female","Female","Male","Female","Female","Female","Female","Male","Male","Male","Female","Female","Female","Female","Male","Male","Male","Female","Female","Female","Female","Female","Male","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Male","Female","Male","Female","Male","Female","Male","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Male","Male","Female","Female","Male","Male","Male","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Female","Female","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Male","Female","Female","Female","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Male","Female","Female","Male","Female","Male","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Female","Female","Male","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Male","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Female","Female","Female","Female","Female","Female","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Male","Female","Male","Male","Male","Female","Female","Male","Female","Male","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Male","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Female","Female","Female","Female","Male","Male","Female","Female","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Female","Female","Male","Male","Female","Male","Male","Female","Female","Female","Male","Female","Female","Male","Female","Female","Male","Female","Female","Female","Male","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Male","Female","Male","Male","Female","Female","Female","Female","Female","Male","Female","Female","Male","Female","Male","Female","Female","Male","Female","Male","Male","Female","Female","Female","Female","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Female","Female","Male","Female","Female","Female","Male","Male","Female","Female","Female","Male","Female","Female","Male","Male","Female","Female","Female","Male","Male","Female","Female","Female","Male","Male","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Male","Female","Female","Male","Female","Female","Male","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Female","Female","Female","Female","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Female","Female","Female","Female","Female","Male","Male","Female","Male","Female","Female","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Male","Female","Male","Female","Female","Female","Male","Male","Female","Female","Female","Male","Male","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Female","Female","Male","Female","Female","Male","Female","Female","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Male","Male","Male","Female","Male","Male","Female","Male","Female","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Female","Male","Female","Female","Male","Female","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Female","Male","Male","Male","Male","Male","Female","Male","Female","Female","Male","Female","Male","Male","Female","Female","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Female","Female","Female","Male","Male","Male","Male","Female","Male","Female","Female","Female","Female","Male","Female","Male","Male","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Male","Male","Male","Male","Male","Female","Female","Male","Female","Female","Male","Female","Female","Female","Male","Female","Male","Female","Male","Male","Female","Male","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Female","Female","Male","Female","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Male","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Male","Female","Female","Female","Male","Female","Male","Male","Female","Male","Female","Male","Male","Female","Female","Male","Female","Male","Male","Female","Female","Female","Male","Female","Male","Male","Female","Male","Male","Female","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Male","Male","Male","Female","Female","Male","Male","Male","Female","Male","Male","Female","Male","Male","Male","Male","Female","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Female","Female","Male","Female","Female","Male","Female","Male","Male","Male","Male","Female","Male","Male","Male","Male","Male","Male","Female","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Female","Male","Male","Female","Male","Female","Female","Male","Female","Female","Female","Male","Male","Male","Male","Male","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Female","Male","Male","Female","Female","Female","Male","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Male","Male","Male","Male","Female","Female","Male","Male","Female","Male","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Female","Male","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Male","Male","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Male","Male","Female","Female","Female","Male","Male","Male","Female","Male","Male","Female","Male","Female","Female","Female","Male","Female","Male","Female","Male","Female","Female","Male","Male","Female","Male","Female","Male","Male","Female","Male","Male","Male","Male","Female","Female","Male","Female","Female","Female","Female","Female","Male","Male","Male","Female","Male","Male","Male","Female","Male","Female","Female","Male","Female","Female","Male","Female","Male","Male","Female","Male","Female","Female","Female","Male","Female","Female","Male","Male","Female","Female","Male","Male","Male","Female","Male","Female","Female","Male","Male","Male","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Female","Male","Male","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Female","Male","Female","Male","Female","Male","Female","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Female","Male","Male","Male","Female","Male","Female","Female","Male","Female","Male","Female","Female","Female","Male","Female","Male","Male","Male","Male","Male","Male","Female","Female","Female","Female","Male","Male","Female","Female","Male","Male","Female","Male","Male","Male","Female","Male","Male","Male","Female","Male","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Female","Male","Male","Female","Female","Male","Male","Female","Male","Male","Female","Male","Male","Female","Female","Male","Female","Male","Female","Female","Female","Male","Male","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Male","Male","Male","Female","Male","Female","Male","Female","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Male","Female","Male","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Female","Female","Male","Female","Male","Female","Female","Female","Male","Male","Male","Female","Male","Female","Female","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Male","Male","Male","Male","Male","Male","Male","Female","Female","Female","Male","Male","Male","Male","Female","Male","Male","Female","Male","Female","Male","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Male","Male","Female","Male","Female","Male","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Female","Female","Male","Male","Male","Male","Female","Female","Male","Male","Male","Male","Female","Female","Male","Male","Female","Male","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Male","Male","Female","Male","Female","Male","Female","Female","Male","Female","Female","Female","Male","Male","Female","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Male","Female","Female","Male","Male","Male","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Male","Male","Female","Female","Female","Female","Male","Male","Female","Male","Female","Male","Female","Female","Female","Female","Male","Female","Male","Female","Male","Male","Male","Female","Female","Male","Female","Male","Male","Male","Male","Male","Female","Female","Female","Female","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Female","Female","Female","Male","Female","Female","Female","Female","Female","Female","Male","Female","Male","Female","Male","Female","Male","Female","Male","Female","Male","Male","Male","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Female","Male","Male","Male","Female","Female","Male","Female","Male","Female","Female","Male","Female","Male","Female","Female","Male","Male","Female","Female","Female","Female","Female","Male","Male","Male","Female","Male","Male","Female","Female","Female","Male","Male","Male","Male","Male","Male","Male","Male","Female","Male","Female","Female","Male","Female","Male","Female","Female","Male","Male","Male","Female","Male","Male","Male","Male","Male","Female","Female","Male","Male","Male","Female","Male","Female","Male","Female","Male","Male","Female","Female","Male","Female","Male","Female","Female","Male","Male","Female","Male","Male","Female","Female","Male","Male","Male","Female","Female","Male","Male","Male","Male","Female","Female","Female","Female","Male","Female","Female","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Female","Male","Female","Male","Male","Male","Male","Female","Male","Male","Female","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Male","Female","Male","Female","Female","Male","Female","Male","Male","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Male","Male","Male","Male","Male","Female","Female","Female","Male","Male","Female","Female","Female","Female","Male","Male","Female","Male","Female","Male","Male","Male","Female","Female","Male","Male","Female","Male","Male","Female","Male","Male","Female","Male","Male","Male","Male","Male","Male","Male","Male","Male","Female","Male","Female","Male","Male","Male","Male","Male","Female","Male","Male","Female","Female","Female","Male","Male","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Male","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Male","Male","Female","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Female","Male","Male","Female","Female","Male","Female","Female","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Male","Male","Female","Female","Male","Female","Male","Male","Female","Female","Male","Male","Female","Female","Female","Female","Female","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Female","Male","Female","Female","Male","Male","Male","Female","Male","Male","Female","Male","Female","Male","Female","Female","Female","Male","Male","Male","Female","Female","Male","Female","Female","Male","Female","Female","Female","Female","Male","Female","Female","Male","Male","Female","Male","Male","Male","Male","Female","Female","Male","Male","Male","Male","Female","Female","Female","Female","Male","Female","Male","Female","Female","Male","Female","Female","Female","Male","Female","Female","Female","Male","Female","Female","Female","Female","Male","Male","Male","Male","Female","Male","Male","Male","Male","Female","Female","Female","Female","Male","Female","Male","Male","Male","Female","Female","Male","Female","Female","Male","Female","Male","Male","Male","Male","Male","Male","Female","Male","Male","Female","Female","Male","Male","Male","Male","Male","Female","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Female","Male","Male","Female","Male","Female","Male","Female","Female","Male","Male","Female","Female","Male","Male","Male","Female","Male","Female","Male","Male","Female","Female","Male","Female","Female","Female","Male","Female","Female","Male","Male","Female","Male","Male","Male","Female","Female","Female","Female","Male","Male","Male","Female","Male","Female","Male","Male","Female","Male","Male","Female","Female","Male","Female","Female","Male","Male","Female","Female","Female","Female","Female","Male","Male","Male","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Female","Female","Female","Female","Female","Male","Female","Female","Female","Male","Male","Male","Female","Female","Female","Male","Female","Male","Female","Male","Male","Female","Male","Male","Male","Female","Male","Male","Female","Male","Male","Male","Male","Female","Male","Female","Male","Male","Male","Male","Male","Male","Male","Male","Male","Male","Female","Female","Male","Male","Male","Male","Male","Female","Male","Female","Female","Female","Male","Male","Male","Female","Male","Female","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Female","Female","Female","Female","Female","Female","Female","Female","Female","Male","Female","Male","Male","Female","Male","Male","Female","Male","Male","Male","Female","Male","Female","Female","Male","Female","Female","Male","Female","Female","Male","Female","Female","Male","Female","Female","Male","Male","Male","Male","Female","Female","Female","Male","Male","Male","Female","Female","Female","Female","Male","Female","Female","Female","Male","Male","Male","Female","Male","Male","Female","Male","Male","Male","Female","Female","Female","Male","Female","Female","Male","Female","Female","Female","Female","Male","Female","Female","Female","Male","Female","Male"],"Wage_hour":[5.7803468208,10.569777044,13.786127168,6.7514450867,7.2667217176,6.859344894,18.063583815,4.6242774566,5.0057803468,4.6242774566,11.560693642,15.211439002,7.9273327828,17.341040462,8.7486330261,5.0867052023,7.5144508671,7.8612716763,13.762730526,20.231213873,7.3426027183,8.0924855491,6.936416185,4.6242774566,5.7803468208,8.8928412628,8.2209377007,8.734746307,4.6242774566,17.036811682,5.4913294798,5.4277456647,16.872363693,5.7803468208,3.8535645472,5.549132948,6.3583815029,8.323699422,7.8612716763,13.87283237,8.6589595376,5.0867052023,4.8676604807,5.7803468208,3.1445086705,6.936416185,5.9454995871,18.643139641,9.2485549133,15.133998949,5.7803468208,4.1104688504,17.341040462,5.7803468208,8.6705202312,5.2023121387,9.2485549133,4.9132947977,16.184971098,12.04238921,2.8075970273,4.0462427746,10.569777044,8.1695568401,13.487475915,5.4936416185,8.7486330261,13.747851898,5.2023121387,4.3352601156,8.0924855491,9.8265895954,16.698779705,8.0924855491,6.5028901734,5.1380860629,7.3805902038,7.9099482811,9.1268634013,13.212221305,4.7225433526,9.2485549133,6.5510597303,5.7803468208,5.6300578035,8.0924855491,10.98265896,20.231213873,5.7803468208,12.716763006,8.4077771939,4.4958253051,8.6705202312,10.089332633,9.633911368,7.5144508671,8.7861271676,5.2848885219,10.404624277,15.414258189,11.560693642,6.0845756009,6.936416185,11.248242462,6.6061106524,6.0776218002,25.433526012,7.9273327828,6.936416185,15.520231214,6.936416185,10.789980732,5.3357047577,7.1933204881,6.2427745665,12.169151202,7.3988439306,6.936416185,6.936416185,12.138728324,13.212221305,14.450867052,8.6705202312,6.936416185,9.710982659,7.2667217176,14.450867052,8.6705202312,7.5144508671,9.633911368,5.7803468208,5.2023121387,5.4335260116,8.2209377007,8.6705202312,6.8739259491,6.3583815029,5.6518946692,8.6705202312,4.9545829893,15.445086705,11.177539224,8.0924855491,11.560693642,9.9091659785,5.0806206267,10.952236082,40.462427746,5.2023121387,8.4778420039,8.6705202312,14.450867052,6.936416185,10.918432884,4.6242774566,8.0924855491,6.936416185,3.4682080925,26.97495183,7.5144508671,5.549132948,20.809248555,5.7803468208,16.184971098,3.9636663914,12.138728324,5.4913294798,11.248242462,4.6242774566,9.2485549133,7.5144508671,8.8928412628,17.497266052,9.3360412436,6.8739259491,5.7803468208,9.2485549133,7.0064809949,6.936416185,9.2485549133,8.734746307,5.7803468208,5.4913294798,12.716763006,16.515276631,5.7803468208,16.647398844,10.98265896,16.515276631,4.6242774566,7.225433526,9.3735353851,8.5879438481,6.0693641618,5.7803468208,8.1429322123,8.6705202312,6.936416185,98.265895954,7.7071290944,5.7803468208,12.777608762,7.5144508671,24.046242775,4.7398843931,5.9454995871,13.005780347,4.6242774566,5.7032755299,11.873144821,7.3988439306,14.450867052,10.404624277,10.569777044,9.0232696013,6.8739259491,2.8901734104,5.0867052023,6.3583815029,6.936416185,2.5289017341,4.6242774566,7.7071290944,4.8676604807,8.3815028902,6.2758051197,7.7071290944,9.083402147,18.497109827,10.276172126,8.0924855491,10.404624277,7.8034682081,5.4913294798,8.6705202312,13.87283237,10.404624277,9.2485549133,6.3583815029,7.7071290944,21.271676301,8.9595375723,12.023121387,23.468208092,5.1380860629,7.9099482811,5.4913294798,4.6242774566,5.7803468208,5.8306107062,8.5879438481,4.6242774566,9.0610842056,8.6705202312,20.231213873,5.1380860629,15.819896562,4.0462427746,19.818331957,13.212221305,7.9273327828,3.7572254335,5.7803468208,15.414258189,5.1380860629,6.936416185,3.9306358382,7.2667217176,22.265039606,4.161849711,6.936416185,4.5417010735,6.6061106524,6.0115606936,9.9091659785,4.2592029206,6.936416185,8.6705202312,1.7341040462,12.169151202,6.7822736031,4.1104688504,6.0724064497,5.0578034682,9.8265895954,10.404624277,5.7803468208,4.293971924,5.7803468208,7.5144508671,23.121387283,13.086705202,5.0096339114,7.5144508671,9.7353209614,9.633911368,5.7803468208,16.247461334,5.8854440357,7.4142581888,17.726396917,17.785682526,8.4778420039,7.7398843931,9.8265895954,2.0552344252,8.6705202312,7.1466106148,15.1940545,9.9091659785,4.816955684,4.6242774566,7.8612716763,5.7687861272,7.4502247913,5.9454995871,4.6242774566,7.1933204881,10.569777044,8.0924855491,8.2080924855,14.450867052,5.3949903661,8.5879438481,5.1380860629,15.1940545,6.3583815029,5.2023121387,3.002569043,7.1142730102,10.404624277,11.911017691,7.9273327828,5.0867052023,5.7803468208,11.817597945,7.5144508671,5.0446663163,9.2485549133,9.633911368,12.551610239,10.05277708,6.4739884393,13.87283237,3.8535645472,9.8265895954,7.5144508671,5.5662599015,18.497109827,18.253726803,9.633911368,8.6705202312,15.414258189,5.4335260116,8.8081475365,11.329479769,17.341040462,6.3583815029,4.6242774566,null,10.173410405,6.936416185,3.2369942197,8.6705202312,7.2667217176,4.6242774566,16.247461334,8.5879438481,11.560693642,10.569777044,5.7803468208,4.2592029206,6.3583815029,6.3899106674,13.994523882,3.5260115607,7.3311715776,6.521416926,5.7803468208,4.133823787,5.2209584188,11.890999174,4.9207054987,8.9182493807,6.3583815029,7.7071290944,15.414258189,8.6705202312,15.414258189,7.8447563997,5.7803468208,5.8786127168,10.520231214,5.1380860629,5.2023121387,5.549132948,4.7602856171,7.1142730102,6.8400770713,10.701899257,5.7803468208,15.414258189,11.873144821,10.918432884,15.414258189,12.449977768,9.2485549133,14.372754257,7.4502247913,9.450867052,13.212221305,4.6242774566,8.6705202312,9.2485549133,12.716763006,9.8265895954,13.87283237,6.936416185,10.404624277,8.6705202312,6.936416185,13.87283237,20.346820809,21.337737407,12.169151202,6.936416185,18.74707077,3.4682080925,12.169151202,4.6242774566,9.8265895954,6.936416185,5.7803468208,10.98265896,6.936416185,6.0471320587,8.6705202312,12.611665791,17.175887696,8.6705202312,13.386066322,6.8069364162,5.2986512524,4.6242774566,14.602981442,5.549132948,5.2023121387,8.6705202312,5.2023121387,9.8265895954,6.2758051197,23.121387283,4.8676604807,23.121387283,6.1657032755,5.7225433526,2.8901734104,9.8265895954,7.0173410405,6.1657032755,12.716763006,6.936416185,9.2485549133,10.404624277,10.404624277,13.212221305,13.87283237,3.4682080925,5.2023121387,6.3005780347,2.9248554913,15.622558975,9.2485549133,7.4988283081,8.0924855491,null,17.341040462,4.6242774566,6.3058328954,5.2485549133,7.9099482811,8.9595375723,9.9091659785,13.005780347,9.2485549133,4.3352601156,8.6705202312,23.121387283,6.936416185,4.3352601156,26.820809249,4.6242774566,13.404899532,8.0924855491,24.442609414,14.450867052,8.0924855491,17.645269242,9.2485549133,7.9273327828,7.5144508671,6.3583815029,10.789980732,5.7803468208,7.5144508671,7.1933204881,4.1288191577,6.1657032755,9.8265895954,2.9427220179,5.7803468208,13.87283237,10.239471511,8.0924855491,8.9916506101,5.7803468208,5.7803468208,13.87283237,14.997656616,17.900428864,6.1657032755,14.533443435,10.404624277,6.936416185,9.4797687861,6.936416185,5.4913294798,6.5722543353,6.936416185,11.248242462,6.4739884393,5.1380860629,16.428354122,8.0924855491,9.2485549133,null,11.230388109,8.0924855491,7.9273327828,7.7071290944,11.560693642,12.49804718,11.560693642,17.341040462,7.0289017341,9.2485549133,17.645269242,6.936416185,9.8265895954,8.5879438481,5.1380860629,11.560693642,16.515276631,8.0924855491,3.2369942197,13.294797688,9.1084252934,11.560693642,9.8265895954,4.0275964945,9.2485549133,8.9190751445,7.5144508671,19.818331957,2.8901734104,6.6281310212,14.258188825,11.560693642,11.560693642,6.3583815029,10.404624277,6.936416185,7.225433526,6.0115606936,4.0462427746,5.7803468208,6.8786127168,11.560693642,5.7803468208,6.6795118818,8.0924855491,8.0924855491,3.3030553262,2.3121387283,9.8265895954,14.450867052,5.5050922103,6.0115606936,11.560693642,9.0474993717,17.341040462,17.785682526,6.3583815029,12.716763006,4.9545829893,5.7803468208,6.3583815029,8.0924855491,9.4026974952,17.341040462,6.5685759327,10.404624277,6.3583815029,7.5144508671,8.1560693642,3.4153592073,5.7803468208,10.173410405,4.2196531792,6.8208092486,23.121387283,4.0462427746,9.9984377441,14.602981442,8.323699422,9.9091659785,5.1380860629,13.87283237,7.1734104046,8.5879438481,9.2485549133,13.87283237,12.138728324,5.7803468208,7.9075144509,4.7293746716,12.138728324,29.427220179,7.1566198734,5.7803468208,6.1040462428,6.1657032755,11.560693642,7.7071290944,5.2601156069,18.111753372,4.6242774566,11.230388109,19.267822736,9.2485549133,14.073887912,6.6061106524,5.2023121387,12.777608762,5.3410404624,7.1933204881,19.818331957,17.836498761,2.1676300578,6.936416185,2.9543994862,5.6518946692,14.22854602,11.560693642,12.777608762,16.698779705,3.8535645472,8.6705202312,6.3583815029,8.2576383154,5.3757225434,9.9091659785,6.4226075787,9.2485549133,6.1040462428,6.936416185,5.4913294798,10.671409515,7.7071290944,6.936416185,5.0392767156,13.212221305,4.0462427746,10.664739884,9.8265895954,3.1791907514,20.231213873,11.494632535,9.9091659785,12.185596001,5.0867052023,2.0552344252,6.2490235901,11.271676301,8.2043632295,8.9113680154,4.9545829893,5.2023121387,6.3583815029,5.7803468208,8.6705202312,7.5144508671,5.0096339114,5.7803468208,9.2485549133,7.7898055702,6.7712634187,10.789980732,4.9132947977,8.4393063584,6.1271676301,8.6705202312,12.716763006,10.404624277,13.212221305,9.9091659785,7.5144508671,9.5375722543,9.633911368,6.6795118818,12.716763006,18.253726803,6.1657032755,8.1695568401,4.7428486735,6.936416185,6.0115606936,8.0924855491,6.936416185,42.03888597,6.936416185,11.560693642,9.3735353851,5.3949903661,11.560693642,7.225433526,21.965317919,4.6242774566,6.936416185,7.9273327828,7.4988283081,6.0693641618,10.404624277,6.936416185,13.212221305,8.8631984586,6.1271676301,5.2848885219,9.1268634013,4.9132947977,6.936416185,8.4778420039,10.569777044,11.560693642,6.936416185,4.9942196532,5.7803468208,14.372754257,6.0225708781,9.3735353851,9.633911368,16.76300578,9.3735353851,3.612716763,9.9091659785,23.746289642,3.5324341683,5.7803468208,6.8439306358,16.247461334,13.212221305,8.2576383154,4.9132947977,14.450867052,6.2813102119,4.4040737682,12.716763006,6.7437379576,8.6705202312,11.210369592,5.7803468208,7.5144508671,6.3583815029,11.890999174,11.560693642,11.560693642,4.6242774566,5.3949903661,7.5144508671,7.5144508671,6.4603876233,14.531791908,4.4464206314,13.294797688,9.1268634013,21.296014603,8.0924855491,9.1268634013,5.0096339114,8.5879438481,5.4913294798,20.038535645,6.936416185,16.247461334,9.2485549133,9.5054592164,6.936416185,12.169151202,9.8265895954,7.9273327828,13.747851898,5.7803468208,9.4310921813,2.774566474,6.3583815029,4.5761078998,10.05277708,7.6589595376,8.0924855491,8.0924855491,46.37489678,6.1657032755,7.4988283081,12.138728324,7.7071290944,9.8265895954,7.1933204881,11.230388109,5.7803468208,5.7803468208,5.2848885219,8.1237306671,10.98265896,2.8901734104,5.1156069364,6.936416185,2.408477842,7.1933204881,8.5879438481,6.4739884393,6.6795118818,6.936416185,10.374981473,1.387283237,5.2023121387,15.211439002,5.7803468208,9.2485549133,5.0536746491,13.87283237,28.901734104,8.1888246628,17.836498761,7.9728921666,6.936416185,5.549132948,6.7437379576,7.5278935341,5.7803468208,7.5144508671,5.7803468208,9.2485549133,5.6518946692,10.569777044,6.4739884393,7.3988439306,6.1657032755,6.936416185,21.871582565,7.5144508671,8.0422216637,2.2520831769,null,11.560693642,13.212221305,5.7803468208,5.549132948,8.6705202312,19.818331957,10.276172126,16.184971098,5.4500412882,7.5144508671,5.7803468208,7.0905587669,11.560693642,14.22854602,10.322047894,4.6242774566,6.936416185,7.5144508671,5.7803468208,5.7803468208,8.4077771939,11.322873658,10.310888924,6.936416185,10.404624277,5.0867052023,7.5669994745,6.6473988439,6.936416185,3.8535645472,13.994523882,64.739884393,8.0924855491,11.791907514,13.122949539,10.913294798,7.5144508671,6.3583815029,8.0924855491,9.668943773,6.936416185,3.9636663914,8.323699422,7.9099482811,13.87283237,9.9091659785,8.0924855491,7.5144508671,7.225433526,5.7803468208,10.569777044,6.6061106524,4.6242774566,7.7071290944,6.936416185,4.5317919075,4.161849711,12.716763006,7.7071290944,13.294797688,6.936416185,9.2485549133,10.019267823,6.289017341,8.6705202312,15.473988439,6.3583815029,17.469492614,5.2023121387,6.936416185,5.2848885219,7.5144508671,3.0828516378,8.4778420039,4.0462427746,8.0924855491,14.450867052,8.9916506101,5.5050922103,9.8265895954,17.836498761,16.184971098,9.633911368,10.847233691,5.7803468208,10.322047894,16.184971098,7.5144508671,7.1933204881,8.0924855491,11.560693642,10.98265896,14.997656616,17.341040462,9.3735353851,7.5144508671,5.7803468208,11.560693642,8.6705202312,16.184971098,8.0924855491,3.5886319846,19.818331957,5.549132948,10.404624277,3.2580136626,4.6242774566,5.0867052023,8.0924855491,8.1237306671,12.551610239,6.936416185,11.873144821,4.9132947977,15.414258189,11.560693642,10.039549741,8.0924855491,5.022922065,7.225433526,12.023121387,11.560693642,7.1566198734,12.49804718,13.87283237,8.6705202312,11.230388109,6.936416185,12.716763006,9.2485549133,6.3583815029,13.87283237,6.936416185,14.821402105,9.9091659785,17.341040462,17.341040462,11.248242462,7.225433526,13.005780347,5.9306358382,12.240734444,8.0924855491,7.5144508671,5.7803468208,5.3357047577,6.936416185,6.4739884393,9.2485549133,7.3988439306,10.445086705,14.450867052,19.818331957,7.0905587669,8.6705202312,8.5184058412,8.5879438481,6.0693641618,12.716763006,7.2832369942,9.9091659785,9.5054592164,13.87283237,8.0924855491,6.7585593597,18.566473988,8.0924855491,8.2576383154,13.994523882,15.854665566,9.2485549133,5.4335260116,9.2485549133,6.936416185,20.231213873,5.2023121387,17.919075145,11.560693642,11.560693642,11.248242462,5.2327350167,10.509721492,5.7803468208,11.560693642,7.0110013052,7.9273327828,5.1380860629,13.635689936,15.854665566,12.04238921,16.515276631,10.404624277,2.5377132384,7.5144508671,5.2665382145,6.936416185,14.739884393,11.817597945,66.473988439,6.521416926,8.4778420039,10.339595376,10.98265896,7.9099482811,3.9411455596,6.936416185,6.936416185,5.7407101569,5.7803468208,8.6705202312,11.560693642,6.9901868531,4.6242774566,6.1657032755,6.936416185,13.87283237,6.936416185,9.4797687861,4.6242774566,6.936416185,13.005780347,9.2485549133,4.3352601156,11.560693642,4.6242774566,9.9091659785,6.6024405909,7.7071290944,13.87283237,10.98265896,14.313239747,13.425321648,9.633911368,6.3583815029,5.1380860629,10.867052023,7.2667217176,9.2485549133,10.208092486,5.7803468208,5.7803468208,8.0924855491,6.6795118818,6.936416185,3.4682080925,6.936416185,3.8535645472,15.414258189,9.2485549133,4.8554913295,5.6069364162,9.3735353851,5.7803468208,10.952236082,9.1268634013,6.3583815029,4.6242774566,6.7052023121,8.6705202312,5.9285608419,6.936416185,17.341040462,4.816955684,7.5144508671,6.1657032755,6.2490235901,21.052960475,10.623340103,7.4988283081,5.9730250482,11.560693642,4.6242774566,5.7803468208,6.774566474,18.497109827,10.343778521,6.1657032755,4.6242774566,19.075144509,13.87283237,12.661712084,6.936416185,13.122949539,5.2023121387,16.184971098,14.533443435,7.1098265896,15.928066795,6.936416185,6.3058328954,6.0115606936,12.845215157,4.8554913295,6.936416185,8.0924855491,8.323699422,8.0924855491,11.560693642,4.5761078998,14.533443435,5.0867052023,5.4500412882,7.8612716763,5.6878612717,8.1888246628,12.169151202,2.408477842,17.175887696,6.6473988439,3.7572254335,8.8928412628,17.175887696,10.63583815,19.818331957,4.6242774566,3.8535645472,6.2620423892,4.6242774566,15.414258189,17.175887696,4.161849711,9.2485549133,16.955684008,12.138728324,16.815554388,4.6473988439,7.3988439306,8.5879438481,5.4913294798,4.6242774566,13.487475915,8.5879438481,5.2023121387,6.936416185,5.0289017341,3.0828516378,21.676300578,6.936416185,4.2389210019,14.450867052,7.9273327828,7.9273327828,9.2485549133,69.36416185,7.5144508671,6.1657032755,5.7803468208,6.6795118818,6.0556014313,16.515276631,5.8959537572,4.6242774566,5.7803468208,4.5086705202,4.1104688504,5.7803468208,7.301490721,5.1380860629,5.3757225434,15.028901734,8.0924855491,9.8265895954,5.7803468208,7.7071290944,7.5144508671,12.845215157,11.230388109,5.7803468208,20.729519633,5.7803468208,5.2023121387,20.137982472,6.936416185,24.971098266,11.560693642,8.6705202312,6.3583815029,7.225433526,8.0924855491,8.5879438481,7.5144508671,8.2576383154,7.4502247913,23.121387283,12.169151202,4.8383643759,8.5879438481,4.6242774566,4.816955684,7.6057195011,3.6994219653,10.173410405,8.5184058412,15.414258189,15.622558975,12.169151202,6.1965317919,7.225433526,6.936416185,6.3583815029,13.212221305,13.212221305,14.450867052,11.350499212,8.6705202312,5.7803468208,6.936416185,5.7803468208,6.3583815029,8.6705202312,8.5879438481,5.549132948,3.7456647399,8.3630549748,8.6705202312,5.1110435047,8.323699422,7.7071290944,5.3949903661,26.204238921,6.936416185,12.551610239,8.0924855491,7.2667217176,10.115606936,7.4988283081,6.2427745665,9.2485549133,6.3583815029,9.2485549133,13.294797688,1.9267822736,7.9273327828,13.87283237,6.5510597303,8.6705202312,14.643545279,11.098265896,12.551610239,6.4739884393,5.7803468208,12.845215157,18.497109827,5.2023121387,7.5144508671,8.8081475365,18.122168411,6.3583815029,9.2485549133,10.98265896,6.4739884393,8.0924855491,9.5375722543,3.8535645472,5.1445086705,6.936416185,7.7071290944,6.6061106524,16.515276631,8.5879438481,5.5050922103,5.7803468208,3.1791907514,54.913294798,12.611665791,8.0924855491,7.5144508671,10.671409515,19.818331957,9.2485549133,2.6424442609,13.87283237,8.6705202312,7.8034682081,6.2620423892,19.818331957,8.9341040462,7.3568050447,6.936416185,6.3583815029,7.7071290944,10.789980732,5.0096339114,7.9768786127,17.341040462,7.5144508671,7.1142730102,12.331406551,5.7803468208,8.0924855491,6.936416185,2.774566474,6.8739259491,12.611665791,17.341040462,6.936416185,16.955684008,4.9132947977,6.2758051197,13.212221305,23.781998348,19.818331957,9.1084252934,4.0462427746,5.0096339114,9.8265895954,7.5144508671,10.789980732,15.622558975,21.296014603,10.019267823,8.3630549748,15.211439002,4.6242774566,3.6784025223,2.8457092041,9.1522157996,7.1142730102,6.1657032755,6.936416185,8.6705202312,4.9132947977,12.716763006,5.5876685934,6.0115606936,7.3352601156,6.936416185,7.7071290944,10.404624277,5.1380860629,13.762730526,5.2548607462,9.1268634013,5.1734104046,15.211439002,8.6705202312,13.042833852,10.404624277,9.2485549133,7.5144508671,4.0462427746,12.551610239,14.821402105,6.936416185,19.996875488,15.622558975,5.5616309952,5.4113885131,9.8265895954,8.6705202312,10.509721492,7.5144508671,8.0924855491,9.8265895954,2.732527588,7.5144508671,7.5395828098,14.533443435,12.138728324,6.4226075787,19.818331957,8.4361818466,13.212221305,6.2427745665,16.428354122,12.551610239,6.4739884393,5.7803468208,12.331406551,6.936416185,7.5144508671,8.6705202312,16.955684008,17.341040462,3.6994219653,6.6061106524,4.7602856171,4.6242774566,11.0388109,12.716763006,11.560693642,11.560693642,7.7071290944,6.6473988439,5.7803468208,6.936416185,5.7803468208,12.716763006,9.2485549133,14.797687861,6.2490235901,4.6242774566,12.845215157,6.1657032755,3.4682080925,21.579961464,8.0924855491,8.3815028902,9.1268634013,11.560693642,12.716763006,6.3783137333,4.6242774566,23.121387283,6.3583815029,2.119460501,6.6473988439,4.6242774566,7.5144508671,6.936416185,5.0578034682,6.6061106524,4.161849711,4.6242774566,10.404624277,12.716763006,5.9033329234,6.5510597303,6.9239181378,13.294797688,11.560693642,15.028901734,4.7481420314,8.5879438481,7.3988439306,4.6242774566,10.404624277,5.7803468208,14.450867052,4.6242774566,11.560693642,6.936416185,8.6705202312,18.497109827,6.3583815029,5.2023121387,27.74566474,4.9132947977,5.7803468208,11.560693642,19.157720892,15.622558975,2.7525461051,8.0924855491,9.633911368,5.6051847959,1.9267822736,8.6705202312,10.623340103,11.560693642,6.6061106524,15.414258189,8.6705202312,12.169151202,8.6705202312,19.075144509,13.294797688,7.225433526,11.560693642,11.560693642,5.2548607462,18.253726803,7.9099482811,4.6242774566,17.341040462,8.323699422,3.8535645472,14.533443435,4.9132947977,10.398018167,12.138728324,6.936416185,13.386066322,13.068610204,7.8516377649,5.901734104,9.2485549133,6.3583815029,6.936416185,12.023121387,5.0096339114,3.7572254335,14.797687861,6.936416185,8.6705202312,6.3583815029,8.6705202312,5.2023121387,5.6151940545,7.225433526,5.0392767156,6.936416185,17.836498761,11.010184421,5.7803468208,5.3770668101,10.115606936,11.849710983,6.5976609759,6.936416185,9.6309470876,4.1387283237,20.809248555,2.697495183,3.3030553262,6.4739884393,5.7803468208,6.936416185,3.8535645472,9.8265895954,6.3583815029,4.0141297367,7.9768786127,6.3583815029,4.9421965318,7.8034682081,2.5690430315,4.3352601156,5.6518946692,11.560693642,10.924855491,6.6795118818,9.2485549133,10.404624277,14.450867052,15.854665566,11.230388109,23.121387283,4.6242774566,11.890999174,5.2023121387,9.8265895954,19.267822736,17.572254335,11.829546982,6.1657032755,24.971098266,6.3583815029,8.1604896294,14.450867052,6.936416185,21.117533719,8.0924855491,null,11.560693642,14.450867052,8.0924855491,8.6705202312,9.3735353851,4.161849711,7.5144508671,7.5144508671,4.6242774566,4.161849711,18.74707077,7.5144508671,6.936416185,9.633911368,5.5938840201,4.161849711,5.7803468208,4.5649918482,26.011560694,13.294797688,5.5144508671,9.2485549133,7.5144508671,5.0867052023,9.9984377441,7.5395828098,12.716763006,8.6705202312,7.5144508671,7.7071290944,6.2295623452,7.5498407455,4.2726396917,7.2667217176,7.774566474,8.6705202312,8.0924855491,9.2485549133,86.705202312,14.450867052,6.936416185,8.6705202312,3.5308285164,4.6242774566,7.2667217176,20.231213873,6.1657032755,5.7803468208,10.255986788,10.98265896,8.0924855491,22.020368841,13.994523882,10.404624277,9.7353209614,6.1657032755,13.005780347,8.6705202312,14.450867052,6.1657032755,12.169151202,16.247461334,4.6242774566,4.5086705202,2.0231213873,9.4962840628,7.9099482811,6.7262217551,4.3352601156,4.5163776493,13.87283237,7.5144508671,8.734746307,12.023121387,37.456647399,6.936416185,6.936416185,10.404624277,20.478943022,11.560693642,17.065785852,15.211439002,7.9273327828,8.5879438481,2.7056942565,13.87283237,6.5028901734,4.6242774566,8.6705202312,15.953757225,5.9454995871,7.5144508671,7.4988283081,5.7803468208,10.404624277,8.3815028902,12.49804718,11.010184421,13.87283237,12.427745665,4.4315992293,13.212221305,12.138728324,17.341040462,24.971098266,4.1104688504,20.231213873,5.7803468208,4.6242774566,7.5144508671,12.49804718,6.936416185,8.9182493807,14.450867052,8.0924855491,3.4682080925,5.2023121387,9.2485549133,13.87283237,8.7861271676,4.374316513,7.225433526,14.450867052,7.5144508671,3.8535645472,4.3490228461,9.6960656349,5.7803468208,19.996875488,17.036811682,6.936416185,9.633911368,5.0867052023,7.5144508671,5.7803468208,5.8511265778,7.0648683365,14.128384545,6.1657032755,6.3583815029,6.6061106524,7.7071290944,5.4913294798,18.74707077,5.0867052023,6.936416185,15.414258189,4.9545829893,5.7803468208,8.6705202312,8.0924855491,8.6705202312,7.7456647399,11.560693642,11.010184421,15.722543353,6.936416185,5.6518946692,11.230388109,16.599970357,5.7803468208,8.6705202312,15.622558975,6.6061106524,4.8933263269,8.5879438481,3.0828516378,6.0693641618,6.936416185,13.359023764,13.747851898,11.560693642,6.0751445087,14.450867052,5.1156069364,6.4739884393,5.6914184082,16.184971098,8.0924855491,4.6242774566,6.0556014313,6.936416185,9.633911368,9.2485549133,7.3988439306,5.7803468208,18.166804294,10.343778521,8.3815028902,15.606936416,5.465055176,19.267822736,6.3583815029,12.49804718,4.9132947977,9.2485549133,6.6061106524,6.936416185,5.7803468208,5.2023121387,3.4682080925,5.549132948,3.6994219653,6.936416185,7.5144508671,4.8554913295,7.5144508671,4.2609413708,5.7803468208,8.0924855491,6.8208092486,6.0462427746,5.7803468208,5.7803468208,8.0924855491,14.602981442,8.8081475365,10.789980732,5.7803468208,14.450867052,6.3005780347,8.6705202312,6.6061106524,26.011560694,9.2485549133,15.606936416,7.301490721,6.7976878613,5.7803468208,10.05277708,6.3583815029,3.4682080925,7.8612716763,5.7803468208,18.122168411,13.87283237,7.9273327828,5.7803468208,8.2576383154,6.3058328954,10.404624277,3.0828516378,11.560693642,13.87283237,3.3030553262,7.8612716763,12.524084778,14.450867052,5.7803468208,4.9132947977,10.952236082,5.7803468208,18.497109827,4.6242774566,10.774566474,10.404624277,3.1529164477,6.936416185,6.936416185,9.0234256161,9.8265895954,8.6705202312,5.7803468208,4.2658959538,8.6705202312,7.1566198734,7.9099482811,11.560693642,8.0924855491,5.2023121387,14.602981442,8.0924855491,7.7071290944,6.1657032755,6.3583815029,20.687557043,4.6242774566,9.0751445087,4.816955684,5.7803468208,8.6705202312,6.1040462428,15.1940545,19.470641923,8.6705202312,11.890999174,7.5144508671,6.3583815029,6.3583815029,7.1279933939,6.936416185,13.212221305,5.549132948,8.5184058412,14.533443435,12.716763006,3.0828516378,9.2485549133,8.6705202312,8.6705202312,16.184971098,5.549132948,34.682080925,4.6242774566,6.936416185,13.87283237,6.6473988439,6.936416185,8.6705202312,9.633911368,11.560693642,8.6705202312,16.515276631,11.560693642,4.3930635838,4.2774566474,13.994523882,19.737769632,2.408477842,5.5662599015,8.0924855491,8.2576383154,10.019267823,5.7803468208,8.5879438481,21.296014603,11.560693642,7.2667217176,10.98265896,7.3217726397,8.1237306671,19.818331957,6.936416185,null,9.9091659785,5.549132948,5.7803468208,4.6242774566,12.169151202,5.3949903661,9.1268634013,7.4988283081,15.414258189,4.9545829893,5.7803468208,15.414258189,8.7486330261,5.2023121387,4.4464206314,8.0924855491,21.139554088,5.7803468208,4.6242774566,9.9091659785,8.1237306671,5.3949903661,7.7071290944,11.560693642,12.023121387,5.2023121387,6.936416185,7.7071290944,6.3583815029,8.6705202312,13.87283237,9.710982659,66.795118818,15.606936416,3.9768786127,7.5144508671,6.3583815029,14.450867052,17.506193229,18.497109827,9.8090733929,8.9182493807,18.034682081,12.449977768,6.6061106524,14.518080387,5.7803468208,7.7071290944,9.2485549133,17.919075145,8.6033068961,19.524727039,14.161849711,9.9091659785,16.247461334,9.4137076796,12.551610239,10.569777044,11.2642656,10.569777044,12.845215157,8.5879438481,9.9091659785,10.590879897,11.021194605,16.515276631,6.936416185,13.87283237,14.533443435,8.6705202312,9.2485549133,16.515276631,12.716763006,11.098265896,7.3454868831,10.671409515,9.1164327002,9.5788604459,11.43224149,8.5879438481,8.2947976879,21.58509955,17.820809249,9.1410135771,10.070648683,11.230388109,41.361592807,13.747851898,7.7071290944,7.225433526,18.522105921,16.184971098,15.606936416,5.1791907514,18.122168411,3.4682080925,11.829546982,11.873144821,22.350674374,13.359023764,20.749962946,12.169151202,12.023121387,13.232547799,16.184971098,10.602807597,8.8612716763,18.74707077,6.6930331609,9.0850133935,5.9285608419,11.990090834,9.633911368,9.485697347,15.622558975,10.569777044,10.918432884,10.671409515,9.2485549133,3.4814203138,16.599970357,11.560693642,9.9091659785,9.2485549133,11.420231214,10.903559477,9.8090733929,11.560693642,8.9361037338,9.9091659785,6.0776218002,6.1416184971,26.424442609,16.184971098,14.533443435,14.219653179,12.777608762,13.042833852,8.5879438481,9.485697347,13.212221305,9.485697347,5.2848885219,20.47088679,2.0552344252,15.028901734,14.450867052,8.0924855491,8.3815028902,14.533443435,9.710982659,10.701899257,17.10982659,9.2485549133,10.952236082,23.121387283,9.4599504542,10.343778521,18.497109827,9.1637764933,13.005780347,17.341040462,22.633269107,15.414258189,9.4587493431,27.74566474,11.890999174,9.8265895954,18.497109827,5.5050922103,19.818331957,9.2485549133,8.5184058412,15.414258189,10.199834847,23.121387283,18.497109827,7.2882633828,15.854665566,16.475639967,15.764582239,14.602981442,10.357195791,10.305532618,7.7071290944,15.414258189,9.9091659785,9.1268634013,18.497109827,13.005780347,13.851156069,9.1268634013,6.2620423892,15.028901734,9.9091659785,12.283236994,10.671409515,6.7382328654,19.421965318,12.757565454,11.560693642,16.515276631,17.126953543,4.9132947977,16.599970357,15.009083402,11.838150289,12.881915772,9.9984377441,8.5879438481,17.645269242,13.386066322,8.5914207484,11.817597945,10.930110352,10.115606936,13.526011561,11.2642656,8.0924855491,31.529164477,16.184971098,8.0462427746,13.542526837,23.121387283,14.533443435,12.551610239,17.241948803,17.785682526,9.3735353851,15.211439002,10.404624277,10.343778521,9.3014037985,9.063583815,16.515276631,7.9550070302,13.760349945,8.6705202312,10.671409515,15.819896562,9.633911368,10.569777044,11.230388109,5.2023121387,9.7052023121,9.4335260116,16.76300578,11.230388109,20.552344252,16.647398844,12.138728324,9.0229804032,12.169151202,8.3922072361,12.881915772,11.543775553,15.414258189,15.414258189,9.2485549133,24.405908799,10.200612037,12.774566474,10.789980732,9.7623635196,6.4226075787,11.560693642,11.758876961,12.947976879,10.98265896,9.6565793948,12.551610239,12.49804718,8.7486330261,16.515276631,12.351958895,5.0338563171,14.450867052,13.225433526,13.212221305,13.87283237,5.1380860629,13.517118719,11.230388109,3.7572254335,12.449977768,16.515276631,18.74707077,11.560693642,9.843104872,14.997656616,15.595926232,16.247461334,11.857121684,11.560693642,3.8535645472,15.075144509,13.040462428,12.551610239,10.830057803,9.633911368,10.343778521,8.6705202312,16.184971098,16.515276631,9.9091659785,9.633911368,10.789980732,17.175887696,11.560693642,13.199009083,8.2750228172,24.855491329,9.9091659785,13.635689936,17.175887696,23.746289642,10.4596752,15.414258189,9.7353209614,11.857121684,10.952236082,14.821402105,13.87283237,13.212221305,13.487475915,18.497109827,9.9091659785,14.335260116,6.3154417836,9.9091659785,10.569777044,32.369942197,9.9091659785,11.230388109,15.134599505,13.212221305,11.560693642,11.641930948,9.2485549133,5.2848885219,14.960897654,10.239471511,22.350674374,8.8310854207,12.449977768,9.9935773924,9.633911368,14.599504542,10.900082576,9.1410135771,8.0924855491,11.560693642,7.2667217176,13.859620149,11.230388109,15.260115607,10.019267823,9.7770437655,9.8265895954,15.854665566,7.9273327828,18.082110568,7.3988439306,23.121387283,14.863748968,3.9636663914,12.449977768,13.635689936,9.2485549133,12.401471361,7.2023121387,10.364987614,16.056518947,9.2485549133,15.414258189,17.785682526,10.569777044,12.449977768,9.9091659785,12.845215157,19.746914545,9.0173410405,11.890999174,11.230388109,11.43900213,13.747851898,23.121387283,10.276172126,23.121387283,9.5223608153,4.4194880264,13.87283237,14.377299002,17.175887696,34.682080925,13.005780347,14.450867052,8.0924855491,9.5986787779,11.560693642,11.560693642,17.341040462,9.9091659785,13.005780347,15.414258189,10.569777044,6.936416185,11.560693642,11.303789338,7.1142730102,11.890999174,10.900082576,8.5879438481,20.346820809,11.890999174,7.2667217176,8.7742700459,10.404624277,18.717313515,10.98265896,27.085053675,12.169151202,7.7071290944,8.9182493807,11.560693642,10.787778695,9.3735353851,13.212221305,20.552344252,11.071841453,15.414258189,10.751445087,17.341040462,11.689145793,40.158198966,9.4203137903,12.221304707,12.45251858,43.352601156,9.485697347,10.078553431,3.5722543353,11.890999174,13.212221305,15.260115607,14.533443435,10.019267823,16.541165443,22.512929723,8.4778420039,8.5317919075,11.316634554,12.201486375,6.521416926,13.740710157,16.184971098,22.941554271,8.5879438481,10.028561714,30.828516378,17.803468208,8.2999851786,10.789980732,9.633911368,13.87283237,19.267822736,11.230388109,15.764582239,8.5184058412,9.2485549133,12.367253663,10.789980732,15.414258189,8.6794130725,15.606936416,14.386640976,8.7861271676,9.083402147,15.414258189,8.5879438481,10.404624277,10.578034682,11.412056152,13.87283237,23.121387283,10.979355904,15.330017475,8.8631984586,10.671409515,8.0924855491,15.1940545,10.569777044,10.671409515,12.086179716,11.791907514,19.524727039,18.253726803,9.1536979398,18.473395583,11.857121684,17.065785852,16.955684008,19.618146786,9.5127993394,12.777608762,14.137076796,10.569777044,10.019267823,4.203888597,9.7999110716,8.6705202312,21.46985962,15.414258189,7.2667217176,11.560693642,16.497109827,9.7406254632,13.436829067,19.025598679,16.599970357,11.890999174,11.560693642,8.4566473988,13.87283237,12.845215157,16.76300578,9.5986787779,10.569777044,17.341040462,10.569777044,14.09840688,20.809248555,8.6606110652,2.5690430315,8.8226346212,12.716763006,19.291907514,11.560693642,8.0462427746,7.2667217176,11.248242462,9.485697347,10.623340103,8.5879438481,7.3988439306,13.212221305,15.075144509,11.560693642,11.890999174,17.175887696,11.230388109,9.063583815,13.212221305,10.569777044,10.952236082,9.1892693049,14.450867052,15.656482246,7.3568050447,6.6859344894,9.2485549133,15.854665566,13.275317919,4.6242774566,14.602981442,17.785682526,10.239471511,11.397483849,10.569777044,8.6705202312,7.6146435453,9.9091659785,12.551610239,14.602981442,8.6705202312,6.936416185,17.341040462,11.720109522,15.028901734,8.4077771939,35.466991177,15.986787779,11.649622054,11.560693642,8.5634767716,15.242774566,9.3930635838,18.497109827,9.2485549133,19.267822736,11.890999174,10.173410405,12.716763006,16.184971098,9.9091659785,13.747851898,6.2758051197,21.46985962,10.019267823,10.404624277,9.4137076796,7.1933204881,9.1098265896,17.816680429,10.536746491,15.414258189,19.524727039,9.1268634013,17.170143252,8.6705202312,9.2485549133,9.9091659785,18.497109827,11.890999174,7.2667217176,24.442609414,9.9091659785,10.800059286,9.2485549133,16.599970357,9.2485549133,14.821402105,10.569777044,15.414258189,11.890999174,10.952236082,10.019267823,13.212221305,14.797687861,9.4587493431,13.517118719,9.4181117534,8.2209377007,21.139554088,10.623340103,14.386640976,13.339261894,5.549132948,9.2485549133,16.918088256,11.230388109,11.230388109,9.3735353851,8.8928412628,8.6705202312,6.936416185,12.449977768,15.689512799,11.817597945,12.241123039,17.846060237,19.421965318,13.359023764,22.528531199,21.640115607,17.43462703,12.716763006,11.560693642,17.866526537,13.212221305,8.5879438481,24.50867052,8.5879438481,23.554913295,7.7071290944,14.450867052,11.890999174,10.173410405,9.0173410405,13.359023764,7.3988439306,9.5722543353,13.052023121,11.890999174,8.3493898523,11.560693642,6.3583815029,19.580164284,11.560693642,16.918088256,14.533443435,12.449977768,11.230388109,12.023121387,16.007114273,8.9182493807,10.609159627,17.785682526,25.763831544,12.710156895,9.2485549133,11.533542527,8.1280569142,12.912405514,9.8265895954,11.098265896,11.248242462,17.341040462,8.6705202312,13.87283237,9.3930635838,17.752087347,9.2485549133,15.414258189,8.9048586158,18.959537572,10.569777044,17.616295073,10.305532618,9.8265895954,6.2249888839,8.9349789095,12.881915772,11.421965318,9.4619831036,10.265895954,19.818331957,53.949903661,8.2576383154,21.342819031,4.161849711,17.292363858,11.230388109,14.929810074,10.239471511,17.192826441,13.212221305,9.710982659,12.881915772,10.078553431,11.2642656,9.21552436,16.515276631,9.4291907514,8.4077771939,36.608863198,12.023121387,10.503715937,10.73492981,18.497109827,29.132947977,9.8265895954,19.075144509,9.2485549133,28.901734104,8.5184058412,13.150289017,10.338563171,12.023121387,20.552344252,23.63519589,10.952236082,11.778819937,10.078553431,15.040710157,7.9273327828,8.2209377007,10.569777044,8.9710982659,20.809248555,13.359023764,16.515276631,11.239563263,10.404624277,9.2485549133,8.9916506101,11.230388109,11.560693642,20.038535645,9.1907514451,10.276172126,23.121387283,9.2341040462,12.551610239,10.239471511,9.2485549133,23.121387283,13.212221305,9.710982659,13.487475915,4.5634317006,18.497109827,17.341040462,12.74640581,9.5788604459,20.809248555,11.428571429,11.078447564,12.426094137,4.6242774566,18.971394694,9.2485549133,16.257638315,6.0115606936,10.02146986,11.230388109,18.497109827,22.658959538,10.200612037,11.230388109,23.121387283,16.441875401,12.56597135,30.057803468,9.9091659785,23.121387283,11.560693642,13.740710157,14.821402105,9.1860646774,9.485697347,18.37853861,13.212221305,13.294797688,13.212221305,16.247461334,16.167185416,13.339261894,19.442984761,9.9091659785,9.9091659785,11.873144821,10.356454721,12.845215157,9.5788604459,8.6705202312,9.7623635196,null,12.551610239,13.87283237,17.175887696,16.19818332,8.5879438481,12.845215157,12.832369942,10.952236082,11.560693642,28.901734104,20.157106862,11.618618801,23.121387283,5.3357047577,2.6424442609,19.818331957,15.1940545,8.4797687861,10.276172126,14.863748968,15.028901734,10.191664131,13.87283237,14.362785577,9.2237819983,16.515276631,9.9091659785,10.671409515,11.890999174,9.9091659785,9.7623635196,15.854665566,9.9091659785,13.122949539,12.65591725,14.22854602,13.487475915,11.560693642,18.063583815,16.515276631,null,16.662813102,11.890999174,10.597302505,10.687219011,14.847951747,19.267822736,14.797687861,17.469492614,6.936416185,11.857121684,14.643545279,16.184971098,10.655656482,15.211439002,6.5895953757,8.5879438481,7.4318744839,7.1933204881,11.2642656,8.734746307,10.173410405,9.8265895954,10.239471511,9.2485549133,19.267822736,13.042833852,10.441916838,21.579961464,11.164327002,19.818331957,22.543352601,14.450867052,9.2485549133,9.8265895954,16.184971098,11.890999174,11.857121684,11.230388109,14.821402105,9.9566473988,12.40644965,14.335260116,11.890999174,9.6581337737,8.8928412628,18.37853861,9.2369942197,9.2485549133,9.3063583815,13.212221305,8.0867052023,2.146985962,3.6333608588,12.551610239,16.184971098,16.515276631,6.9989064209,12.845215157,9.5127993394,8.7167630058,11.267822736,null,16.184971098,8.0078951079,9.485697347,38.810900083,8.8928412628,7.7071290944,11.560693642,16.184971098,5.8574181118,9.5127993394,10.434267082,8.2576383154,28.040831386,12.169151202,10.569777044,11.560693642,9.0610842056,9.9091659785,11.890999174,17.036811682,10.276172126,12.604885325,6.7052023121,11.890999174,11.910817506,11.230388109,8.8928412628,11.560693642,13.461785485,14.372754257,11.857121684,9.2485549133,14.863748968,14.599504542,12.551610239,11.593724195,9.9091659785,12.201486375,10.503715937,17.10982659,9.8959537572,10.003853565,10.900082576,9.1233140655,13.87283237,18.361101666,6.0115606936,10.276172126,9.4467382329,10.276172126,11.985627246,11.18776804,6.120367222,9.485697347,11.230388109,18.034682081,14.821402105,12.283236994,8.7486330261,9.9091659785,13.294797688,6.6061106524,9.8034682081,16.030828516,7.9273327828,19.43382244,12.845215157,12.169151202,12.845215157,8.4481991996,9.5260115607,17.836498761,26.011560694,12.145528732,13.042833852,10.349573355,9.6184971098,8.1604896294,10.272502064,10.555415934,8.9916506101,21.676300578,13.635689936,15.028901734,17.341040462,9.485697347,21.965317919,11.890999174,9.3476465731,9.6547414466,11.560693642,17.517493155,18.819733835,11.857121684,10.75413362,6.5960179833,8.7486330261,9.485697347,10.789980732,10.671409515,7.3988439306,12.023121387,10.078553431,11.560693642,11.817597945,13.042833852,16.515276631,9.083402147,13.579128261,23.121387283,9.4335260116,14.533443435,9.9091659785,12.551610239,14.606110652,10.4596752,16.184971098,9.1268634013,12.881915772,11.271676301,12.312138728,13.56038119,8.3630549748,15.1940545,9.9091659785,7.1466106148,11.010184421,9.9091659785,10.343778521,9.843104872,18.497109827,10.556564822,16.515276631,10.648007301,11.092016872,24.046242775,17.98330122,31.306358382,8.9145793192,6.936416185,12.449977768,13.454445362,7.9099482811,22.307514451,9.4919379373,12.74640581,12.551610239,8.6705202312,10.184420589,12.551610239,8.9332632685,19.752270851,10.701899257,12.386457473,10.019267823,9.7770437655,9.4137076796,9.9091659785,10.110920169,9.633911368,15.819896562,11.890999174,8.6705202312,10.569777044,11.230388109,11.560693642,15.640938456,27.231856134,19.157720892,9.8265895954,11.086408774,10.597302505,10.4596752,17.036811682,8.323699422,9.442476226,12.572254335,15.141205615,9.2485549133,6.936416185,8.323699422,10.107349298,7.5309661437,28.901734104,17.572254335,8.6705202312,10.569777044,14.450867052,12.221304707,11.890999174,11.976878613,10.173410405,15.260115607,19.250206441,13.87283237,10.404624277,10.248398688,9.3735353851,11.890999174,9.4026974952,17.036811682,5.7803468208,13.324525186,10.078553431,14.393063584,15.414258189,9.9091659785,9.2485549133,8.8928412628,6.8336544637,22.232103157,13.640669927,29.555739059,8.8423683799,15.769971839,14.997656616,8.0924855491,8.9182493807,12.331406551,13.740710157,16.13120043,8.7736291204,20.231213873,11.890999174,9.633911368,12.551610239,11.032204789,5.7803468208,13.87283237,8.8081475365,14.533443435,8.2999851786,13.212221305,12.49804718,20.038535645,9.4467382329,16.421965318,11.560693642,17.341040462,23.121387283,11.560693642,11.132519803,10.276172126,9.485697347,15.854665566,25.690430315,9.9091659785,22.44059088,10.078553431,18.497109827,12.716763006,9.2485549133,16.515276631,8.8928412628,10.789980732,9.9091659785,7.4988283081,8.1237306671,12.49804718,10.569777044,19.564250778,13.212221305,12.947976879,12.716763006,9.9550417469,10.276172126,10.878612717,19.075144509,9.9599822143,9.3735353851,39.739884393,25.089274245,12.672298799,12.404624277,10.404624277,4.6242774566,15.801288192,9.9091659785,5.3716354294,7.2667217176,15.1940545,9.9091659785,19.818331957,16.184971098,18.122168411,12.551610239,8.9916506101,10.597302505,10.305532618,11.873144821,25.176621708,11.946050096,15.974776668,23.121387283,10.014450867,20.970560559,10.967837557,10.671409515,21.139554088,9.8265895954,12.367253663,10.671409515,8.2043632295,8.8928412628,23.121387283,36.477842004,18.74707077,16.247461334,12.169151202,10.98265896,11.560693642,12.449977768,14.524974063,9.9091659785,13.87283237,6.936416185,10.671409515,24.338302403,11.175337187,17.891549683,14.450867052,16.698779705,7.2667217176,3.506743738,7.7071290944,9.9091659785,12.331406551,9.485697347,10.078553431,12.716763006,12.881915772,41.040462428,11.98886748,11.83044316,9.9091659785,13.994523882,18.497109827,15.854665566,12.011264266,9.2485549133,12.427745665,14.467382329,9.9091659785,29.642804209,10.63583815,13.212221305,11.230388109,5.2023121387,7.8705202312,24.613089689,13.747851898,12.716763006,9.633911368,11.230388109,9.3735353851,23.121387283,27.938342967,8.7266721718,9.633911368,35.672997523,10.671409515,19.075144509,14.372754257,15.028901734,9.2485549133,10.29672447,13.294797688,72.667217176,8.8081475365,11.271676301,9.0173410405,6.936416185,9.7353209614,13.87283237,9.2485549133,8.6705202312,10.150289017,16.515276631,16.815554388,10.648007301,13.212221305,9.2485549133,12.524084778,21.579961464,9.4203137903,9.9599822143,14.713610089,22.375536081,9.633911368,15.1940545,11.560693642,9.633911368,8.323699422,9.8045692265,13.359023764,4.3336085879,24.046242775,8.5152766309,11.890999174,10.569777044,9.4181117534,11.890999174,15.414258189,12.815854666,12.169151202,4.6903385632,11.890999174,8.6705202312,10.276172126,16.659896891,18.063583815,9.4919379373,9.2485549133,12.881915772,7.9273327828,11.560693642,20.552344252,10.197748707,18.928709056,12.023121387,13.052396047,10.569777044,7.0134874759,7.7071290944,9.2485549133,8.4659848822,9.1816245817,11.890999174,14.196531792,11.560693642,8.1206823629,6.6795118818,23.121387283,9.633911368,12.551610239,16.056518947,14.533443435,13.600816049,12.904960344,3.9306358382,16.441875401,16.007114273,18.497109827,7.8612716763,14.533443435,14.277456647,9.2485549133,18.122168411,10.900082576,14.22854602,16.815554388,11.230388109,9.6787202581,13.517118719,11.230388109,14.863748968,11.857121684,10.305532618,10.259289843,3.4748142031,8.4778420039,14.997656616,8.9182493807,14.637616719,10.019267823,13.87283237,10.900082576,13.212221305,14.713610089,15.593493749,9.9091659785,11.316267547,7.9099482811,5.549132948,9.1110763943,10.509721492,9.8265895954,11.857121684,8.1814139618,5.85541626,9.4297765974,10.757529662,16.007114273,8.3677401596,21.676300578,9.5054592164,9.2485549133,10.952236082,12.1552436,9.7169112198,17.98330122,11.010184421,6.0115606936,19.611890999,12.268491212,16.515276631,9.5869166784,12.704905884,10.115606936,8.5879438481,11.349298101,19.267822736,9.2485549133,10.741535921,17.469492614,13.212221305,5.9944337401,11.560693642,19.075144509,43.159922929,8.2576383154,8.5448605177,9.4577484173,4.6242774566,22.543352601,12.936416185,13.212221305,13.042833852,17.341040462,13.063583815,16.056518947,13.212221305,13.040462428,8.0924855491,13.212221305,9.9091659785,7.7071290944,4.9545829893,7.7071290944,14.84768005,7.7071290944,8.2209377007,8.7486330261,11.560693642,7.2667217176,8.7861271676,15.55933356,21.579961464,9.2419488026,9.9091659785,9.2485549133,23.121387283,11.248242462,9.2485549133,20.231213873,9.4167104572,15.1940545,9.1268634013,12.023121387,22.543352601,10.860445912,7.9273327828,17.785682526,13.212221305,10.374981473,10.404624277,8.455821635,13.410404624,21.965317919,14.386640976,6.936416185,16.845582164,11.857121684,22.543352601,16.184971098,12.551610239,24.351445087,12.881915772,11.230388109,21.271676301,15.1940545,12.551610239,11.560693642,11.857121684,8.4778420039,15.1940545,16.346820809,13.740710157,21.019442985,17.785682526,7.2667217176,8.2209377007,17.341040462,17.175887696,7.5589150734,9.7353209614,2.3517753922,10.63583815,7.8257003112,21.374438022,8.5879438481,14.313239747,12.793834297,19.267822736,13.212221305,9.2485549133,8.1078998073,12.023121387,7.3810582481,12.65591725,22.328654005,8.8081475365,9.9091659785,10.276172126,13.042833852,17.175887696,13.997812842,10.12716763,13.212221305,10.520231214,17.308009909,12.716763006,13.87283237,9.9091659785,20.552344252,9.1907514451,6.936416185,2.697495183,9.559042114,10.949628406,13.87283237,18.497109827,9.2485549133,10.779565693,8.8928412628,10.880652839,10.569777044,14.543352601,23.121387283,9.5524360033,12.716763006,10.305532618,10.569777044,7.2667217176,7.9823837049,20.231213873,19.737769632,9.9984377441,9.2485549133,12.524084778,19.322873658,13.212221305,8.6705202312,8.8786127168,18.74707077,10.404624277,9.2742453436,12.551610239,17.836498761,11.2642656,14.533443435,8.1237306671,11.560693642,12.094264117,16.184971098,13.87283237,7.7071290944,10.184420589,11.278725504,17.809552784,17.836498761,20.231213873,27.502890173,20.809248555,20.231213873,11.758876961,12.551610239,10.73492981,12.551610239,15.819896562,8.8928412628,9.2485549133,8.734746307,13.699421965,26.336705202,9.5390543945,10.115606936,11.560693642,12.449977768,8.6705202312,12.331406551,11.230388109,23.97773496,7.9273327828,13.042833852,14.171172851,19.010918433,7.7071290944,16.815554388,9.2722691567,9.2485549133,13.122949539,8.6705202312,6.1436829067,17.036811682,18.497109827,13.534904402,23.121387283,15.455202312,10.671409515,10.569777044,14.450867052,17.192826441,7.9273327828,24.99609436,19.818331957,9.2485549133,9.2485549133,11.560693642,16.515276631,8.7861271676,8.8323699422,10.173410405,12.221304707,7.7071290944,8.7861271676,9.2485549133,18.497109827,9.2485549133,12.331406551,12.611665791,16.61849711,7.5309661437,15.295686972,23.714243367,7.7071290944,14.821402105,18.966763006,4.617671346,14.797687861,6.4226075787,9.2485549133,18.497109827,20.749962946,11.230388109,8.4778420039,12.947976879,13.87283237,7.1142730102,12.723988439,10.569777044,6.936416185,18.09017341,8.0924855491,7.8612716763,7.7886044591,10.894797688,9.2485549133,9.9091659785,11.890999174,5.2848885219,14.777869529,12.235067437,32.113037893,12.245771783,8.9182493807,11.108542068,13.294797688,14.931554765,13.212221305,12.22864483,8.2209377007,6.1849710983,7.2667217176,8.734746307,15.1940545,26.245899078,9.9091659785,7.8951078528,5.681255161,9.0474993717,14.518080387,50.096339114,10.276172126,7.5144508671,10.239471511,11.560693642,16.872363693,19.858702633,9.485697347,11.560693642,6.2758051197,14.386640976,19.752270851,9.9091659785,8.9111076394,22.070415134,12.716763006,10.569777044,9.5788604459,15.1940545,9.51940545,10.73492981,15.622558975,8.6705202312,null,13.452996653,13.042833852,6.612716763,8.0924855491,5.2023121387,22.020368841,11.909601015,9.8959537572,14.533443435,9.485697347,10.115606936,10.305532618,13.410404624,17.192826441,10.115606936,9.4075144509,11.729874524,10.467682606,18.497109827,11.849710983,9.2485549133,15.606936416,10.019267823,9.2485549133,10.404624277,8.6705202312,10.019267823,19.774870703,5.2023121387,10.48528028,14.347758163,16.405174787,15.306358382,20.260941371,23.121387283,25.103220479,25.690430315,12.758051197,12.300578035,6.936416185,3.1529164477,9.2485549133,25.690430315,7.5669994745,14.181117534,10.569777044,11.890999174,18.034682081,9.9091659785,9.668943773,12.182080925,14.401321222,11.314721436,10.671409515,9.485697347,7.9273327828,null,10.900082576,12.777608762,17.341040462,22.543352601,14.797687861,31.791907514,null,8.9578860446,16.647398844,9.485697347,7.9273327828,12.023121387,10.671409515,11.560693642,10.404624277,6.0556014313,15.854665566,13.212221305,9.9091659785,10.343778521,6.521416926,11.857121684,11.560693642,18.190751445,12.716763006,8.9502144322,9.2485549133,5.9454995871,17.175887696,11.560693642,9.9091659785,16.007114273,9.4137076796,20.194880264,27.38150289,10.714789229,18.063583815,9.2485549133,13.717288492,13.994523882,13.386066322,10.509721492,16.76300578,10.569777044,19.267822736,14.533443435,9.9091659785,6.6930331609,11.116051578,9.2485549133,25.643063584,12.551610239,11.560693642,12.716763006,14.277456647,8.9182493807,15.414258189,9.2485549133,9.9091659785,null,10.569777044,13.510389002,10.569777044,10.569777044,18.801338607,10.886870355,9.710982659,9.9091659785,11.560693642,29.642804209,9.8265895954,9.5054592164,12.138728324,15.710686231,10.477639185,18.959537572,8.6705202312,12.283236994,10.078553431,9.2485549133,10.576170054,11.560693642,7.1142730102,9.9984377441,9.4467382329,6.7437379576,9.7968620974,24.112303881,11.560693642,19.602915305,7.9273327828,8.7861271676,8.7486330261,12.97053433,11.890999174,7.9273327828,10.019267823,10.404624277,11.857121684,8.2209377007,10.623340103,10.272502064,12.023121387,9.2485549133,11.560693642,9.2485549133,15.819896562,10.926337632,13.87283237,null,11.387283237,12.845215157,22.496484924,10.02807597,13.212221305,15.260115607,7.7071290944,11.560693642,9.4137076796,23.121387283,9.2485549133,15.1940545,11.890999174,9.8761354253,41.288191577,11.421965318,16.515276631,5.8959537572,21.800165153,7.9273327828,19.653179191,9.2485549133,17.341040462,10.792100193,10.623340103,12.25433526,11.230388109,11.164327002,24.171758877,25.048169557,9.5205712343,10.023433838,9.4587493431,7.3568050447,9.6136294493,11.329479769,17.341040462,12.111202863,11.230388109,20.550289017,11.560693642,9.2485549133,12.449977768,15.1940545,12.109000826,10.404624277,11.873144821,25.433526012,13.122949539,16.942838793,15.414258189,11.230388109,12.138728324,13.487475915,11.560693642,8.8405304318,8.8928412628,13.87283237,14.599504542,9.6279828072,9.0944123314,14.284813452,11.560693642,14.533443435,14.037985136,17.206613792,12.046242775,9.0474993717,6.8178449681,7.2667217176,9.746554024,51.527663088,19.818331957,9.9091659785,9.2485549133,8.5879438481,12.331406551,11.873144821,11.230388109,10.239471511,14.258188825,6.6061106524,10.276172126,9.6647398844,10.470685384,16.74307355,10.078553431,30.158331239,7.9273327828,10.222087009,10.404624277,17.175887696,14.258188825,11.560693642,11.230388109,8.8928412628,9.710982659,10.671409515,10.239471511,23.746289642,10.671409515,9.9190751445,14.060303078,11.560693642,9.3036058354,11.890999174,7.2667217176,9.4335260116,18.497109827,13.212221305,13.4746307,9.1512017037,24.277456647,8.9916506101,11.560693642,27.052023121,11.2642656,10.952236082,16.247461334,15.414258189,8.0924855491,31.791907514,10.415634462,4.6242774566,13.149547947,13.212221305,16.184971098,11.855491329,16.61849711,21.800165153,20.231213873,34.682080925,12.169151202,8.323699422,12.023121387,7.5970272502,11.40655106,9.5788604459,23.506743738,11.560693642,17.341040462,8.901734104,10.503715937,8.3493898523,9.6787202581,9.6779521057,13.597577759,14.821402105,9.485697347,13.212221305,9.4735197625,5.9454995871,9.823625315,7.7071290944,10.900082576,11.230388109,10.173410405,18.786127168,10.343778521,12.49804718,8.5879438481,15.775392238,17.192826441,9.3278282411,9.3735353851,7.0064809949,21.139554088,26.166804294,13.005780347,8.8928412628,15.817400326,15.854665566,13.05421028,13.212221305,8.6705202312,10.404624277,9.485697347,15.1940545,11.560693642,6.1657032755,11.230388109,22.020368841,9.3735353851,7.8447563997,13.294797688,22.350674374,16.61089139,10.404624277,20.809248555,4.1890668869,10.789980732,8.5879438481,12.551610239,11.560693642,7.9273327828,11.230388109,16.515276631,8.5964132207,1.5414258189,9.710982659,17.271676301,9.485697347,8.323699422,10.276172126,7.4810533076,9.0229804032,9.4587493431,23.121387283,11.184145334,25.433526012,10.671409515,16.335762754,12.449977768,8.1237306671,10.867052023,9.083402147,10.63583815,9.2485549133,11.881824021,14.450867052,9.633911368,21.019442985,16.71345995,11.560693642,10.404624277,9.4797687861,15.028901734,10.509721492,13.810342134,18.122168411,8.9916506101,11.329479769,12.716763006,12.994219653,17.036811682,36.416184971,17.341040462,10.539968984,24.08477842,11.248242462,8.7742700459,10.789980732,7.8612716763,10.327552987,9.9984377441,18.917498686,20.809248555,21.246680206,13.410404624,13.097585855,13.87283237,17.10982659,10.086705202,5.0392767156,15.414258189,5.549132948,18.497109827,12.221304707,null,11.132519803,7.1933204881,6.2620423892,3.4682080925,9.5788604459,15.458298927,11.164327002,10.078553431,9.2485549133,28.901734104,15.1940545,23.714243367,9.485697347,7.9273327828,7.7842003854,23.121387283,15.028901734,22.478790574,10.305532618,13.294797688,7.0156895128,15.1940545,5.9454995871,9.2485549133,9.9091659785,21.965317919,9.2485549133,14.612716763,10.200612037,21.836865768,11.514450867,1.874707077,8.7090558767,11.230388109,13.87283237,9.485697347,7.7379576108,16.515276631,8.5448605177,8.774566474,12.28241123,4.9876135425,11.890999174,11.560693642,10.882997807,7.9273327828,14.643545279,8.5964132207,13.87283237,15.133998949,25.433526012,9.2485549133,12.551610239,8.4668318194,23.121387283,8.1237306671,9.9091659785,11.890999174,10.63583815,10.630461083,13.122949539,16.872363693,10.569777044,13.747851898,17.488176563,8.6705202312,12.551610239,9.6017983301,16.548307184,14.863748968,21.271676301,7.8034682081,16.007114273,8.1888246628,9.1268634013,8,11.098265896,16.955684008,15.211439002,11.963835779,9.2485549133,9.6596017983,16.515276631,9.3930635838,19.267822736,11.092016872,12.449977768,9.5305230509,5.0841288192,9.3221229637,5.6151940545,14.450867052,15.028901734,11.248242462,20.552344252,12.296374146,16.007114273,14.533443435,6.1271676301,11.560693642,10.714789229,10.503715937,27.74566474,33.030553262,10.569777044,14.599504542,9.633911368,9.485697347,11.157720892,13.87283237,9.9091659785,9.9842354178,13.212221305,10.404624277,11.560693642,8.0924855491,7.4988283081,8.5184058412,11.560693642,17.341040462,11.857121684,12.49804718,14.821402105,7.9273327828,10.714789229,11.303789338,11.230388109,11.560693642,14.112019135,9.9091659785,7.0064809949,14.450867052,10.404624277,11.572550763,11.857121684,10.767960363,15.854665566,16.515276631,7.179799209,7.7071290944,20.038535645,5.4403264196,23.714243367,6.6853839802,14.863748968,11.890999174,8.9916506101,16.599970357,13.212221305,12.551610239,32.755298651,26.245899078,18.497109827,19.695218077,15.028901734,12.25433526,9.6104548882,10.893476466,9.2485549133,17.836498761,13.815028902,18.497109827,11.175337187,16.515276631,6.521416926,5.6241212311,10.820809249,8.6705202312,7.5144508671,17.341040462,18.497109827,8.5184058412,10.184420589,4.5317919075,8.4778420039,9.9091659785,12.845215157,10.173410405,null,26.358381503,9.5788604459,10.115606936,13.87283237,10.671409515,7.7071290944,9.9091659785,25.895953757,8.734746307,38.535645472,12.845215157,12.708199529,11.037709882,11.098265896,10.019267823,23.121387283,10.338563171,23.121387283,17.175887696,11.560693642,8.1791907514,13.899256813,11.560693642,22.398843931,10.671409515,21.296014603,9.4104046243,12.551610239,5.7803468208,10.98265896,10.73492981,14.997656616,18.497109827,19.653179191,16.488852188,10.239471511,11.818331957,11.408753097,12.169151202,8.0924855491,14.533443435,7.7071290944,8.6705202312,3.8645747316,6.936416185,8.8928412628,13.810342134,22.093770071,13.294797688,11.817597945,19.818331957,11.890999174,17.726396917,8.2209377007,18.392012612,14.129736673,12.339519319,17.919075145,8.8928412628,9.9091659785,9.1586384072,10.404624277,8.6705202312,19.818331957,11.637764933,12.73731535,9.2485549133,8.6705202312,11.230388109,30.057803468,6.4226075787,10.404624277,10.900082576,16.599970357,19.996875488,15.682332244,11.2642656,12.551610239,28.406275805,16.515276631,26.204238921,9.5406145421,11.230388109,12.485549133,19.818331957,19.357440516,13.102119461,13.212221305,25.690430315,11.046885035,13.534470605,7.9273327828,22.196531792,8.5879438481,12.122213047,15.414258189,9.3573614417,11.375722543,8.1604896294,15.414258189,10.671409515,11.132519803,13.212221305,5.7803468208,10.310888924,10.569777044,18.971394694,7.8420038536,10.007707129,13.212221305,20.512820513,8.6705202312,9.485697347,23.121387283,9.1268634013,15.1940545,9.0173410405,15.414258189,9.9984377441,11.100986059,7.2667217176,9.9842354178,13.87283237,10.404624277,6.936416185,9.9091659785,13.747851898,24.971098266,10.270763614,10.569777044,9.2485549133,8.0035571365,10.543352601,9.633911368,10.305532618,11.157720892,9.9091659785,10.767960363,11.857121684,6.0676125416,11.751445087,8.0924855491,8.8631984586,10.276172126,26.718047527,17.175887696,21.965317919,12.845215157,12.598191789,17.341040462,10.276172126,7.9273327828,10.078553431,8.4361818466,10.305532618,10.404624277,8.9916506101,7.9273327828,9.9091659785,9.9091659785,11.2642656,8.4778420039,8.7655748234,18.497109827,16.515276631,11.560693642,5.809989625,2.774566474,8.2999851786,10.77246453,25.433526012,4.9045366964,15.854665566,13.212221305,25.620996719,7.9273327828,15.819896562,24.046242775,16.515276631,10.569777044,9.5788604459,7.1345995045,11.560693642,23.121387283,7.9273327828,32.369942197,6.936416185,8.0924855491,19.774870703,10.02807597,11.890999174,6.612716763,10.019267823,12.331406551,9.2485549133,11.069364162,13.87283237,13.87283237,16.76300578,10.057803468,10.437654831,6.5862923204,10.434267082,21.800165153,14.129736673,14.3512059,9.2485549133,22.452083967,17.747226996,10.239471511,14.533443435,9.9091659785,6.5510597303,7.9273327828,26.011560694,10.404624277,17.98330122,17.836498761,13.179190751,9.7623635196,14.386640976,23.121387283,13.87283237,12.221304707,6.5400495458,15.854665566,41.983571646,15.606936416,6.1657032755,8.4778420039,9.8791382028,11.873144821,8.8928412628,12.660521793,9.2485549133,9.8265895954,14.713610089,21.296014603,9.4310921813,16.515276631,15.414258189,27.06894121,10.276172126,10.085924074,8.5879438481,14.797687861,3.7115911165,8.5879438481,19.157720892,8.8928412628,10.569777044,9.9842354178,6.936416185,9.0077071291,6.1657032755,10.789980732,14.216528667,8.2999851786,11.560693642,11.175337187,10.07262487,9.2485549133,6.8739259491,12.551610239,9.9984377441,10.272502064,14.533443435,10.952236082,19.737769632,14.213872832,9.2485549133,9.5788604459,9.6184971098,9.9091659785,8.135302933,16.515276631,9.5127993394,19.818331957,6.6061106524,11.890999174,6.5864708639,9.161849711,18.402736817,12.947976879,23.63519589,9.2485549133,12.777608762,13.843930636,7.9768786127,17.785682526,11.873144821,10.967837557,10.404624277,18.497109827,19.818331957,3.5571365051,16.184971098,8.6705202312,7.077975699,10.404624277,8.5879438481,19.041142469,17.469492614,14.602981442,16.441875401,10.693641618,14.037985136,14.863748968,13.212221305,8.3967143292,13.87283237,13.172768144,9.6960656349,17.341040462,9.9091659785,19.267822736,7.5144508671,15.854665566,14.69492614,24.776391847,13.122949539,10.078553431,6.6061106524,8.9502144322,10.918432884,10.671409515,8.7486330261,15.519075145,19.421965318,12.526837325,4.9285062367,9.9984377441,16.515276631,13.212221305,9.1877091573,21.213872832,18.717313515,24.371192001,14.797687861,11.491954382,13.616845582,10.569777044,9.5223608153,10.569777044,8.4361818466,16.408726459,13.212221305,10.181668043,9.3735353851,11.560693642,11.560693642,5.2023121387,14.821402105,13.87283237,9.8265895954,23.121387283,11.2642656,10.520231214,8.2543352601,15.1940545,11.560693642,19.127693116,9.2742453436,12.449977768,9.2485549133,14.797687861,18.063583815,20.644095789,9.6837810269,9.2485549133,15.1940545,13.87283237,8.6833654464,13.87283237,16.515276631,11.857121684,11.046885035,10.509721492,15.1940545,10.090834021,13.615928067,7.7071290944,7.5970272502,15.414258189,17.803468208,11.230388109,1.2386457473,13.87283237,11.890999174,16.069364162,100.19267823,12.866193229,8.0154142582,13.042833852,9.2485549133,12.221304707,8.2832369942,11.223781998,14.188124015,8.5879438481,12.331406551,8.5772888309,7.6738009686,14.821402105,11.890999174,10.239471511,9.8908156712,12.221304707,7.9273327828,13.212221305,7.5144508671,8.5879438481,11.560693642,9.9025598679,10.659552394,11.560693642,11.230388109,14.821402105,13.304706854,13.87283237,21.246680206,11.890999174,9.2485549133,8.5879438481,8.9595375723,9.5638465581,28.901734104,10.63583815,11.890999174,10.98265896,8.3630549748,15.995257151,27.32527588,8.4161849711,14.170107349,13.87283237,15.722543353,5.2023121387,10.648007301,10.22625929,12.551610239,12.809248555,2.8802642444,19.826589595,17.341040462,8.612716763,11.288677321,12.947976879,11.230388109,12.169151202,11.341811175,9.9091659785,23.121387283,10.173410405,10.672345604,19.77135517,17.175887696,8.8226346212,2.6424442609,13.87283237,5.5876685934,8.1237306671,14.771997431,9.8761354253,10.63583815,10.078553431,11.2642656,10.4596752,8.6429947702,9.1084252934,16.515276631,9.2485549133,9.6184971098,10.63583815,7.5144508671,10.789980732,12.185596001,11.560693642,10.374981473,11.890999174,14.797687861,29.727497936,12.005335705,13.87283237,12.723369116,11.667407737,14.821402105,12.551610239,11.857121684,17.341040462,17.341040462,13.87283237,23.121387283,11.230388109,8.2576383154,13.87283237,9.5568400771,8.9595375723,9.4123314066,11.911017691,12.386457473,15.117830147,10.100395497,10.404624277,11.230388109,10.623340103,17.374071016,15.654539272,10.952236082,11.494632535,16.429397192,11.857121684,9.868884816,13.690295102,16.732582902,18.497109827,6.1657032755,12.690338563,11.890999174,12.111202863,9.9686209744,17.190751445,7.5838150289,10.078553431,26.424442609,9.2485549133,13.212221305,10.404624277,15.433526012,4.6965317919,11.890999174,11.817597945,2.7800715662,11.560693642,6.936416185,8.0924855491,7.8612716763,14.533443435,9.485697347,15.1940545,11.857121684,10.671409515,13.762730526,13.212221305,9.3930635838,6.6628131021,24.855491329,12.551610239,10.05277708,26.589595376,20.231213873,9.2485549133,11.098265896,9.2485549133,12.881915772,9.4211725846,20.552344252,16.599970357,10.901734104,12.551610239,18.034682081,15.1940545,7.5144508671,17.175887696,14.821402105,14.22854602,16.955684008,19.075144509,13.209613629,7.5144508671,8.6353355114,21.800165153,10.404624277,13.901734104,17.341040462,13.87283237,12.449977768,15.709331131,11.857121684,10.952236082,11.560693642,12.290301863,17.341040462,21.46985962,8.9595375723,15.689512799,2.7525461051,8.0035571365,11.560693642,10.98265896,6.7437379576,15.974776668,19.77135517,18.74707077,10.404624277,23.121387283,10.900082576,24.575465639,9.2485549133,11.393063584,13.549132948,19.075144509,16.515276631,14.771997431,9.485697347,12.485549133,6.4226075787,7.8034682081,8.8928412628,13.212221305,15.1940545,16.007114273,21.019442985,10.078553431,10.789980732,13.87283237,10.671409515,16.515276631,9.9091659785,13.042833852,21.139554088,15.028901734,8.2576383154,11.549414916,10.305532618,20.809248555,7.7071290944,15.746257596,7.7023121387,8.1206823629,6.1657032755,9.4181117534,15.1940545,10.276172126,9.1522157996,11.890999174,8.0924855491,13.635689936,14.900449583,9.9091659785,21.786952931,6.521416926,11.774121832,11.560693642,21.761305678,16.698779705,9.2485549133,24.260329694,19.267822736,10.078553431,21.139554088,18.166804294,8.2369942197,9.5788604459,10.75413362,10.996757366,12.461210831,19.157720892,7.1933204881,25.488576934,10.276172126,11.560693642,4.4958253051,17.341040462,8.4161849711,8.7134599505,11.410717075,13.810342134,7.3217726397,10.837409219,8.9182493807,15.854665566,12.881915772,14.533443435,9.7821253891,15.819896562,10.078553431,11.145694383,11.2642656,11.857121684,15.414258189,10.63583815,8.9502144322,19.818331957,43.352601156,9.2485549133,26.485549133,9.485697347,18.497109827,9.9091659785,31.791907514,9.2485549133,9.9091659785,7.9273327828,10.019267823,12.644508671,16.007114273,10.966143683,11.946050096,3.4682080925,8.9182493807,27.167630058,14.073887912,13.31231389,5.4995871181,16.515276631,10.276172126,2.6085667704,25.763831544,4.6242774566,5.1519193716,10.404624277,8.6705202312,15.622558975,9.7862615943,14.22854602,15.96476741,11.824938068,5.0446663163,14.323402994,14.129736673,23.121387283,10.952236082,9.9091659785,8.9916506101,15.028901734,15.235342692,10.671409515,13.87283237,10.019267823,6.6061106524,17.98330122,15.028901734,10.789980732,22.460776218,8.323699422,18.497109827,20.552344252,9.9091659785,6.936416185,16.515276631,8.3238150289,12.169151202,9.2485549133,9.0474993717,16.515276631,9.2485549133,28.901734104,10.140379851,8.1567116249,11.560693642,16.647398844,15.1940545,14.533443435,15.414258189,19.010918433,10.701899257,13.87283237,14.450867052,12.138728324,9.5696852922,13.87283237,9.9091659785,15.622558975,15.622558975,16.845582164,6.6061106524,30.828516378,12.845215157,8.9202312139,17.98330122,3.3030553262,9.2485549133,6.936416185,15.405450041,15.1940545,18.416184971,11.626754748,8.4778420039,7.179799209,11.560693642,9.0173410405,13.068610204,34.682080925,11.857121684,9.0610842056,13.87283237,8.6705202312,7.0671290944,32.759884393,19.075144509,9.6184971098,11.230388109,14.450867052,9.9285957157,11.890999174,9.9091659785,9.9091659785,12.449977768,10.789980732,18.497109827,7.2789552558,null,9.2485549133,11.890999174,null,15.854665566,12.280759703,11.857121684,8.5879438481,25.555217524,6.5510597303,31.791907514,20.809248555,11.873144821,14.450867052,11.560693642,20.157106862,14.473988439,10.623340103,13.245251858,11.857121684,9.3735353851,16.289017341,16.955684008,16.599970357,7.5970272502,9.1410135771,16.383154418,13.87283237,10.754409367,4.293971924,11.230388109,10.569777044,9.063583815,14.821402105,11.817597945,28.901734104,9.485697347,9.1164327002,7.8951078528,10.078553431,14.385252304,11.890999174,21.151787626,16.473988439,8.9916506101,8.8928412628,26.424442609,10.265895954,10.05277708,11.065235343,11.613542527,15.310107796,13.212221305,9.2485549133,9.1151622944,8.4227910818,26.424442609,4.8117481643,11.873144821,10.276172126,9.5722543353,18.063583815,12.716763006,9.9091659785,14.269199009,12.845215157,10.378933847,6.2758051197,19.470641923,8.0422216637,11.685193419,11.857121684,13.042833852,19.653179191,13.842409492,5.6151940545,13.487475915,9.4401321222,28.406275805,9.7353209614,15.1940545,18.497109827,15.028901734,16.247461334,11.560693642,11.248242462,19.075144509,15.945784333,23.121387283,9.0558766859,13.102119461,10.377098816,9.7999110716,15.260115607,8.323699422,9.2485549133,23.121387283,17.506193229,13.212221305,11.560693642,17.341040462,16.184971098,null,22.496484924,10.677126342,12.023121387,18.625561978,8.7486330261,7.4318744839,12.49804718,11.000912686,9.6647398844,21.031898951,9.3586567575,9.3608587944,6.936416185,11.725846408,10.569777044,11.291840301,13.212221305,9.083402147,6.8042939719,7.8998073218,10.487068538,15.211439002,13.377374071,9.5788604459,9.9091659785,11.098265896,9.9091659785,17.469492614,10.417836499,8.8226346212,null,4.4464206314,13.747851898,10.946325351,15.1940545,9.9091659785,10.404624277,14.739884393,18.497109827,8.323699422,12.551610239,20.749962946,5.9454995871,26.011560694,9.2485549133,13.635689936,11.230388109,12.449977768,11.278725504,7.9273327828,10.569777044,19.267822736,23.121387283,13.701073493,9.2303011865,13.87283237,18.076720967,13.87283237,9.5953757225,9.2485549133,11.058054788,10.239471511,21.676300578,9.2485549133,19.616671737,6.4989845337,9.9091659785,7.6057195011,13.212221305,9.9091659785,12.716763006,8.4778420039,11.600330306,16.515276631,9.9006966059,9.2485549133,39.665202312,11.572254335,13.635689936,10.569777044,9.9091659785,7.7071290944,10.623340103,9.9091659785,10.807597027,12.881915772,14.533443435,6.0670520231,17.175887696,15.622558975,15.414258189,7.225433526,19.818331957,4.9545829893,13.212221305,16.515276631,13.747851898,16.12716763,5.7803468208,20.809248555,23.121387283,10.838150289,8.9048586158,12.551610239,13.994523882,18.497109827,8.0924855491,11.303789338,9.1268634013,18.253726803,8.7583815029,7.5144508671,14.3512059,12.904960344,17.341040462,9.407101569,13.615928067,14.450867052,10.208092486,11.560693642,21.271676301,17.10982659,11.248242462,16.515276631,10.452052764,14.894475064,9.4335260116,13.87283237,13.87283237,8.323699422,16.776448447,21.46985962,23.121387283,13.212221305,30.057803468,9.9091659785,6.1657032755,10.239471511,11.560693642,2.8728323699,15.028901734,10.789980732,13.87283237,9.789430223,10.305532618,13.87283237,12.924262635,11.560693642,12.49804718,27.74566474,9.7366730893,12.49804718,7.5669994745,2.802592398,14.335260116,23.121387283,13.600816049,5.500087581,8.734746307,6.0115606936,14.997656616,6.936416185,12.845215157,11.248242462,9.2485549133,14.797687861,6.3583815029,2.8901734104,7.4988283081,11.873144821,4.6242774566,17.341040462,6.0115606936,15.764582239,9.2485549133,8.8226346212,21.076033793,7.7071290944,5.7803468208,5.9454995871,6.0471320587,10.343778521,11.098265896,6.5510597303,12.138728324,10.952236082,9.8312138728,6.8641618497,26.815169886,5.7803468208,13.102119461,12.49804718,12.661712084,7.3731535003,6.936416185,7.7023121387,8.0924855491,11.560693642,14.372754257,7.4988283081,6.8850353243,7.7071290944,6.4226075787,6.6061106524,8.7486330261,14.129736673,13.212221305,4.1288191577,16.184971098,8.8081475365,14.372754257,12.551610239,8.9916506101,12.845215157,9.0173410405,5.9375722543,10.569777044,13.122949539,10.509721492,8.6705202312,6.936416185,10.623340103,9.2485549133,8.536166224,7.7071290944,5.3641618497,11.560693642,10.789980732,17.175887696,7.225433526,17.341040462,8.6705202312,8.0924855491,6.0115606936,9.2485549133,8.6705202312,10.714789229,8.1888246628,6.5028901734,7.3859987155,10.952236082,9.7353209614,13.87283237,6.0693641618,10.597302505,7.4988283081,8.7486330261,5.3949903661,12.661712084,10.115606936,8.5879438481,7.7071290944,5.549132948,13.122949539,8.1237306671,9.2485549133,6.936416185,8.323699422,9.7225433526,8.8928412628,10.789980732,6.2620423892,3.5581245986,1.0276172126,6.936416185,6.997261941,5.9537572254,10.276172126,9.2922980784,11.035207567,6.0471320587,14.450867052,7.9273327828,6.521416926,8.6705202312,7.8112794876,16.524084778,12.845215157,11.560693642,8.9267301984,13.487475915,6.3783137333,4.6242774566,23.121387283,5.7768786127,8.8928412628,17.175887696,null,10.623340103,5.7803468208,6.936416185,19.267822736,6.0693641618,9.2292870906,11.560693642,11.560693642,8.0924855491,11.175337187,13.294797688,5.7803468208,14.183319571,13.87283237,15.414258189,6.1657032755,5.7453144158,5.4403264196,10.404624277,7.1142730102,6.936416185,86.705202312,10.623340103,7.5867052023,12.169151202,6.3279586249,6.8739259491,7.7071290944,15.49132948,10.276172126,4.5761078998,8.1127674678,10.142581888,11.560693642,8.4778420039,9.5869166784,23.121387283,15.622558975,7.225433526,7.8612716763,11.054913295,5.1380860629,5.7803468208,7.301490721,10.623340103,9.3930635838,8.6705202312,13.102119461,6.3583815029,7.3988439306,6.6473988439,17.341040462,20.290301863,18.74707077,9.2485549133,7.7071290944,7.0648683365,5.7803468208,15.622558975,5.8794384806,1.7341040462,7.0809248555,21.871582565,11.560693642,5.2023121387,6.8786127168,6.2490235901,7.5468208092,7.5144508671,13.294797688,7.0809248555,3.4682080925,11.560693642,12.138728324,8.6473988439,8.323699422,7.8112794876,23.815028902,4.9545829893,5.2179346977,5.3949903661,15.622558975,7.1566198734,9.0610842056,7.3988439306,6.2620423892,14.450867052,6.8538398018,11.560693642,5.3949903661,14.557910512,13.87283237,13.66263794,6.936416185,4.2358381503,11.857121684,8.2576383154,5.2338413032,11.333761507,12.169151202,16.184971098,16.515276631,5.4592164419,8.9916506101,6.3583815029,7.301490721,12.49804718,5.7803468208,18.394348105,5.5326176713,8.7486330261,4.293971924,11.248242462,9.2485549133,18.253726803,5.3949903661,12.716763006,15.524360033,15.622558975,9.3735353851,6.2490235901,10.738599872,7.7071290944,6.2490235901,6.6061106524,6.7437379576,7.225433526,13.87283237,5.9421965318,12.111202863,7.9099482811,15.980958858,7.2667217176,9.2485549133,6.4739884393,9.1268634013,16.872363693,12.04238921,15.83044316,5.2023121387,5.0578034682,10.019267823,13.87283237,8.0924855491,5.7803468208,18.74707077,4.8554913295,6.936416185,12.611665791,6.6061106524,6.0404624277,9.3860334323,10.63583815,5.7803468208,6.4739884393,9.2485549133,13.294797688,6.5028901734,21.626204239,8.2487111389,19.818331957,7.225433526,11.560693642,9.2485549133,17.866526537,10.728323699,7.7071290944,5.7803468208,15.622558975,11.098265896,6.6061106524,11.248242462,8.9332632685,15.622558975,6.8786127168,5.5810245166,9.2485549133,10.404624277,12.49804718,18.992568126,12.138728324,19.50867052,7.7071290944,3.3465165805,8.1237306671,11.560693642,9.9984377441,6.936416185,14.372754257,16.76300578,8.5634767716,5.2848885219,8.8928412628,6.5082423464,11.890999174,14.073887912,18.74707077,12.716763006,8.6705202312,8.459044128,7.9479768786,8.323699422,13.212221305,6.037251124,7.3988439306,9.668943773,5.7803468208,7.225433526,16.056518947,5.0578034682,7.3988439306,23.121387283,15.895953757,4.7630057803,6.4226075787,8.6705202312,8.4778420039,21.676300578,21.565948502,13.212221305,6.4855491329,6.7437379576,7.0905587669,15.49132948,7.7071290944,6.3583815029,8.4077771939,9.5183044316,7.3988439306,5.3692999358,6.7213335126,10.623340103,7.7175441337,10.509721492,8.6705202312,9.2485549133,9.8517215381,7.2667217176,11.890999174,9.2485549133,7.5144508671,20.231213873,19.996875488,11.560693642,11.230388109,11.560693642,6.2490235901,6.4739884393,13.747851898,10.78447564,6.4739884393,9.633911368,11.98886748,6.8490687219,13.635689936,22.496484924,8.7486330261,15.81315717,12.316585149,6.7712634187,7.301490721,6.2490235901,9.2485549133,4.6242774566,3.6333608588,5.7803468208,7.9728921666,13.386066322,9.2485549133,16.184971098,10.404624277,5.3544265287,46.242774566,19.653179191,72.25433526,10.789980732,5.549132948,8.1237306671,13.66263794,12.683044316,11.560693642,5.1380860629,8.6011560694,4.5761078998,12.49804718,9.8160798739,16.515276631,8.0924855491,6.0924855491,9.1268634013,14.997656616,5.7803468208,12.138728324,11.560693642,20.231213873,14.372754257,7.774566474,7.1566198734,9.633911368,18.497109827,10.276172126,20.231213873,6.1657032755,7.7071290944,7.8612716763,14.797687861,20.401224073,7.4988283081,18.74707077,4.6242774566,15.133998949,20.231213873,19.818331957,6.1436829067,10.569777044,9.6859865646,5.7803468208,10.276172126,10.276172126,20.909232932,6.936416185,5.6241212311,14.129736673,8.6705202312,7.1142730102,5.3949903661,9.3735353851,12.169151202,10.952236082,7.6862990158,11.560693642,7.7071290944,13.87283237,6.0465930986,10.789980732,6.3583815029,6.4739884393,8.2043632295,6.936416185,9.4962840628,6.0115606936,7.1676300578,11.946050096,6.7052023121,13.87283237,11.560693642,7.2667217176,9.633911368,8.7486330261,11.560693642,9.9091659785,21.965317919,10.364759817,12.111202863,13.87283237,9.8265895954,5.7803468208,7.9099482811,10.838150289,17.196531792,7.6069364162,5.1445086705,11.175337187,9.2485549133,16.872363693,9.633911368,6.8004080245,9.9598812686,9.2485549133,15.028901734,6.7052023121,86.705202312,8.4161849711,9.3735353851,9.9091659785,5.7803468208,6.4739884393,7.4988283081,6.2563753825,9.4172785502,12.777608762,6.936416185,7.0024772915,7.5144508671,17.656332107,6.1657032755,6.6061106524,7.7071290944,18.833877859,15.211439002,8.8631984586,11.560693642,6.3583815029,7.6057195011,10.569777044,12.611665791,14.821402105,11.2642656,6.0845756009,17.836498761,6.8670520231,12.716763006,8.4077771939,4.816955684,10.05277708,11.890999174,18.497109827,8.1237306671,14.037985136,11.560693642,8.8928412628,6.2249888839,10.404624277,15.854665566,7.7071290944,7.9099482811,9.9984377441,12.49804718,5.549132948,15.414258189,6.2490235901,12.49804718,6.1657032755,6.1657032755,21.836865768,18.497109827,5.9454995871,6.1657032755,12.716763006,9.633911368,5.7803468208,10.648007301,6.0693641618,9.1428571429,7.2369942197,15.414258189,8.8281660536,11.092016872,16.168455822,7.6630883567,10.246425312,9.1468208092,13.87283237,12.611665791,5.549132948,12.97053433,9.4587493431,11.560693642,10.324435102,16.441875401,9.1268634013,6.8004080245,13.761078998,6.936416185,7.4988283081,7.5144508671,14.705202312,10.73492981,6.8739259491,7.7071290944,6.4524801721,9.8265895954,10.019267823,8.4077771939,6.936416185,10.115606936,8.6705202312,7.9099482811,7.7071290944,5.4913294798,8.7486330261,11.230388109,6.8004080245,8.8928412628,5.9285608419,11.560693642,10.276172126,6.6930331609,9.9984377441,19.818331957,6.3583815029,9.3735353851,15.1940545,14.533443435,8.8081475365,13.87283237,5.7803468208,6.3005780347,9.2485549133,8.2999851786,12.111202863,12.49804718,11.51734104,7.5144508671,30.828516378,7.9273327828,17.065785852,8.1237306671,12.551610239,5.4797687861,19.010918433,12.331406551,7.5278935341,5.1380860629,11.921965318,7.5144508671,16.872363693,5.6647398844,8.1237306671,15.414258189,8.4778420039,18.122168411,8.9113680154,7.8612716763,10.276172126,9.1268634013,9.633911368,15.622558975,34.219653179,17.341040462,13.212221305,11.873144821,6.83131897,8.6705202312,5.549132948,11.660678019,9.1299836965,14.372754257,14.372754257,6.0845756009,14.129736673,6.0845756009,14.450867052,10.246978455,10.73492981,22.190109184,10.623340103,6.936416185,6.2249888839,13.487475915,7.6597006077,10.276172126,4.161849711,6.6061106524,9.5501382257,9.8347283237,12.169151202,4.8755968836,11.857121684,8.5879438481,5.1380860629,8.9332632685,11.058054788,13.386066322,4.6242774566,8.7486330261,5.7803468208,6.3583815029,7.5867052023,10.98265896,6.936416185,11.873144821,15.414258189,9.2485549133,16.515276631,6.6061106524,14.450867052,9.8265895954,14.643545279,6.9942196532,6.204238921,21.139554088,8.0462427746,5.2848885219,12.644508671,9.9091659785,8.8081475365,6.7262217551,12.491971741,18.253726803,8.7475915222,3.612716763,8.1237306671,13.294797688,13.747851898,6.8670520231,7.1933204881,8.2576383154,8.8081475365,11.560693642,11.248242462,16.698779705,14.450867052,6.7052023121,19.618146786,30.828516378,14.242774566,15.606936416,8.0264244426,8.2273603083,7.5144508671,5.7919075145,20.231213873,30.828516378,10.509721492,7.7071290944,9.3735353851,12.138728324,5.7803468208,17.497266052,13.87283237,12.845215157,5.549132948,6.3231967831,10.597302505,6.0556014313,6.83131897,12.111202863,10.623340103,23.121387283,13.068610204,9.3735353851,6.2490235901,9.2485549133,2.5323424167,7.7071290944,17.341040462,4.6242774566,8.6994219653,7.225433526,5.1380860629,15.568400771,10.671409515,5.7803468208,13.87283237,23.781998348,6.2490235901,4.6867676925,8.9916506101,2.3121387283,6.6473988439,6.5433526012,9.633911368,6.8004080245,5.7803468208,9.7623635196,12.49804718,6.936416185,5.7803468208,7.7071290944,5.7869529315,12.929723152,10.512524085,9.633911368,8.5634767716,6.3899106674,8.8928412628,12.04238921,5.0867052023,6.6930331609,9.2485549133,5.4843930636,8.0924855491,9.7572254335,8.7486330261,11.560693642,8.7982963188,7.5144508671,11.560693642,7.225433526,12.138728324,9.2485549133,14.997656616,12.023121387,null,10.789980732,10.623340103,13.87283237,5.7803468208,11.560693642,9.3110451492,10.404624277,11.560693642,13.487475915,5.7032755299,9.2485549133,11.873144821,6.6329479769,7.225433526,5.7803468208,9.0610842056,17.341040462,13.212221305,12.331406551,24.405908799,6.3583815029,11.010184421,5.367464905,5.7289659602,6.5510597303,9.2485549133,10.509721492,7.5970272502,7.4988283081,8.4778420039,5.4761180408,11.185752226,11.83044316,6.3583815029,13.87283237,15.622558975,7.3645900235,11.248242462,6.8004080245,5.7803468208,5.4761180408,11.873144821,7.3988439306,8.9916506101,6.6561569452,9.1268634013,10.019267823,47.293746716,28.901734104,5.7803468208,12.138728324,7.7071290944,8.0924855491,8.6705202312,9.3735353851,11.560693642,5.7803468208,4.6242774566,11.560693642,17.341040462,10.597302505,17.497266052,16.247461334,9.1268634013,6.2490235901,6.4226075787,15.117830147,13.747851898,9.3735353851,6.1657032755,75.144508671,3.5306983284,5.9285608419,9.2485549133,5.6518946692,17.367464905,21.577878456,8.6705202312,11.248242462,20.569777044,9.633911368,7.4988283081,10.789980732,6.8641618497,8.6705202312,21.296014603,7.9479768786,6.8739259491,13.762730526,19.29418923,20.231213873,6.936416185,11.560693642,10.276172126,12.845215157,10.63583815,12.49804718,18.253726803,13.386066322,5.7803468208,11.560693642,7.2667217176,6.2490235901,4.1288191577,7.7071290944,18.74707077,9.633911368,11.890999174,10.404624277,6.0693641618,21.676300578,10.404624277,8.2141770611,18.74707077,5.8794384806,12.283236994,20.809248555,9.2485549133,7.225433526,15.414258189,5.6321327998,11.890999174,8.6705202312,15.211439002,8.8928412628,5.2848885219,12.881915772,10.404624277,11.560693642,6.936416185,10.276172126,11.560693642,13.212221305,6.8114357132,7.1466106148,5.0867052023,13.122949539,11.560693642,9.2485549133,16.515276631,7.4988283081,11.817597945,12.49804718,12.661712084,7.1142730102,11.560693642,13.994523882,6.2941554271,12.138728324,9.9296984846,28.901734104,8.2209377007,12.49804718,8.8062327218,5.549132948,5.7032755299,5.9248554913,13.741602875,8.7486330261,5.7803468208,9.2485549133,23.121387283,2.4393063584,8.6473988439,6.1416184971,5.2327350167,9.5375722543,60.316662478,11.248242462,6.7602532342,10.693641618,8.323699422,4.6242774566,12.726396917,5.549132948,11.560693642,7.225433526,16.428354122,9.6184971098,13.969171484,6.6061106524,8.6705202312,14.780719114,7.1466106148,9.3735353851,8.7486330261,7.5144508671,14.643545279,1.8571098266,7.5144508671,115.60693642,38.535645472,7.225433526,14.997656616,9.2485549133,7.5860170658,8.0924855491,5.0096339114,6.1657032755,2.7250206441,5.6151940545,3.6584473549,7.0648683365,14.713610089,14.335260116,6.936416185,5.6358381503,15.414258189,6.4739884393,4.6242774566,15.414258189,6.4123314066,15.49132948,5.7803468208,5.2531791908,7.6909035595,9.2485549133,12.331406551,6.2427745665,5.2986512524,6.4226075787,8.0924855491,14.450867052,12.611665791,5.0867052023,5.7803468208,5.7803468208,10.115606936,19.052023121,2.3121387283,6.936416185,16.056518947,12.845215157,10.509721492,16.515276631,5.9248554913,6.3583815029,7.7071290944,11.560693642,11.560693642,8.2906688687,11.560693642,9.2485549133,9.5501382257,5.6151940545,10.918432884,5.7803468208,9.2485549133,6.3455362877,6.5549132948,11.248242462,15.028901734,9.9842354178,15.622558975,7.7071290944,14.129736673,10.404624277,8.4077771939,7.5144508671,15.07916562,6.936416185,4.816955684,8.1237306671,14.450867052,14.11654429,5.7803468208,7.1531791908,17.616295073,14.533443435,15.821635012,6.8786127168,6.936416185,11.817597945,6.936416185,11.230388109,10.404624277,14.450867052,9.2485549133,5.7803468208,23.121387283,19.818331957,4.450867052,9.2485549133,7.3988439306,9.4310921813,9.3490826841,9.2485549133,17.10982659,6.1657032755,8.6705202312,10.918432884,8.6463391137,18.786127168,12.845215157,6.4226075787,9.2485549133,38.535645472,9.7353209614,5.7803468208,11.560693642,12.138728324,10.276172126,7.0648683365,8.9332632685,9.633911368,8.2576383154,15.593493749,5.7803468208,14.797687861,18.497109827,15.414258189,9.2485549133,6.8336544637,24.338302403,8.6705202312,6.4226075787,9.8265895954,12.202954399,8.6705202312,15.622558975,10.98265896,24.405908799,11.560693642,10.918432884,5.549132948,7.5144508671,5.7803468208,8.9595375723,10.918432884,5.7803468208,10.404624277,10.404624277,10.276172126,6.3058328954,11.010184421,28.259473346,15.414258189,17.638315442,7.3988439306,13.294797688,10.404624277,9.633911368,8.0035571365,5.7803468208,18.497109827,14.643545279,11.560693642,6.3583815029,12.845215157,17.341040462,9.2485549133,17.341040462,7.7071290944,13.994523882,10.789980732,9.0229804032,11.560693642,21.579961464,20.231213873,9.2485549133,10.98265896,16.056518947,10.404624277,10.404624277,10.276172126,9.8265895954,10.404624277,13.87283237,11.560693642,18.497109827,13.294797688,7.7071290944,13.212221305,22.479126525,10.789980732,6.936416185,7.7071290944,38.535645472,17.341040462,18.497109827,11.560693642,9.2485549133,8.4778420039,9.2485549133,9.2485549133,10.078553431,8.3493898523,7.9479768786,12.56597135,12.845215157,9.633911368,5.7803468208,12.845215157,10.880652839,9.3127809891,9.2485549133,12.845215157,8.2141770611,9.8265895954,10.216426939,26.274303731,8.0924855491,15.606936416,7.7456647399,8.0924855491,9.2485549133,12.449977768,8.734746307,13.294797688,13.487475915,16.184971098,13.487475915,11.560693642,11.560693642,12.449977768,6.3583815029,12.845215157,8.4393063584,7.5144508671,14.643545279,10.404624277,11.560693642,9.098265896,10.98265896,9.083402147,5.4913294798,11.303789338,5.2023121387,13.87283237,6.7437379576,8.3493898523,6.3583815029,10.404624277,11.890999174,14.450867052,8.9768786127,8.734746307,9.2485549133,8.3493898523,15.055787068,9.1410135771,5.465055176,7.0648683365,14.129736673,7.5144508671,16.056518947,6.936416185,13.487475915,7.5144508671,10.918432884,9.8265895954,8.6705202312,9.2485549133,9.8265895954,8.6705202312,17.341040462,5.7803468208,7.3937058446,7.5144508671,7.8034682081,7.7071290944,11.560693642,10.019267823,8.6705202312,10.404624277,7.3988439306,7.5144508671,10.121387283,9.5375722543,10.019267823,15.414258189,8.6705202312,33.397559409,11.873144821,20.453534904,11.560693642,7.5144508671,49.132947977,17.341040462,11.560693642,30.828516378,7.5144508671,6.3058328954,28.901734104,10.918432884,9.2485549133,7.3988439306,7.5144508671,2.3763648041,16.184971098,17.497266052,6.936416185,9.8265895954,30.422878004,14.602981442,9.2485549133,5.7803468208,14.602981442,12.845215157,9.633911368,7.5144508671,10.404624277,9.633911368,9.2485549133,12.845215157,6.6061106524,11.560693642,9.2485549133,46.242774566,8.1888246628,6.7672353024,8.8947976879,10.115606936,9.8265895954,12.202954399,10.404624277,8.2576383154,16.184971098,7.3988439306,10.597302505,10.276172126,12.524084778,10.078553431,6.6473988439,9.2485549133,12.845215157,15.028901734,8.3879254978,7.7071290944,7.0751445087,13.87283237,8.5879438481,7.2667217176,9.8265895954,11.560693642,7.9823837049,17.341040462,6.4226075787,9.1268634013,12.331406551,13.487475915,5.1380860629,13.583815029,16.056518947,11.560693642,8.6705202312,23.746289642,15.414258189,7.225433526,15.414258189,11.560693642,46.242774566,8.6705202312,6.936416185,7.1566198734,8.0924855491,6.3583815029,5.2023121387,12.202954399,18.253726803,23.121387283,17.98330122,9.9091659785,13.87283237,9.8265895954,10.276172126,15.689512799,12.845215157,10.98265896,6.936416185,8.6705202312,12.845215157,5.0867052023,8.0924855491,16.955684008,10.404624277,11.323057161,7.0648683365,8.0422216637,12.777608762,7.9099482811,5.7803468208,13.294797688,10.838150289,8.3493898523,5.4761180408,7.0064809949,7.3988439306,8.1682080925,17.98330122,5.7803468208,10.276172126,14.771997431,19.968470836,8.6062941554,6.1657032755,13.762730526,10.404624277,7.0751445087,9.2485549133,12.661712084,11.560693642,16.377649326,25.433526012,24.08477842,16.698779705,5.5050922103,28.259473346,20.231213873,8.7486330261,11.560693642,6.936416185,9.3586567575,11.560693642,9.2485549133,10.918432884,11.560693642,8.4778420039,20.231213873,10.276172126,6.936416185,11.890999174,5.367464905,23.121387283,9.633911368,12.138728324,11.560693642,16.377649326,24.338302403,5.3949903661,9.2485549133,21.19460501,9.633911368,8.6705202312,5.7803468208,9.633911368,10.276172126,6.1657032755,13.747851898,20.346820809,11.078998073,14.129736673,29.543994862,9.2485549133,11.303789338,6.3583815029,11.560693642,9.2485549133,10.019267823,23.121387283,10.98265896,12.716763006,8.6705202312,7.5144508671,10.918432884,5.6518946692,8.6705202312,9.1522157996,13.212221305,16.428354122,13.87283237,20.231213873,13.87283237,5.1380860629,8.0924855491,12.202954399,6.0693641618,13.487475915,7.0648683365,17.341040462,19.421965318,6.3583815029,7.098265896,9.633911368,9.2485549133,9.2485549133,8.3815028902,24.338302403,11.560693642,14.450867052,11.190751445,15.125240848,7.9099482811,9.633911368,10.276172126,8.0924855491,8.0924855491,23.121387283,5.7803468208,11.560693642,11.560693642,8.3493898523,11.560693642,10.98265896,8.0924855491,13.87283237,7.5144508671,7.7071290944,10.276172126,8.6705202312,9.2485549133,12.202954399,10.918432884,11.890999174,12.815028902,17.126953543,7.5144508671,5.7803468208,14.129736673,7.7071290944,27.74566474,11.560693642,9.2485549133,10.404624277,8.6705202312,5.4592164419,7.8034682081,21.676300578,5.1380860629,13.386066322,16.441875401,11.560693642,10.276172126,11.560693642,5.7803468208,11.560693642,13.487475915,10.404624277,5.6151940545,13.102119461,13.487475915,23.121387283,11.890999174,14.450867052,6.7437379576,34.219653179,14.450867052,10.404624277,12.309096441,10.173410405,10.276172126,5.2023121387,8.0924855491,21.271676301,6.3583815029,16.184971098,14.797687861,7.5144508671,12.716763006,9.2485549133,9.633911368,7.5144508671,6.7437379576,35.324341683,7.5144508671,6.0556014313,8.2209377007,8.2209377007,5.1380860629,8.0282594733,7.5144508671,12.845215157,9.2485549133,23.121387283,3.5966602441,10.789980732,6.936416185,9.5674706,9.7353209614,18.111753372,10.98265896,8.3493898523,13.487475915,11.560693642,11.303789338,15.07916562,6.2620423892,11.560693642,8.0924855491,8.6705202312,7.7071290944,6.6795118818,7.7071290944,7.9099482811,14.450867052,12.138728324,7.3988439306,9.8265895954,12.04238921,10.693641618,15.722543353,11.560693642,5.2023121387,9.8265895954,24.405908799,8.0924855491,5.2023121387,6.0115606936,5.7803468208,6.1657032755,8.0924855491,8.6705202312,11.560693642,21.19460501,10.173410405,7.5144508671,12.845215157,24.971098266,19.421965318,5.7803468208,14.797687861,57.803468208,7.7071290944,13.212221305,7.7071290944,17.341040462,10.404624277,14.797687861,6.936416185,19.267822736,10.019267823,5.2023121387,9.1329479769,11.560693642,14.643545279,10.276172126,9.2485549133,12.169151202,10.822777026,18.304431599,13.635689936,16.184971098,5.7803468208,16.515276631,9.9984377441,9.4219653179,9.9984377441,23.121387283,9.633911368,8.2576383154,8.0924855491,4.6242774566,9.4489402697,11.560693642,23.121387283,15.867618724,9.2485549133,8.0924855491,12.360308285,9.633911368,10.789980732,9.1522157996,7.3568050447,9.2485549133,19.653179191,10.276172126,8.0924855491,null,5.2986512524,13.294797688,9.8265895954,8.6705202312,6.3583815029,22.479126525,27.74566474,7.225433526,11.560693642,8.0924855491,26.011560694,10.918432884,8.6705202312,12.260419836,8.0077071291,10.693641618,8.1888246628,32.113037893,7.3988439306,16.416184971,11.010184421,9.1522157996,12.169151202,8.0924855491,5.2986512524,6.5343051018,9.2485549133,13.487475915,14.450867052,5.7803468208,5.0263885398,11.560693642,7.5144508671,23.121387283,10.569777044,16.698779705,10.276172126,17.341040462,7.7071290944,13.87283237,8.0924855491,6.936416185,5.7803468208,9.2485549133,10.404624277,6.1657032755,6.4226075787,8.0924855491,21.19460501,12.169151202,11.560693642,8.6705202312,11.560693642,12.716763006,12.716763006,15.764582239,11.230388109,7.4502247913,11.560693642,25.690430315,9.2485549133,17.341040462,16.184971098,12.202954399,21.019442985,23.445086705,20.809248555,10.98265896,14.919379373,6.7052023121,13.359023764,6.6061106524,15.414258189,6.4739884393,10.98265896,23.714243367,6.2427745665,10.404624277,10.276172126,6.3583815029,14.450867052,9.7623635196,13.212221305,6.936416185,9.2485549133,9.633911368,11.560693642,11.560693642,13.487475915,8.2209377007,11.010184421,8.6705202312,6.1657032755,8.0924855491,4.816955684,8.6705202312,16.428354122,7.5144508671,10.019267823,7.3988439306,16.515276631,10.404624277,5.7803468208,8.0924855491,8.6705202312,6.7437379576,8.3699421965,8.6705202312,12.947976879,7.7071290944,5.7803468208,6.3583815029,16.698779705,7.1142730102,9.2485549133,4.3352601156,7.5144508671,15.838150289,10.404624277,6.4739884393,13.787989724,14.450867052,16.056518947,8.5879438481,6.1657032755,14.450867052,9.7623635196,11.303789338,6.2620423892,8.734746307,13.102119461,7.7071290944,8.6705202312,17.341040462,5.2023121387,20.552344252,18.497109827,10.404624277,10.404624277,5.7803468208,9.2485549133,9.633911368,10.671409515,2.408477842,12.845215157,10.019267823,7.8034682081,15.414258189,14.450867052,13.212221305,11.560693642,7.8612716763,20.809248555,8.2209377007,13.87283237,8.0924855491,5.2986512524,9.0173410405,5.2986512524,8.6705202312,20.809248555,9.8265895954,13.66263794,7.4318744839,15.414258189,14.129736673,16.76300578,9.2485549133,24.433391585,20.231213873,8.6705202312,16.698779705,12.086179716,10.404624277,3.0828516378,5.367464905,6.4226075787,22.479126525,9.8265895954,8.0924855491,14.797687861,14.900449583,6.3583815029,11.560693642,6.936416185,10.343778521,9.2485549133,21.387283237,9.8265895954,9.2485549133,13.102119461,9.2485549133,10.693641618,9.8265895954,9.2485549133,5.7803468208,16.056518947,10.98265896,15.928066795,13.487475915,16.698779705,9.8265895954,6.4739884393,5.7803468208,12.138728324,11.560693642,5.2023121387,15.1940545,8.6705202312,8.0924855491,11.637764933,7.7071290944,8.7861271676,8.0924855491,12.202954399,12.331406551,23.121387283,6.0115606936,17.98330122,11.560693642,14.450867052,12.594733462,12.524084778,11.010184421,26.011560694,8.6705202312,8.734746307,9.2485549133,15.414258189,11.560693642,6.936416185,15.028901734,9.7353209614,11.560693642,9.633911368,24.405908799,5.7803468208,19.818331957,15.928066795,13.102119461,15.606936416,12.947976879,8.0924855491,5.5050922103,9.8265895954,11.560693642,12.551610239,10.98265896,12.845215157,25.289017341,11.560693642,8.5879438481,7.5144508671,8.5549132948,10.918432884,20.346820809,8.323699422,11.560693642,7.5144508671,9.8265895954,13.487475915,2.2947976879,9.9091659785,13.87283237,10.404624277,5.7803468208,15.414258189,14.129736673,10.404624277,15.414258189,19.357440516,10.98265896,7.9099482811,null,17.341040462,19.470641923,13.294797688,11.560693642,9.8265895954,9.2485549133,9.1791907514,20.231213873,46.242774566,9.2485549133,11.560693642,23.121387283,8.0924855491,9.8265895954,9.2485549133,9.633911368,11.560693642,8.459044128,18.094998743,8.0924855491,10.98265896,11.560693642,17.341040462,13.994523882,8.0255552175,5.1380860629,11.560693642,6.7052023121,11.248242462,7.7071290944,9.2485549133,11.416184971,25.690430315,8.0924855491,5.774566474,8.0924855491,34.682080925,8.323699422,8.6705202312,22.543352601,26.424442609,9.633911368,8.0924855491,15.414258189,5.7803468208,15.211439002,7.7071290944,11.560693642,12.283236994,11.560693642,7.9640333976,26.589595376,14.298752662,17.645269242,8.9916506101,30.828516378,14.450867052,24.772914946,10.918432884,5.3949903661,9.2485549133,30.828516378,19.267822736,18.625561978,8.6936416185,18.304431599,23.121387283,5.774566474,7.225433526,13.386066322,9.8265895954,10.404624277,11.560693642,14.602981442,8.6705202312,5.3949903661,11.303789338,12.777608762,9.2485549133,6.0693641618,9.8265895954,11.560693642,12.202954399,9.9091659785,8.0346820809,7.7071290944,25.433526012,5.549132948,17.341040462,9.5568400771,20.346820809,7.5144508671,9.633911368,15.414258189,49.545829893,8.2576383154,17.572254335,8.2485549133,7.225433526,6.0693641618,7.7071290944,8.0924855491,26.97495183,8.2209377007,6.6795118818,10.789980732,10.276172126,17.785682526,8.0924855491,17.572254335,14.129736673,9.8265895954,10.98265896,22.928709056,9.2485549133,5.0096339114,9.4198244487,23.121387283,51.380860629,17.341040462,11.857121684,16.698779705,8.6033068961,15.414258189,10.918432884,9.8265895954,10.404624277,9.2485549133,21.19460501,16.184971098,8.0924855491,10.404624277,11.560693642,8.6705202312,16.056518947,9.2485549133,6.936416185,7.8034682081,8.5634767716,9.8265895954,6.1657032755,16.515276631,21.019442985,10.786127168,7.7071290944,6.936416185,10.404624277,21.19460501,8.0924855491,8.734746307,12.588310854,8.0924855491,13.87283237,42.389210019,16.056518947,14.771997431,18.497109827,9.485697347,8.6705202312,6.7437379576,17.98330122,7.5144508671,16.114906288,8.9916506101,17.98330122,9.7623635196,14.543352601,13.294797688,9.2485549133,15.414258189,23.121387283,17.98330122,14.450867052,8.323699422,7.5761078998,10.789980732,13.87283237,8.612716763,32.113037893,8.0924855491,11.560693642,18.253726803,6.4226075787,16.955684008,9.633911368,25.048169557,10.276172126,14.662343155,11.560693642,15.414258189,7.7071290944,13.87283237,5.7803468208,5.549132948,9.633911368,6.1657032755,5.2023121387,6.4183429672,13.487475915,9.1714836224,16.184971098,24.338302403,8.9916506101,8.3493898523,9.2485549133,10.671409515,16.184971098,15.606936416,11.560693642,9.8265895954,6.4226075787,8.0924855491,19.267822736,7.7071290944,13.294797688,11.560693642,10.98265896,12.661712084,9.2485549133,8.1502890173,7.7071290944,4.0462427746,5.549132948,23.121387283,12.845215157,8.0924855491,5.4592164419,12.845215157,13.87283237,14.386640976,11.560693642,10.276172126,12.202954399,11.560693642,8.5218827415,26.424442609,6.1657032755,11.560693642,6.3583815029,11.2642656,12.845215157,8.0924855491,9.4161849711,15.028901734,11.560693642,12.524084778,13.701562835,14.450867052,7.5144508671,8.4971098266,14.98608435,20.038535645,9.2485549133,9.8265895954,11.098265896,9.485697347,10.769171484,7.8612716763,9.9091659785,9.9091659785,8.6705202312,6.5510597303,11.560693642,12.845215157,14.129736673,7.3217726397,7.0648683365,9.2485549133,14.450867052,5.9555088457,14.997656616,16.955684008,15.414258189,11.560693642,12.138728324,12.023121387,16.184971098,9.6184971098,8.6705202312,6.6795118818,8.5879438481,9.5375722543,5.7341040462,16.056518947,16.184971098,10.276172126,10.404624277,7.1142730102,7.7071290944,13.212221305,9.8265895954,6.936416185,10.789980732,9.7353209614,4.3930635838,10.98265896,8.0924855491,20.552344252,5.7803468208,19.010918433,11.560693642,7.5144508671,12.202954399,7.8034682081,8.0924855491,10.276172126,5.2548607462,20.231213873,5.5876685934,15.606936416,20.809248555,7.5144508671,5.7803468208,6.5510597303,5.1380860629,16.184971098,7.7071290944,12.169151202,5.0263885398,9.5691014188,19.267822736,18.497109827,20.621777847,8.0282594733,20.346820809,9.633911368,13.87283237,10.647398844,9.5375722543,5.0867052023,5.0096339114,13.487475915,22.441346481,12.716763006,10.276172126,10.918432884,9.1965317919,9.9091659785,9.2485549133,8.0924855491,6.936416185,8.2576383154,7.225433526,7.5144508671,7.5144508671,1.5722543353,16.647398844,20.552344252,10.98265896,9.633911368,11.560693642,17.341040462,5.7803468208,9.633911368,8.6705202312,14.566473988,5.5050922103,13.728323699,7.5144508671,9.9091659785,12.202954399,16.76300578,13.294797688,10.404624277,5.0446663163,14.450867052,13.87283237,17.001020061,18.497109827,23.121387283,9.633911368,7.5278935341,12.845215157,23.121387283,12.658959538,6.4226075787,8.6705202312,8.9916506101,9.2485549133,26.011560694,14.129736673,9.2485549133,25.690430315,3.1529164477,15.211439002,8.6705202312,9.2485549133,8.0924855491,6.936416185,11.560693642,11.560693642,9.2485549133,9.2485549133,7.3988439306,18.332826285,15.606936416,10.404624277,13.87283237,12.716763006,16.33911368,8.0924855491,11.560693642,25.690430315,14.93256262,11.560693642,6.936416185,11.817597945,11.560693642,14.450867052,10.98265896,17.98330122,10.276172126,15.606936416,7.3988439306,8.6705202312,5.7803468208,9.0173410405,5.7803468208,11.560693642,15.96476741,14.797687861,9.8265895954,12.97053433,9.1268634013,8.0924855491,14.643545279,7.5144508671,20.231213873,21.296014603,9.2485549133,7.5395828098,10.404624277,16.377649326,8.0924855491,7.5144508671,11.271676301,9.8265895954,8.2576383154,14.450867052,7.7071290944,8.6705202312,15.606936416,9.2485549133,16.515276631,11.560693642,7.4318744839,5.2023121387,8.6705202312,15.028901734,22.543352601,11.560693642,16.955684008,11.857121684,11.560693642,17.341040462,4.3352601156,6.6930331609,12.845215157,10.404624277,8.0924855491,16.056518947,5.7803468208,10.276172126,13.102119461,5.549132948,10.276172126,7.7071290944,6.936416185,15.028901734,6.8872217439,26.011560694,8.6705202312,11.560693642,12.845215157,11.560693642,8.6705202312,13.87283237,14.450867052,23.121387283,7.8612716763,7.8034682081,7.225433526,10.404624277,14.450867052,5.6051847959,8.0924855491,9.5788604459,12.845215157,25.690430315,2.8901734104,18.497109827,14.450867052,10.98265896,14.771997431,16.056518947,8.9916506101,9.8265895954,6.6930331609,10.404624277,11.560693642,13.87283237,8.0924855491,9.2485549133,18.497109827,7.225433526,10.404624277,11.560693642,7.5144508671,8.6705202312,10.918432884,15.895953757,13.487475915,14.129736673,10.404624277,9.2485549133,16.184971098,16.184971098,5.9147734911,11.857121684,8.5549132948,23.121387283,10.019267823,8.6705202312,10.404624277,19.818331957,8.9916506101,15.028901734,9.8908156712,5.1380860629,3.1791907514,13.87283237,8.0924855491,6.936416185,5.7803468208,13.87283237,16.056518947,7.5144508671,8.0924855491,24.405908799,19.267822736,8.0924855491,8.6705202312,6.0115606936,9.2485549133,6.6795118818,7.225433526,12.845215157,9.8265895954,8.6705202312,7.5144508671,10.918432884,17.001020061,8.734746307,9.2393063584,12.111202863,10.623340103,12.777608762,15.028901734,11.560693642,16.76300578,6.7437379576,6.4739884393,6.936416185,23.121387283,10.276172126,13.87283237,14.863748968,12.202954399,7.5144508671,24.277456647,12.716763006,8.0924855491,16.896398399,8.7861271676,8.6705202312,10.841361593,15.414258189,17.341040462,5.235031083,11.835948252,11.560693642,34.682080925,20.231213873,11.560693642,10.276172126,10.98265896,9.4971098266,14.693641618,23.121387283,16.184971098,17.341040462,5.7803468208,7.7071290944,12.947976879,6.3583815029,18.304431599,9.1268634013,10.404624277,10.276172126,8.9916506101,5.7803468208,5.2848885219,11.560693642,17.341040462,8.0924855491,15.414258189,6.0784910253,9.2485549133,12.716763006,11.239563263,11.560693642,13.87283237,14.129736673,16.698779705,17.822736031,10.98265896,10.404624277,7.5144508671,7.7071290944,23.121387283,7.225433526,18.304431599,9.2485549133,10.404624277,10.115606936,6.0248999555,10.276172126,9.2485549133,12.861271676,10.789980732,11.560693642,11.560693642,10.841361593,5.2023121387,16.056518947,12.138728324,9.2485549133,16.184971098,11.560693642,6.936416185,23.935260116,10.98265896,9.2485549133,11.2642656,15.819896562,8.7919075145,11.560693642,8.6705202312,8.3493898523,9.2485549133,5.7803468208,10.404624277,11.560693642,9.2485549133,26.97495183,11.303789338,9.633911368,5.7803468208,13.73270275,8.9595375723,13.102119461,7.5144508671,5.1380860629,6.936416185,8.0924855491,19.010918433,20.552344252,5.2023121387,22.116109575,8.2157996146,7.9273327828,7.4804488269,6.6061106524,8.5184058412,16.184971098,13.487475915,9.8265895954,9.2485549133,13.487475915,12.947976879,7.1290944123,9.2485549133,13.762730526,15.606936416,9.2485549133,10.404624277,8.323699422,12.845215157,15.606936416,6.936416185,9.1329479769,6.936416185,8.3815028902,13.005780347,8.3493898523,5.0096339114,7.225433526,15.028901734,9.289017341,8.4778420039,3.3718689788,11.010184421,7.5144508671,7.7071290944,5.549132948,12.845215157,9.2485549133,24.338302403,7.7071290944,14.771997431,8.3493898523,9.2485549133,14.450867052,7.5144508671,5.0867052023,6.936416185,9.2485549133,13.294797688,5.2986512524,11.560693642,9.2485549133,6.3783137333,10.276172126,11.560693642,14.450867052,10.918432884,11.560693642,12.845215157,7.9273327828,8.1888246628,13.87283237,8.6705202312,8.3493898523,23.121387283,49.132947977,8.9916506101,2.8901734104,7.0648683365,17.341040462,7.7071290944,10.918432884,26.589595376,9.5375722543,11.560693642,8.6705202312,14.129736673,6.936416185,14.450867052,7.5144508671],"Wage_month":[1000,1600,2385,730,1100,890,2500,800,866,900,1500,2500,1200,3000,1400,880,1300,850,2500,3500,1175,1400,900,800,900,1000,1600,1700,1000,2800,950,939,2700,1000,1000,600,1100,1800,1700,2100,1498,1100,800,1000,340,1200,900,3064,1600,3600,1000,800,3000,1000,1500,900,1600,850,3500,2500,850,700,1600,1060,700,1188,1400,2200,900,450,1400,1700,2600,1400,900,1000,1213,1300,1500,2000,817,1200,850,1000,974,1400,1900,3500,1200,110,1200,700,1500,2400,2500,1300,570,800,1800,2000,2000,1000,1200,1800,1000,920,1100,1200,1200,2685,900,1400,300,1400,1080,2000,800,1200,1200,2100,2000,2500,1500,1200,1470,1100,2500,1500,1300,1500,500,900,470,1600,1500,1100,550,1100,1500,900,2672,1692,700,2000,1500,835,1800,1400,450,2200,1500,1500,1200,850,700,1400,1200,600,700,1300,1200,2700,1000,2100,600,2100,950,1800,400,1400,1300,1500,2800,1494,1100,1000,1600,1000,1200,1800,1700,1000,950,2200,2500,1000,1800,1900,2500,400,1500,1500,1300,1050,1000,1937,1500,1200,1700,1500,500,2100,1300,1040,246,900,900,1000,740,1900,1600,2500,1800,1600,1522,1100,750,1100,1100,1200,700,800,1500,400,1450,570,1000,1100,3200,2000,1400,1800,1350,950,1500,2400,1800,1600,1100,400,2300,1550,2600,2030,1200,1300,950,800,1000,580,1300,1000,1450,1500,3500,1000,2600,700,3000,2000,1200,650,800,3000,1000,1200,680,1100,2600,720,1200,1100,1000,1300,1500,700,1200,1500,150,2000,880,800,998,700,1700,1800,1000,650,200,1300,3000,1415,1300,650,1600,1000,1200,2600,1400,481,2300,3000,1100,1339,1700,400,1500,1700,2300,1500,500,300,1700,499,1450,900,600,1400,1600,1400,1420,2500,1400,1300,1000,2300,1100,900,935,1200,1800,1700,1200,880,1000,2300,1300,1200,1600,1000,1900,1000,1400,2100,500,1700,1300,1300,2400,3000,1500,1500,3000,564,1600,1960,3000,1100,600,1000,1100,1200,700,1500,1100,600,2600,1300,2000,1600,1000,700,1100,608,2300,610,1300,1100,200,1180,700,1800,830,1350,550,1400,2400,1500,3000,950,1000,1017,1820,1000,900,960,700,1200,355,1620,1000,2000,1900,1700,2200,2100,1400,2300,580,1635,2000,800,1500,1600,2200,1700,2400,1200,1800,1500,1200,2400,2200,3230,2000,1200,3000,300,2000,800,1700,1200,1000,1900,1200,1700,1500,3000,2600,1500,2200,736,1100,800,2400,1200,900,1500,900,1700,950,3500,800,3000,800,990,1000,1700,1214,1200,2200,1800,1600,1800,1800,2000,2400,600,900,1090,506,2500,1600,1200,1400,800,3000,1000,900,908,1300,1550,1500,2700,1000,1500,1500,3500,1200,750,116,800,2435,1400,3700,2500,1400,2900,1600,1200,1300,550,2100,1000,1300,1400,1000,400,1700,700,1000,2400,1550,1400,1400,600,1000,2400,2400,2400,400,2200,1800,300,1640,1200,950,1137,1500,1800,1400,1000,2700,700,400,2000,1700,1400,1200,1500,2000,2000,2000,3000,760,1600,2900,1200,1700,1300,1200,2500,2500,1400,350,2300,1300,2500,1700,540,1200,1543,1300,3000,750,1290,1850,2000,2000,1100,1800,1200,1250,1300,700,1000,595,2000,750,1300,1400,1400,1200,600,1700,2500,1000,1300,2000,1800,3000,1000,1100,2200,900,1000,1100,840,1098,3000,1250,1800,550,1300,1411,517,1000,2200,730,1180,3000,700,1600,2400,900,1500,400,2400,1241,1300,1400,2100,2100,1000,1368,900,2100,2800,1300,500,660,1200,1500,1200,910,470,800,1700,250,1600,1400,1000,900,2100,924,1400,2400,2700,750,1200,230,1100,1600,2000,2100,1300,500,1500,1100,1250,930,1500,500,1600,660,1200,950,1800,500,900,850,2000,700,1845,1700,550,3500,1740,600,1950,330,400,1000,1950,1100,1850,300,900,2200,1000,1500,1300,1300,1000,1400,1853,820,2100,850,730,265,1500,2200,1800,2000,1500,1300,1650,2000,1300,2200,3000,800,1166,800,1500,650,1400,1200,2000,1500,1800,1500,700,1800,1250,3800,800,300,1200,1200,1050,1800,300,2000,2300,1325,800,1500,850,1200,1100,1600,200,1200,216,500,2300,1094,1500,2500,2900,1500,625,1500,3800,1100,1000,740,2600,2000,1500,850,2500,815,800,2200,1400,1500,1600,200,1300,550,1800,1200,1750,800,700,1300,1300,1900,2514,1000,2300,1500,3500,1400,1500,1300,1300,950,1300,1200,2600,1600,1850,1200,2000,850,1200,2200,950,1550,300,1100,950,1000,1325,1400,1400,1404,1200,1200,2100,600,1700,1400,1700,1000,1000,800,1300,1900,500,1062,1200,500,1400,1300,1400,1300,1200,1750,600,900,2500,600,1400,765,3000,1000,1700,2700,1000,1080,600,1050,1400,650,1300,1000,800,1100,1600,1400,1600,800,1200,3500,1300,1600,750,830,2000,2000,1000,600,1500,3000,2000,1400,990,1300,1000,920,2000,800,2500,1000,1200,1300,1000,1200,1200,1714,1650,1200,1800,1100,720,690,600,800,2300,1400,1400,2550,2100,2360,1300,550,1400,2300,1500,1200,1800,1300,1800,1500,700,1300,1250,1000,1600,800,300,1500,600,980,900,2200,900,2300,600,1600,1300,408,1500,2677,1100,3400,900,1200,800,1300,400,1100,700,1400,2500,1400,1000,1700,2700,2800,1500,1642,1000,2500,2100,1300,1400,1400,900,1900,2400,3000,1500,1300,500,2000,1500,2800,1400,745,3000,1200,1800,930,900,1100,700,1300,1900,1200,1900,850,1000,2000,1650,700,630,1250,2600,2000,1300,2000,2100,1500,1700,1200,550,1800,1100,2100,1200,2500,1500,3000,3000,1800,1250,1800,1026,900,1400,1300,300,900,1200,700,1600,800,1807,2500,3000,460,1500,700,1300,420,2200,630,1500,1850,2700,1400,380,3212,1400,250,2300,2400,1600,940,120,1200,3500,900,3100,2000,2000,1800,860,1000,1000,2000,940,1200,1000,2300,2400,2500,2500,1800,450,1300,410,1200,2550,2300,2300,1100,1100,1431,1900,1300,750,1200,1200,869,1000,1500,2000,1300,900,1200,1200,300,1200,410,800,300,450,1400,450,2000,1200,1500,257,1500,3000,1900,2600,1800,250,1100,200,2350,1100,1200,1766,1000,900,700,1300,1200,1200,1200,900,2000,1600,1050,970,1500,1000,1800,1500,1100,1100,580,1500,1000,1200,3000,500,1300,1200,1000,3369,1700,1200,620,2000,1000,1000,586,2400,1700,1200,1000,3300,1800,2300,900,2100,900,2800,2200,1230,3100,1200,1200,1300,3000,420,1200,700,1800,1400,2000,950,2200,880,990,1700,492,850,2000,250,2600,1150,780,2500,2600,2300,3000,800,1000,650,1000,3000,2600,900,1400,2200,2100,800,402,800,1040,950,700,700,1300,900,1200,870,400,1500,1200,1100,2500,1200,1200,120,300,1300,1200,500,1300,1100,2500,1020,500,1000,780,800,1000,1200,800,930,2600,1400,1700,1000,1500,1300,2500,1700,1050,2600,300,900,2700,1200,2700,2000,1500,1100,1250,1400,1300,1300,1250,1450,3500,2000,1130,1300,600,1000,1250,800,2200,1400,3000,2500,2000,670,500,1200,1100,2000,2000,2500,2700,1500,1000,1200,1000,1100,1500,1300,1200,405,1700,1500,840,1800,800,700,3400,1200,1900,700,1100,2100,1200,945,600,1100,1600,2300,500,1200,2400,850,1500,1900,2400,1900,1400,1000,1000,2000,900,1300,1600,2900,1100,1600,1900,700,1400,1650,700,890,1200,1000,1000,1000,2600,1000,1200,550,1900,1800,1400,1300,1800,3000,2000,400,2400,600,1350,1300,3000,966,1750,1200,1100,2000,2100,650,345,3000,1300,1200,1600,600,1400,1200,480,1100,1800,3000,1200,2200,850,950,2000,3600,3000,1300,700,1300,1700,1300,700,2500,3500,1300,1700,2500,1000,700,800,1900,1200,1200,1200,1500,850,2200,580,650,1269,1200,1500,1800,800,2500,1000,1500,895,2500,1500,2200,1800,1600,1300,700,1900,2500,1200,3200,2500,890,1100,1700,1500,2500,1300,1400,1700,520,1300,750,2200,2100,1000,3000,1350,2000,540,2700,1900,1400,1500,2400,1200,650,1500,2200,3000,800,800,700,300,1671,2200,2000,1000,1500,1150,500,900,1000,2200,1200,3200,1000,800,2500,1200,600,2800,1400,1450,1500,2000,2200,800,1200,1500,1100,550,1150,1000,1300,1200,875,1000,450,800,1800,2200,1200,1700,1108,2300,2000,2600,1150,1300,800,800,1800,1000,2500,800,2000,1200,1500,800,1100,900,1200,850,600,2500,2900,2500,500,1400,1500,800,400,1800,1700,1500,1200,2400,1500,2000,1500,3300,2300,1250,800,500,250,3000,1300,900,3000,900,1000,2200,850,1574,2100,600,2200,2600,815,1021,1400,1100,300,2600,1300,650,3200,1200,1500,550,1500,900,850,1250,850,1200,2700,2000,1000,1000,1400,2050,1227,210,1083,716,2700,700,600,280,1000,1200,800,1700,1100,625,690,1100,855,1350,600,600,1100,2500,1890,1300,1600,900,2500,2400,1700,3500,800,1800,900,1700,2500,3800,2200,1200,2700,550,600,2500,1500,1096,1400,1300,2000,2500,1400,1500,1500,900,1300,650,500,900,3000,1300,1200,2000,750,900,1000,770,900,2300,954,1600,1300,1100,1600,1500,2200,750,1300,1500,943,1600,887,1100,1345,1500,1400,1600,3000,500,1200,1500,733,400,1100,3500,800,1000,1242,1900,1400,2000,2300,1800,1600,1200,2250,1500,2500,1200,2000,2600,600,390,350,1150,1300,1600,750,586,2100,1300,1700,1300,972,600,1200,1800,3100,1000,3100,2500,1200,1300,550,900,900,900,1500,3450,1800,1300,1200,600,1800,1450,2000,2000,2100,2150,460,2000,2100,3000,2700,800,3500,1300,900,1300,2000,750,1350,2500,1400,600,900,1400,2400,1900,700,1250,2500,1300,500,790,1300,1000,3200,2800,300,2000,1100,1300,1000,1240,1100,2322,800,1100,1000,500,950,3000,1100,1200,3000,900,1000,1500,1400,1500,1340,2000,1000,3400,1200,1100,1700,2800,1200,1500,2500,1000,1164,1300,800,1050,1200,2600,2200,1500,1051,2500,885,700,1600,1400,1400,600,1100,1200,2500,1200,800,1000,2750,1700,1450,2700,1300,2500,1100,2000,850,1600,800,1200,1000,900,450,1200,400,1200,1300,840,1300,645,1000,1400,590,523,1000,1000,1400,2400,1600,1400,1200,2500,1090,1500,2000,900,1600,2700,1200,147,1000,2000,1100,600,680,1000,2900,2100,1200,1000,1000,1500,1800,400,2000,2400,600,1700,2600,2500,1000,850,1800,1000,1600,600,2330,1800,900,600,1200,1483,1700,1500,1250,738,1500,1300,1300,2000,1400,900,2400,1400,1000,800,1100,3400,240,1570,500,1000,1500,1320,2300,3200,1500,1800,1300,1100,1100,1079,1200,2000,600,1400,2200,2200,400,1400,1500,1500,2800,1200,1200,400,1200,1800,1150,1200,1500,1500,2000,1500,2500,2000,1900,740,2300,3500,500,1300,1400,1500,1300,850,1300,3500,2000,1100,1900,1900,1300,3000,1200,1500,1500,1200,1000,800,2000,700,1500,1200,2000,1050,1000,3000,1400,450,500,1400,3200,1000,1000,1800,1300,700,800,750,1300,900,300,1400,1100,1500,2400,2100,2600,2700,430,1300,550,2500,2650,2000,1400,1350,2340,700,2000,2700,1000,1300,1600,3100,1600,3800,2450,1500,2600,1425,1900,1600,1900,1600,2000,1300,1500,1649,1430,2500,1200,2400,2200,1500,800,2500,2200,1680,1239,1800,1380,1450,1780,1560,1435,4201,3083,1700,1568,1700,3220,2200,900,2500,2964,2450,2700,784,2900,300,2200,1900,3480,2600,3500,2000,1820,2232,2800,1605,1533,3000,1100,1611,1000,1815,1500,1600,2500,1600,1700,1800,1600,527,2800,2000,1500,2000,1975.7,1792,1400,1400,1430,1500,920,850,4000,3500,2200,123,2100,2200,1300,1600,2000,1600,800,3630,320,2600,2500,1400,1450,2200,2100,1620,3700,1400,1800,4000,1432,1700,3200,2378,2250,2400,1762,2000,1800,3600,1800,850,2800,1000,3000,1400,1400,3000,1544,3900,3200,1450,2400,2494,3750,2400,1747,1560,1300,3000,1500,1500,4000,1800,1917,1500,650,2600,1500,1700,1800,1020,4200,938,1900,2500,2000,1700,2800,2272,2560,1950,1600,1300,2900,2200,1412,2300,2600,1400,2340,1900,700,3000,2800,870,2050,1500,2200,1900,2610,3000,1500,2500,900,1700,1408,1176,3000,1273,2202,1500,1800,2600,1500,1600,1700,900,1679,1428,2900,1700,3200,3600,2100,1600,2000,980,1950,2047,3000,2000,1400,1900,1500,2210,1400,1900,500,900,1780,2800,1900,710,1900,2000,1400,2500,2404,762,2500,2860,2000,2100,800,2280,1700,650,2100,2500,3000,1200,1490,2400,2833,2600,2000,1800,200,2282,2538,1900,1171,1250,1700,1500,2800,2500,1500,2500,980,2600,1500,1998,680,4300,1500,2300,2600,3800,950,2600,1600,2000,1800,2500,2100,2000,4200,3600,1500,3100,956,1800,1600,5600,1500,1700,2291,2000,2000,1863,2000,1600,2200,1550,3770,1375,2100,1167,250,2210,1650,1700,700,2750,1100,2098,1700,3960,260,1480,850,2400,1200,3050,1600,3900,1800,120,2100,2300,1600,2950,623,1569,2500,2400,3000,3000,1600,2100,1500,2500,3160,585,1800,1700,1880,2200,4200,1600,5000,1565,669,2100,1368,2600,3000,1800,2000,1400,1453,1500,1600,1800,1500,1800,2000,1600,1500,1500,2200,1200,1800,1980,1300,4400,1800,1100,1480,1800,3400,1900,4100,2000,900,1350,1450,1633,1500,2000,4000,1676,2600,1860,2625,910,3300,1426,1850,1885,1500,1600,1700,309,1800,2000,3300,2200,1300,2647,3700,1430,1476,1762,1847,1100,2080,3500,4465,1300,737.35,5200,2695,1400,1400,1500,3300,3500,1700,1500,1400,1400,2300,2100,2000,488,2700,2800,1900,1650,2600,1300,1350,1647,1382,2100,4000,1662,2851,2300,1800,1400,2300,1600,1800,2300,2550,3800,3000,1544,3116,2000,3100,2860,2800,1440,2100,2140,1600,2600,1800,1653,1500,3900,2800,1100,1600,2854,1643,2034,2880,2800,1800,1900,1463,2100,2500,2900,1453,1600,3000,1600,2500,3600,1311,200,1450,2200,2670,2100,870,1100,1800,1600,1700,1300,800,2000,2608,2000,1800,2600,1700,1372,2000,1600,1800,1550,2500,2370,1400,694,1400,2400,2296.63,800,2400,3000,1550,838,1600,825,988,1500,1900,2400,1500,1200,1500,1926.2,2600,800,5829,2420,1965,2000,1000,2637,1300,2800,1400,2500,1800,1100,2750,3500,1800,2200,950,1300,2600,1800,1425,1400,985,2697,1595,2400,3800,1500,1708,1200,2000,1500,4000,1800,1100,3700,1500,1821.7,1600,2800,2400,2500,1600,2600,1800,1800,1300,2000,3200,900,2280,1222,1600,3200,1700,2800,2250,840,1400,3000,1700,1700,1500,1500,1500,900,2100,1900,2300,1853,2933,4200,2600,3800,3743.74,3167,2200,2000,3400,2000,1300,5300,1300,1630,500,2500,1800,264,1755,2600,800,828,2258,1800,1300,2000,1100,3218,1800,3000,2200,2100,1700,1820,2700,1350,1193,3000,3900,1924,1400,1745.89,457,2178,1700,1200,1800,3000,1500,1200,1625,3455,1400,3000,1425,3280,1600,3200,1560,1700,1400,1429.82,1950,741,532,1776,3000,3500,1500,3600,1170,2842,1700,1356,1550,2900,2000,1470,2340,1700,1900,1395,2500,1305,800,1900,2600,1590,1300,3600,1260,1700,3300,1600,5000,1400,2275,1565,1300,3200,4600,1800,2700,1700,1821.43,1200,1600,1600,970,2700,2600,2500,1750,2925,2000,700,1700,2000,2600,1590,1600,5000,639,1900,1550,1400,2300,2000,2100,700,750,4000,3000,2150,1450,3600,1730,1677,1881,300,3200,1400,2461,780,1517,1700,3600,4900,1500,1700,4000,3200,2500,5200,1800,4500,1750,2080,2500,1470,1600,3100,2000,2300,2000,2600,2727,2250,3700,1500,1500,1900,2150,2000,1450,1425,1900,3100,1900,2100,2600,2452,1300,1000,1110,1800,1800,5000,3400,1909.52,4500,900,400,3000,2300,1467,2000,900,2600,1675,2340,2609,1117,2500,1500,1800,1800,1500,1900,2400,1500,2100,1040,2400,1400,1900,2500,3000,1110,1081,1800,1375,2080,1477,5000,3200,3400,300,2000,3800,2450,1613,2500,684,1300,900,1400,1900,1700,2200,850,1550,1400,5000,2200,1400,2800,1690,3000,3900,2500,2000,340,2800,1800,2000,1700,2500,689,2039,124,1800,1462,1000,3100,799,1400,1127,2000,1399,325,550,1900,2800,2500,1120,2000,1440,1131,1462,1690,2800,1420,1600,4700,1500,500,1500,2800,380,1728,1760,1000,5700,2000,1600,2000,1450,1500,1800,2800,1600,1690,1450,1800,1803,1700,1500,2400,2096,2300,2000,1400,450,2210,1900,1755,1500,1847,1590,2590,1284,1298,1650,947,3000,1350,1300,2000,1430,2000,1918,1500,900,1600,1700,3900,2500,1700,1400,1500,2300,1000,1484,3120,1200,3278,2000,2000,2500,1425,1442,2700,4500,893,2200,940,624,1200,1555,1050,1400,3000,2300,2600,3000,1600,3800,1800,1415,1545,400,2879,3500,2000,2000,1027,1400,1600,1400,1800,1280,1820,1700,1000,2300,2200,2500,1650,2173,1500,1428,2200,1500,1900,2211,1900,2800,1500,1950,1950,1491,2170,1700,2300,1500,1700,2000,1500,1700,1490,2800,1598,2500,1750,1775,4680,3500,5416,1388,600,2100,1222,1300,4824,1560,2150,1900,1500,1850,1900,1700,2990,1620,1500,1300,1480,1425,1500,1618,1000,2600,1800,1500,1600,1700,550,2300,2120,2900,1700,1870,1100,1900,2800,1800,1266,2175,2292,1400,1200,900,1530,1140,5500,3800,1500,1600,250,1850,1800,1813,1540,2970,2914,3000,1800,1640,1500,1800,1830,2800,1500,2017,1700,2490,3000,1500,800,1500,1330,5000,2300.84,4474,1415,2660,2400,700,1350,2400,2080,3000,1404,3500,1800,1000,1900,1670,1500,2100,1600,2200,1400,2400,2000,2600,1430,2841,1550,4500,4500,2000,1300,2000,1600,2400,5000,1500,1747,1700,4000,2200,1400,2500,1000,2800,1500,1200,1300,2000,1600,3300,2000,2800,2200,1550,1600,1882,3300,1680,1500,5500,4883,1425,2146,900,1000,2391.92,1500,2300,1100,2300,1500,3000,2730,2900,1900,1400,2200,1560,1900,4900,2015,3800,4500,693,3900,1850,1800,3200,1700,2300,1800,1100,1000,3500,4733,3000,2600,2000,1900,1750,2100,2450,1500,2100,600,1800,4000,1885,3250,2500,2600,1100,455,500,1500,2240,1600,1700,2200,1560,3550,1400,1535,1500,2300,2800,2400,2026,1400,2150,2190,1500,5000,920,2000,1700,900,851,3300,2200,2200,500,1700,1500,5500,3625,1321,2500,5400,1800,3300,2300,2600,1400,668,2300,2200,1600,1950,975,1200,1600,2100,1400,3000,1317,2500,4000,1750,1600,1000,1950,4200,1426,2800,2100,3000,1500,2300,2000,1500,900,1781,2600,656,5200,1289,1800,1600,1222,1800,2000,1940,2000,710,1800,1500,2000,2666,2500,1560,1400,1950,1200,1800,4000,1676,3684,2600,1750,1600,910,600,1600,952,1509,1800,3377,2000,1440,1300,3900,1500,1900,2500,2200,1000,2400,170,3200,2700,3600,1700,2200,2470,1000,2900,1650,2400,4000,1700,1800,2280,1700,1800,2000,1560,1553,526,1100,2400,1350,2469,2600,2100,1650,2000,2100,2900,1500,1713,650,1008,1458,1000,1700,2000,1380,1950,1509,1768,2700,760,1500,1850,1400,1800,1840,1639,3500,1000,1300,2375,2600,2500,1700,2143,1750,1300,1718,3500,1400,1626,3400,2000,700,2000,3300,2800,1000,850,859,700,3900,1119,2000,2200,2700,452,2500,2400,1974,1400,2000,1500,1400,750,1000,2376,1500,1600,1400,2000,1100,1900,2288,3640,1399,1500,1400,3000,1800,2000,3500,1344,2300,1500,260,3900,1644,1200,3000,2000,1750,1800,1280,2320,3800,2800,900,2040,2000,2340,2800,1900,2633,1950,1700,1840,2300,1900,2000,2000,220,2300,3535,2080,5000,3000,1100,1600,3000,2600,1700,1600,356,1380,2200,4160,1300,2600,2490,3000,2000,1400,1052,936,830,2080,3380,1600,1500,800,2200,2600,2240,1533,2000,1820,2620,2200,1800,1500,4000,1590,900,350,1447,1326,2700,4000,1600,1725,1000,800,1600,2516,3500,1446,2200,1560,1600,1100,1450,3500,3500,1600,1600,1300,2925,2000,1500,960,3000,135,1805,1900,2700,1900,2200,1300,2000,2040,4900,2100,1400,1850,2000,2927,2700,4200,4758,3600,3500,1780,1900,1300,1900,2600,1500,1400,1700,2370,3645,1609,1750,2500,2100,1200,2080,1700,2800,1200,2200,1900,3700,2000,3200,1564,1400,2100,300,930,2800,2400,2283,3500,2139,1800,1600,2000,2900,1200,4000,3000,1400,1400,1750,2500,950,2292,2200,1850,1300,1900,1400,3200,1400,2400,3000,2300,1140,2580,4000,1300,2500,2625,699,3200,750,1600,2800,3500,1700,1650,2800,1800,1200,1761,1600,1200,1956,1400,850,1179,1178,1400,1500,1800,800,2237,1270,2500,1430,1350,2162,2300,2518.58,2000,2380,1600,749,1100,1700,2300,4200,1500,1400,860,1800,2700,2600,1200,1300,1550,3500,2700,3865,1600,2200,950,2800,2990,1500,1426,2100,2200,1600,1450,2300,1441,1625,2500,1500,800,2211,2200,1430,1400,900,4000,2111.87,1498,2200,1600,1400,1560,2900,2900,1750,651,2080,996,3600,2050,1400,2700,1690,1400,1800,1200,1300,3250,450,1950,2296,2980,2317,3067,5500,3800,2000,1545,1064,600,150,400,5000,1800,2392,1600,1800,2730,1500,2300,1686,2180,2300,1800,1600,1200,1500,1650,2100,1800,3900,1600,1100,1500,1356,1800,1600,1200,1820,1800,2000,1800,1100,2400,2400,1500,1700,1100,2000,1500,3147,2200,1200,1400,900,2600,1900,1500,2700,1425,3057,4737,1900,2500,1400,3263,2300,2200,2000,2900,1600,1500,2200,1500,1100,1250,1400,3549,1900,2000,2200,2470,1350,3000,1400,1500,1600,1600,2162,1600,1600,3090,1648,1050,1500,2000,5000,1700,1850,2100,2650,1722,4100,1425,1700,1700,2000,1418,2000,2000,1600,1430,1400,1483,3650,1400,1950,1200,1900,1400,2300,1800,1200,1300,1755,2000,1600,1700,1555,2600,1400,2000,1560,2600,1843,2400,5200,985,2000,3600,1518,2000,330,500,2300,1425,3500,1400,2300,1800,1495,2500,2470,2500,510,3300,1200,5100,1400,3000,1680.33,1700,2120,1700,1690,3659,1300,1400,1604,900,700,790,2450,3000,2200,1700,4444,1950,1800,2100,2300,1833,1800,1900,4400,2100,1319,1800,1700,2100,2100,1750,1300,1000,2400,2210,1624,1180,3398,2000,2200,1700,3200,1563,900,2300,1100,1096,1560,2400,1500,1200,1300,1600,1900,1700,1550,3700,1000,1200,1254,951,2100,1700,3000,1200,1680,1800,2600,2405,2000,1700,1500,1050,1800,1550,3800,1800,1716,2250,2000,845,1800,1100,1428,3200,2000,1049,1504,4200,1400,1400,5850,1900,1800,2600,3000,1400,4400,1892,160,2218,2000,2800,2051,2300,3300,2800,2100,2000,720,1820,1150,1924,1450,3965,1950,3000,1463,1590,1300,1800,1465,2470,2500,1600,2000,1516,900,1657,400,1650,1700,176,2600,1700,2000,1300,2388,2900,1412,1500,1000,3200,3961,2250,1500,2668,2400,2089,2000,1500,1800,1600,2300,2500,1200,1700,4000,1500,950,1150,5800,2730,1800,900,634.12,1400,1300,1900,1750,1200,1700,2500,1450,400,1050,2988,1600,360,2000,1456,1600,900,4000,1693,3300,1800,3250,1400,1300,940,1100,2300,1400,1850,2500,2500,2000,2530,3000,1800,410,2600,1000,2210,2900,1050,588,2200,1967,2800,1260,3000,1869,2500,1800,1480,1400,850,1876,1600,4500,4500,3400,2900,963,1800,3700,1047,850,3000,600,2000,1850,2500,1300,1400,1625,600,1450,2340,1690,1700,2200,2500,2300,4000,1600,1200,1010,5000,2600,1263.87,1560,2300,1062,2300,900,800,1500,3800,1400,1896,750,1700,1743,300,1469,1700,1800,1600,1506,2500,1700,1518,1859.25,755,1800,1600,1365,1200,3800,1450,3000,3600,5500,1400,1140,1538,3500,1300,1500,1800,1794,1977,2100,2700,1600,2200,2496,1500,1900,1495,2004,1800,2300,1350,2700,1700,1500,1211,2400,4400,2500,2018,800,1128,2500,650,2500,1775,2100,1690,769.61,887,1700,2500,2600,1800,4000,2340,1800,2200,530,2500,1900,1272,4200,5000,1600,2210,2500,1600,1689,2100,1200,950,2000,1800,1500,1400,1200,1400,1600,3000,2000,2000,2500,1200,1900,2200,1700,1750,1770,1500,1000,2500,1350,1952,2000,1630,2400,2500,1180,1400,5200,400,4000,1012,2700,1800,350,2800,1600,1900,3400,4200,2960,4685,3250,2120,956,1649,1400,2700,2390,3200,1450,2500,1100,900,2340,1425,1300,3000,2800,1400,1850,392,1430,1500,2500,660,1600,5700,1450,1750,3000,1800,2000,1500,5600,1700,1500,2000,1484,2005,1680,1820,2400,313,1800,2600,1950,1132,2104,2500,3100,1800,3500,814,1900,1500,1900,1300,2400,3200,1700,2496,1550,1789,1727,2000,1400,2200,800,1500,585,1050,1500,2210,4300,2300,2300,3000,1800,2300,1600,3500,2200,2028,1550,1500,1500,1426,1800,1500,2400,906,2479,1600,750,3400,1950,1000,1800,1650,2800,3200,1560,1900,1900,4300,2500,2380,1568,1700,2700,3000,3600,1700,2000,2000,2150,2400,1200,4800,1300,1835,2000,688,1476,1800,3000,1200,1300,1600,200,1650,1600,3200,814,2597,2000,3460,1500,1600,4500,1500,2300,1170,3000,1600,816.2,1100,950,2100,900,1200,1500,2200,2700,1688,1600,1800,1350,2052,2500,1560,1689,1800,1630,2000,866,2033,280,115,1600,5200,2600,3800,2500,2125,3000,800,1200,1700,1350,1560,1800,1400,1200,1500,1500,1900,1100,1706,3600,2500,1850,980,420,1400,2050,5500,700,2400,2000,4100,1200,2600,4680,2500,1600,1450,1080,3000,1200,1200,4900,1200,2100,3250,1518,1440,1430,1300,2400,1200,383,3000,2400,2900,870,1580,997,1760,3300,2750,1800,1400,3690,2840,1550,2200,1500,1700,1200,4500,1800,3500,2700,2850,1520,2800,4200,2400,1850,990,2400,3450,2700,1200,1430,2350,1900,1500,2026,1200,1700,3500,3500,1550,2500,3000,4800,2000,1614,1300,3200,610,1300,2900,2500,1600,1900,1200,935,400,2100,2275,1400,2000,290,1699,1400,1100,1900,1600,1555,2200,1800,3500,2459,1400,1450,2080,1800,950,2500,1440,3000,1000,1800,1054,1585,3900,2800,4600,1400,2100,2395,1380,3000,1900,1850,1800,3200,3000,600,1400,750,1500,1800,1300,1400,3400,2400,3200,1850,1700,1800,2000,1380,2700,2051,1300,3000,1500,1500,1300,2400,2860,4072,2100,1700,1000,1200,1700,1800,1400,3356,2100,1517,810,1600,2000,2000,1510,3670,3400,3900,2880,1839,1649,1600,1565,1600,1350,2200,2000,1233,1500,1800,250,900,2500,2100,1700,3800,1900,1820,714,2300,1400,3640,1444,2100,1400,3200,2500,2500,712,1600,2300,2100,1690,2400,2000,2000,860,1500,2300,1222,2650,1300,1150,2000,3080,1700,150,2400,1800,2502,5200,1947.62,1560,2200,280,1850,1433,1699,2700,1300,1600,1150,1228,2500,1800,1550,1540,1850,1200,2000,1300,1300,1950,1499,1798,500,1700,2500,2014,2100,3400,1800,680,1300,1550,910,5000,1610,1800,1900,1700,2698,1300,910,2145,3000,3400,900,1750,1548,1900,1939,436,3430,2400,1490,830,1400,1700,2000,294.32,1500,2700,2200,1754,3848,2600,1450,400,2100,1450,1300,2300,1495,2300,1700,1900,1900,1570,1300,3000,1600,1456,2300,1300,2100,1950,200,1750,1800,1600,2700,2025,2100,1926,1968,2500,1900,2000,3000,3000,3300,3500,1700,1250,3000,1860,1550,977,1700,1500,850,1660,1800,1700,1700,2630,1151,1800,1740,2487,2000,1750,2250,2750,800,1600,1921,1800,2200,1509,2974,820,1700,1600,1400,2000,1800,2670,1300,1800,2300,505,2000,1800,1400,850,2200,1600,2300,2000,1800,2500,2000,1300,1729,430,1900,1000,2300,3500,800,2400,1400,1560,1426.13,2400,2800,943,1900,2340,2300,1300,2600,2500,2400,2200,3300,2171,1300,859,3300,1800,1924,3000,2100,2100,2378,2000,1800,1900,2392,2400,3250,1550,1900,1000,1350,1600,1900,700,3800,3848,3000,900,400,1650,4783,1400,1971,2051,3300,2500,2300,1600,2700,500,1350,1500,2000,2300,2700,5000,1700,1400,2100,1800,3000,1500,2200,3200,2600,750,2048,1560,4500,1300,2656,533,1440,1200,1222,2300,2000,950,1800,700,2300,2900,1500,3298,1100,1986,350,3200,2600,1400,2833,2500,1700,3200,2750,570,1450,2000,1950,1024,2900,1400,2315,1600,2500,700,3000,910,1319,1826,2210,950,1828,1350,2400,1950,2200,1100,2600,1700,1880,1900,2000,3000,1610,1200,3000,1500,1400,2291,1600,2000,1500,5500,1400,1500,1200,1300,1750,2700,1660,2015,525,1350,4700,1400,1900,999,2500,800,440,3900,1000,869,2250,1500,2500,1820,2400,2900,1790,1200,2416,2750,900,1800,1500,1400,1950,1845,1800,3000,1300,1000,3500,2535,1820,3400,1800,3200,4000,1500,600,2500,1440.02,2000,1600,900,500,1400,5000,1535,1270,2000,1800,2300,2200,200,3700,1620,2100,2500,2100,1490,2100,1500,2500,2500,2550,1000,2800,2000,1929,3500,500,1600,600,2332,2300,1593,1760,1100,590,1300,1950,1300,2400,2000,1450,600,1500,458.48,2833.73,3300,1456,1700,2500,730,1800,1500,1500,2100,2100,4000,1700,1000,1600,1800,4000,2400,1859,2000,1300,2100,1700,5500,3600,1900,2500,1400,3400,2191,1700,2005,2000,1500,2818,3300,2800,1150,1700,2480,2400,1814,650,1700,1600,980,2500,2300,5000,1600,1380,1400,1700,2302,1800,2470,2850,1400,1000,4000,1554,1000,1675,1758,2450,2000,1400,1025,510,4000,770,1900,1200,1449,2500,2200,1500,2160,2500,2020,950,3200,800,1971,2000,2200,1700,2275,850,2100,1429,4300,1600,2300,4000,3250,2600,1750,1800,3300,2000,400,705,3400,1885,1653,3300,900,200,4500,2650,2000,2000,3000,2100,1900,3600,1293,2080,2900,1400,900,2000,1808,1463,2456,1700,1417,360,1775,1600,2100,2400,1100,1030,1640,1587.48,2500,2025,1450,1500,2400,1500,3400,1577,1450,2245,750,2200,1657,2300,1500,900,2550,3200,1800,1900,3500,900,4500,1600,2300,1700,2100,2000,1200,1600,1000,4500,2074,1517,2100,4300,2100,1660,1000,1100,1550,3000,1400,3224,1040,1500,1250,2000,1500,2200,1100,1756,2500,1670,1600,3431.04,2002,2300,1600,1500,1300,1700,1500,1636,1950,2200,656,2600,2500,2600,1000,3000,750,2000,2500,2200,2790,1700,4500,1000,1500,1425,1900,2300,2800,980,2200,1500,3000,947,650,1800,2400,3000,1424,2650,2500,1766,2000,4600,3700,1800,2000,1763,2770,612,2100,3000,1800,3120,2600,4000,2000,2600,1500,1200,1550,2000,248.5,1300,1820,3000,2371,1560,2700,2180,3000,2000,3600,1895,2000,1800,400,2480,2600,1000,785,1700,1040,2400,720,2500,1800,1000,3200,330,250,1200,1900,360,3000,650,1500,1200,1450,3555,1200,800,900,680,1700,1200,510,2100,1800,1063,950,4755,200,1700,2000,1150,574,750,533,1400,2000,2300,1200,1340,1300,2000,1000,1400,2200,2000,500,1400,800,2300,1900,700,2500,1950,1284,1600,2100,2500,900,450,1700,2000,1366,2000,116,1500,1400,2600,250,3000,1500,700,208,800,1500,1900,850,900,575,1800,1600,2400,210,1100,1200,1400,700,2300,700,1300,1000,240,2100,1300,1600,300,1800,841,1500,1400,650,554,320,1200,1150,412,1200,1487,2100,1700,2500,480,1100,1500,1250,3216,2000,2000,1428.5,2100,800,800,5000,499.7,1000,2600,255,1700,400,600,500,420,1916,1900,1000,1400,1450,2300,1200,2147,600,1200,160,820,400,1800,1200,720,6000,1700,525,1000,1040,1100,800,2010,2000,950,2000,1316,2000,1100,1700,4000,2500,1000,1700,1530,1000,1000,1200,1700,650,1500,1700,1100,2400,460,3000,3949,3000,1200,1000,1100,1000,2500,178,600,490,3500,1500,450,595,1000,816,650,2300,980,600,1500,2100,748,1800,1250,4120,600,835,700,2500,1300,1450,800,325,2500,830,2000,700,1700,2400,1300,1800,916,2000,2500,498,2647,2000,700,2500,850,700,330,1200,2000,1500,3580,670,1400,650,1800,1600,3000,350,1650,2350,2500,1500,1000,2090,900,1000,1000,700,500,1200,1285,1100,1300,2350,1100,2200,1400,1500,2700,1250,2054,450,350,1950,2400,1400,200,3000,168,600,1800,400,1045,1502,2300,900,1400,1200,230,450,2806,1320,3000,1250,2000,1600,1700,1392,900,750,2500,1200,1000,1800,850,2500,595,700,2000,1800,2000,1150,2100,2700,1000,550,1300,2000,1600,1200,2300,2900,1000,800,500,760,1800,1400,3000,2200,600,1500,1100,1800,2000,940,800,2300,500,500,2500,350,800,3000,2750,412,1250,1500,1100,1500,1026,2000,561,1400,460,670,1300,440,2000,1235,480,836,1250,1700,1235,1000,1500,1600,980,1100,1800,1200,520,3500,3200,1800,1700,2000,1000,560,2200,3265,560,1000,1400,1333,2300,3600,1400,1436.23,1385,410,600,1000,1000,600,550,1000,1000,2200,1000,1400,1800,440,1000,3400,10000,2800,600,1300,1300,2633,1800,800,930,950,2000,934,2500,560,527,1500,2400,400,2100,2000,3500,2300,538,1300,500,4000,2000,3500,800,1500,2210,3200,1500,1200,3000,500,3600,2800,3000,930,1600,1550,400,1200,1600,3346,1200,900,2200,1800,400,560,1500,2000,1800,1230,2000,1200,2100,863,2100,550,700,2200,1200,1150,1300,310,930,580,1500,1500,1100,1000,1400,2500,1500,4750,1300,1100,2400,1700,500,1300,1500,2975,987,890,2175,600,2700,1000,1000,1593.83,1200,2600,1450,3000,2002,1500,1500,500,700,1200,460,1507,2100,600,1060,1300,4200,1200,1000,500,3747,2500,230,1000,660,1250,1600,1200,2500,1900,1000,2700,297,1100,2000,250,1000,1800,3200,1300,850,1500,1000,700,1800,2400,1000,1300,1600,2000,600,800,1000,2000,400,800,4250,3600,540,800,2200,750,900,1750,1050,1384,1565,3000,2100,1775,1958,232,1684,989,3000,1200,480,2300,450,2000,982.37,3200,1500,500,3571,1500,1200,390,3180,1300,1100,1200,1200,1700,1300,800,750,700,1875,1300,800,1900,1400,1700,500,1000,1000,1000,800,1100,1600,3000,1100,1500,2300,2200,800,3000,1000,218,400,1400,2200,2000,1793.25,1300,8000,1200,3100,1300,1900,474,3700,1600,1400,800,825,1300,2700,490,1300,2000,1100,2900,1850,340,2000,1500,1500,2500,3700,1200,2000,1900,650,600,600,1866,1540,2300,2300,1000,1100,1000,2500,1950,1300,3455,1700,750,350,1400,1292,1600,540,800,950,1063.38,2000,970,2000,1300,200,850,1100,2200,600,1400,600,1100,1050,1900,1200,1900,2000,2200,2000,600,2500,1700,1900,484,161,3200,870,320,1750,1500,1600,960,1945,3000,1135,1250,1300,2300,2200,594,1120,750,800,2000,1800,1300,1000,580,2800,4000,2464,2700,1215,1281,1300,1002,3500,4000,1000,1000,1500,2100,400,2800,3000,1000,600,629,1100,1100,650,1100,1700,3000,1300,1500,1000,1000,230,600,3000,300,1204,500,800,2020,1800,1000,2400,3600,1000,750,350,600,460,283,1000,500,200,1900,2000,1200,1200,700,876,2125,2046,1500,1000,608,2500,1250,440,1100,1000,379.52,700,2110,1400,800,1446,520,2000,500,2100,2000,2400,1300,1200,2100,1700,2400,1000,1000,1490,1800,2000,3500,370,1480,1900,459,1000,550,1450,3000,2000,2400,1900,440,1000,325,446,850,1400,2000,2300,1200,550,1350,1790,3070,220,2400,2500,860,1800,500,200,900,1900,800,700,950,1500,1300,9000,5000,1000,2100,1200,1400,1500,1500,2400,200,900,2500,1500,2200,2800,2600,1500,1000,1000,1700,2200,1500,320,6500,565,1000,1200,1100,2629,3453,300,1800,2491,1000,1200,1400,475,1500,3500,1650,1100,2500,3171,3500,600,2000,2000,2500,2300,2000,3000,2200,450,1200,1100,1000,500,800,3000,1500,1800,1800,420,1500,1800,1350,3000,890,850,3600,1600,500,2000,950,1800,1800,2500,1500,800,1950,1800,2000,1500,2000,2000,1200,1090,680,550,2100,3000,800,2500,1200,2300,2000,2300,800,1200,2300,980,2100,1589,4000,1600,2000,876,960,296,410,2199,1400,750,1200,300,211,187,850,430,1650,6000,1800,614,1850,900,300,2642,600,1150,500,2700,1040,2900,400,750,3771.67,1700,1500,1400,1300,1900,1004,1300,10000,500,1000,2400,1800,689,1400,650,800,165,850,1250,1100,1400,930,600,975,1600,700,600,1000,416,2546,1000,568,1264,1400,1600,540,1100,1250,1400,2500,3000,550,200,1200,1750,4120,200,1200,2500,2000,1000,2500,410,550,1000,1800,2500,1004,1800,1200,1900,850,1700,400,1200,494,1134,1800,1300,950,2500,1600,2200,1800,1200,650,3000,900,500,1300,2500,2259,950,495,3200,2200,2874,357,1200,2300,1200,1700,1800,2500,1800,1000,4000,3000,770,1800,800,1550,930,1000,3700,400,900,1700,897.49,3900,2500,500,1600,1000,1600,900,2000,2100,1600,1100,1700,1500,1500,2900,1000,3200,3200,2000,800,1330,4000,1500,1000,1700,1900,750,2500,1900,1900,2000,1700,600,1300,1500,1550,1700,900,1800,1800,2000,1200,2000,2200,2400,2670,800,2300,1800,1000,1800,800,2000,1900,1000,1100,2500,300,1600,3000,800,2300,1400,1600,2000,4200,3500,1600,1900,2500,1800,900,1600,1700,1800,1200,2000,3200,2300,600,2000,3500,2100,900,1300,3000,3000,4000,2000,1600,1100,1600,2000,1700,1300,1650,2500,2000,1500,1500,2000,1600,1450,1600,2500,1350,1700,1900,5000,1400,2700,1340,1400,1000,2100,1700,2300,2100,3500,1400,2000,1500,2100,1100,2000,1825,1300,1900,1800,2000,1574,1900,1100,950,2200,900,1800,700,1300,1100,1800,1800,2500,1553,1700,1600,1300,2800,1700,1300,1100,2200,1300,2500,1200,2100,1300,1700,1700,1500,1600,1700,1500,3000,1000,1439,1300,1350,2000,150,1300,1500,1800,800,1300,1751,1650,1300,2400,1500,2600,1900,2300,1800,1300,1700,3000,2000,2400,1300,1500,5000,1700,2000,1600,1300,370,2800,2800,1200,1700,5000,2400,1200,750,1200,2000,1000,1300,1800,1000,2200,2000,2000,1800,1800,5000,1700,1200,1538.8,2100,1700,1900,1800,1500,3500,1600,1650,1600,1300,1700,1150,1600,2000,2600,1306,1200,1377,2400,2600,1100,1700,1800,725,3000,1000,1500,2400,2800,1000,2115,2500,2000,1500,3800,2400,1250,3000,1400,800,1800,600,1300,1400,1100,900,1900,3000,3000,2800,3000,1500,1700,1600,1900,2000,1900,1200,1500,2500,1100,700,2200,1800,1763,1100,1600,2100,1300,500,2300,1500,1300,900,1000,1600,1413.1,1400,1200,1600,2300,1900,1340,800,2500,1800,1224,1200,2300,1000,1700,2200,2500,2600,1000,2200,3500,1400,2000,1200,1700,1800,800,1700,1500,1100,3500,2000,900,1800,1300,1800,2000,2100,2000,1700,2000,700,2000,2200,1500,1500,1000,1250,1600,800,2200,2200,2300,2200,2300,1000,2200,1100,1800,1800,1300,4000,950,2200,1500,1300,1700,1100,1500,950,2000,1350,2400,3500,3000,400,1400,1900,1050,2100,1100,3000,2100,1100,614,2500,1400,400,1450,4000,500,2500,1936,1570,1300,1500,1600,1400,1400,5000,1500,1800,2000,1300,1800,1900,1400,3000,1300,1200,1600,1500,1600,1900,1700,1800,2217,2000,1300,900,2200,700,3000,2000,1600,1800,1500,850,1350,4500,800,2200,3200,2000,1600,1500,900,2000,2100,1800,850,1700,1400,4000,1800,2500,700,2664,2500,1800,2023,2200,400,1800,1400,1840,1100,3500,1600,1300,2200,1400,1500,1300,1400,2750,1300,1100,1600,1600,1000,1250,1300,2500,1200,4000,700,1400,1800,1200,1600,1880,1900,1300,1400,1800,1760,3000,650,1500,1400,1500,1200,520,2000,1300,1500,2100,800,1700,2500,1850,1700,2000,900,1700,1900,1400,900,1300,1000,1200,1400,1500,2000,1100,2200,650,1500,2700,2100,1000,1600,2000,1600,2000,500,3000,1800,1600,1200,3000,1300,450,1580,2000,1900,1600,1600,2000,2200,1900,2300,2800,1000,2500,1600,1630,1600,4000,1500,1500,1400,800,1839,1200,5000,3500,1840,1400,1283,2500,1400,1900,1400,1200,1700,1600,1400,3300,550,2300,1700,1500,1100,3500,2400,1000,2000,980,900,1700,1500,2015,1039,1850,1700,2500,1600,1278,1000,1900,2000,1400,550,1300,1600,1400,2500,1000,1000,3000,1300,2500,1600,2600,2000,3000,1200,1200,1400,1200,1200,1800,1800,400,1000,1400,2200,2000,2000,1500,1400,2200,2200,3000,1700,1450,1800,2000,1000,3000,2800,1900,5000,2535,4500,1900,2452,1160,2600,1000,1200,700,1900,4000,540,1800,2000,1100,3000,1900,2400,600,1200,1500,2000,1000,2100,1600,2000,1500,1600,1400,1000,1500,2700,1300,260,1600,3000,1800,1000,1400,1500,1050,724,1500,2800,800,1500,1100,2600,1200,1600,1200,1300,2740,1800,700,2146.79,2500,2500,1300,800,2500,1900,2200,1300,1700,1700,1200,1500,3000,900,1600,3600,1800,1800,1000,1600,1500,1800,250,2000,1300,1350,2400,2500,2000,2000,850,3600,1600,1200,1400,1100,1560,1100,1500,4500,1700,2600,1800,2000,2200,2900,1600,4544,3500,1500,1300,2300,1800,800,1300,1000,3500,1700,1400,3200,2900,1100,2000,1200,1700,1600,3700,1700,1400,1700,1600,1850,1700,1600,500,2500,1900,3100,2100,1300,1700,700,1500,2100,2000,450,2300,1500,1400,1812,1200,950,1400,1900,1600,2000,1300,3500,2000,2250,1961,1300,2000,4500,1500,1700,1600,2000,2000,1200,2600,1600,2000,1500,1900,1000,3000,3100,1700,2700,1680,1400,1000,1700,2600,1900,380,2000,3500,2000,1300,1300,1480,1700,4400,1800,300,1300,1700,2100,794,1800,3000,900,1000,2400,2200,1800,1600,3600,1900,1300,800,3000,3200,2300,2000,1700,1000,1985,3500,800,1600,2000,800,700,1700,1600,1500,1800,1500,1800,1400,1900,2000,3000,2300,1319,400,2000,580,1800,2000,1600,1975,2000,1400,999,1400,1200,900,1500,3900,4000,1750,1400,2800,1000,2500,1000,2000,1700,2000,1240,4600,2350,2900,1400,2400,3000,3000,1700,1400,2000,4000,4000,1450,940,1900,5000,999,750,2200,1700,1800,2500,2400,1500,980,2200,2100,1600,1050,1700,1200,1900,1200,1390,500,2200,1200,3000,1860,2200,1300,1500,3000,1500,1500,3040,1427,1250,1050,1200,1400,2800,1600,1300,1400,1600,2000,1400,1900,2200,1700,1900,2380,1600,1300,1100,4500,4000,1500,2000,1300,1600,2600,1700,1700,450,1000,3300,2800,1400,1800,2000,1500,2500,800,1200,1350,1000,1700,800,5000,4000,1866,1600,1200,1800,3300,1400,1700,1960,840,2700,1100,2500,2300,2000,1600,1500,1400,3500,1300,2300,1400,3500,1900,1258,1150,1800,3200,4500,2800,2500,1800,983,1400,2700,1490,2500,1400,2000,3000,1000,3300,1500,2600,800,2600,1800,3000,1400,2400,600,600,1500,1200,900,416.39,2100,1428,2800,4000,1400,1300,600,1800,2800,2700,2000,1700,1000,1400,2000,1500,2300,2000,1900,2300,1600,1410,1600,700,1200,4000,2000,1400,850,2000,2700,2800,2000,1600,1900,2000,1290,4000,1600,2000,1100,1900,2500,700,1629,2600,1900,1300,1600,2500,1300,1470,3500,2600,1600,1700,1200,1600,1397.3,1700,1800,1800,1800,1700,1800,2000,2200,950,1100,1600,2500,850,2400,2200,1200,1800,2100,1300,2800,1248,1500,1300,2600,1650,1240,2500,2800,1600,1800,1200,600,2000,1700,1200,2100,1600,950,1900,1400,4000,1000,3700,2000,1300,1900,1350,1400,2000,1000,3500,580,2700,4500,650,1000,340,800,2800,1000,2000,1000,1821,3000,2400,3300,1250,2200,1500,3000,1842,1650,1100,1300,2100,3300,2200,1600,1700,1591,1500,1600,700,900,1000,1250,1300,1300,850,1800,3200,1900,1500,2000,1800,1000,1500,300,1890,1000,950,1300,1200,1900,2900,2300,1800,1200,2500,2700,5000,2400,4500,500,1400,2000,4000,2190,1000,1500,700,1600,4500,2200,1200,5000,600,2500,1500,1200,1400,600,1000,2000,1600,2000,1280,3013,2700,1800,1200,2200,3392,1050,2500,5000,1550,2000,1200,2300,2000,2500,1900,3500,1600,2700,800,1500,250,1560,500,1000,2900,1920,1700,2300,1500,700,1900,780,3500,3500,1800,1500,1800,1700,1400,1300,1950,1700,1500,3000,1600,1500,2700,1600,3000,2000,900,900,1500,2600,3900,1500,2200,2000,1500,3600,900,1100,2500,1800,1400,2500,1000,1600,850,1200,1600,1600,1200,2600,1400,4500,750,2000,2000,1800,900,1500,2500,4000,850,1350,1500,1800,2500,800,1400,1450,2000,5000,500,3600,2500,1900,2300,2500,1750,1700,1100,1800,1800,1200,1400,800,3600,1500,1800,2000,1300,1500,1700,3300,2100,2200,1800,1600,2800,2800,1100,2000,1480,4000,1300,750,1800,3000,1400,2600,1540,1200,1100,2400,1400,1200,1000,3000,2500,1300,1400,1900,3000,1400,1500,650,1600,1300,1000,2500,1700,1500,1300,1700,2500,1700,999,2200,1700,2100,2600,1800,2900,1400,1400,900,1800,2000,2400,4500,1900,1300,4200,2200,1400,1900,1900,1500,1688,2400,3000,1200,2150,1800,1500,3500,2000,1600,1900,1643,2542,800,2800,3000,1000,2000,1400,1100,1900,1500,1800,2000,1400,1000,800,2100,3000,1400,1200,999,800,2200,1750,2000,1500,2200,2600,1850,1900,1800,1300,600,500,1500,1900,1600,1800,1750,1355,2000,1600,1780,1400,1000,2500,1688,900,2500,2100,1600,3500,2000,1200,2588,1900,1200,1900,2600,1521,2000,1500,1300,1200,1000,1800,2500,1800,2100,2200,1500,1050,1960,1550,1700,1300,1200,1200,700,3700,4000,900,2200,533,1200,550,800,1400,1400,1400,1700,800,2100,2800,740,2000,2500,2700,600,1800,1800,2000,2700,1200,1580,1200,1450,1125,1300,650,250,2600,1607,1100,700,2000,1300,1500,1200,2500,1600,4000,800,2300,1300,1200,2500,1300,1100,1200,400,2300,1100,1500,1600,800,2000,2000,2500,1700,2000,2000,1200,1700,2400,750,1300,4000,1700,1400,500,1100,1500,2000,1700,4600,1650,900,1500,2200,1800,2500,1300],"Education":["Primary","Tertiary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Tertiary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Primary","Tertiary","Upper_second","Secondary","Tertiary","Primary","Secondary","Secondary","Tertiary","Tertiary","Primary","Secondary","Secondary","Primary","Secondary","Tertiary","Tertiary","Upper_second","Tertiary","Primary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Primary","Secondary","Tertiary","Tertiary","Primary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Primary","Secondary","Primary","Tertiary","Secondary","Secondary","Primary","Secondary","Tertiary","Tertiary","Upper_second","Upper_second","Primary","Upper_second","Secondary","Upper_second","Secondary","Primary","Tertiary","Tertiary","Secondary","Secondary","Primary","Secondary","Upper_second","Upper_second","Primary","Secondary","Secondary","Primary","Primary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Primary","Upper_second","Secondary","Primary","Tertiary","Tertiary","Primary","Primary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Primary","Secondary","Primary","Secondary","Primary","Primary","Upper_second","Primary","Upper_second","Secondary","Primary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Primary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Primary","Tertiary","Upper_second","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Primary","Secondary","Tertiary","Primary","Tertiary","Primary","Secondary","Upper_second","Secondary","Upper_second","Primary","Secondary","Primary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Primary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Primary","Secondary","Primary","Secondary","Secondary","Secondary","Primary","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Primary","Secondary","Upper_second","Primary","Tertiary","Primary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Secondary","Primary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Upper_second","Upper_second","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Primary","Primary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Primary","Primary","Secondary","Tertiary","Upper_second","Upper_second","Secondary","Secondary","Tertiary","Upper_second","Primary","Primary","Primary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Primary","Tertiary","Upper_second","Tertiary","Primary","Primary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Primary","Secondary","Tertiary","Secondary","Primary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Primary","Tertiary","Tertiary","Tertiary","Upper_second","Primary","Primary","Primary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Upper_second","Primary","Tertiary","Upper_second","Secondary","Primary","Secondary","Secondary","Upper_second","Tertiary","Primary","Primary","Secondary","Upper_second","Secondary","Primary","Primary","Tertiary","Secondary","Secondary","Upper_second","Primary","Secondary","Tertiary","Secondary","Primary","Secondary","Primary","Tertiary","Primary","Secondary","Secondary","Tertiary","Primary","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Primary","Primary","Tertiary","Primary","Upper_second","Secondary","Primary","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Primary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Primary","Primary","Tertiary","Secondary","Tertiary","Upper_second","Primary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Upper_second","Primary","Secondary","Primary","Primary","Primary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Primary","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Upper_second","Secondary","Secondary","Primary","Upper_second","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Secondary","Secondary","Primary","Upper_second","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Primary","Secondary","Primary","Secondary","Primary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Tertiary","Tertiary","Primary","Tertiary","Secondary","Primary","Upper_second","Secondary","Primary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Primary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Tertiary","Primary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Primary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Primary","Tertiary","Tertiary","Secondary","Primary","Upper_second","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Primary","Primary","Primary","Secondary","Primary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Primary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Secondary","Primary","Primary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Primary","Upper_second","Secondary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Primary","Tertiary","Primary","Tertiary","Tertiary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Primary","Upper_second","Tertiary","Secondary","Secondary","Primary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Secondary","Secondary","Primary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Primary","Tertiary","Tertiary","Secondary","Primary","Secondary","Secondary","Primary","Upper_second","Primary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Primary","Tertiary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Primary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Upper_second","Primary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Upper_second","Secondary","Primary","Tertiary","Upper_second","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Primary","Upper_second","Secondary","Upper_second","Secondary","Upper_second","Primary","Upper_second","Tertiary","Upper_second","Primary","Upper_second","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Primary","Tertiary","Primary","Tertiary","Tertiary","Secondary","Primary","Upper_second","Tertiary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Primary","Secondary","Primary","Secondary","Primary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Primary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Upper_second","Tertiary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Primary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Primary","Primary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Primary","Primary","Secondary","Primary","Secondary","Tertiary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Primary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Tertiary","Secondary","Primary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Primary","Tertiary","Tertiary","Upper_second","Tertiary","Secondary","Upper_second","Tertiary","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Primary","Tertiary","Primary","Upper_second","Secondary","Secondary","Secondary","Primary","Primary","Secondary","Upper_second","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Primary","Upper_second","Tertiary","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Primary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Primary","Tertiary","Tertiary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Upper_second","Primary","Tertiary","Secondary","Primary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Tertiary","Upper_second","Secondary","Primary","Secondary","Tertiary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Tertiary","Primary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Primary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Primary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Secondary","Primary","Upper_second","Primary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Primary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Primary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Primary","Tertiary","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Upper_second","Primary","Tertiary","Primary","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Primary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Primary","Secondary","Primary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Primary","Primary","Secondary","Secondary","Tertiary","Upper_second","Upper_second","Secondary","Tertiary","Primary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Primary","Upper_second","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Primary","Primary","Primary","Secondary","Secondary","Secondary","Primary","Secondary","Upper_second","Secondary","Upper_second","Tertiary","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Upper_second","Secondary","Primary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Tertiary","Tertiary","Tertiary","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Primary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Primary","Secondary","Tertiary","Tertiary","Tertiary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Primary","Secondary","Secondary","Secondary","Primary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Primary","Secondary","Upper_second","Secondary","Secondary","Primary","Tertiary","Upper_second","Upper_second","Primary","Secondary","Secondary","Primary","Tertiary","Upper_second","Secondary","Tertiary","Upper_second","Primary","Primary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Primary","Primary","Upper_second","Upper_second","Primary","Secondary","Secondary","Secondary","Tertiary","Primary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Primary","Secondary","Primary","Upper_second","Secondary","Tertiary","Primary","Upper_second","Tertiary","Upper_second","Primary","Secondary","Secondary","Tertiary","Primary","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Primary","Primary","Secondary","Tertiary","Secondary","Primary","Upper_second","Secondary","Upper_second","Tertiary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Primary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Tertiary","Tertiary","Primary","Secondary","Upper_second","Secondary","Tertiary","Primary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Primary","Tertiary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Primary","Tertiary","Secondary","Primary","Secondary","Tertiary","Tertiary","Secondary","Primary","Upper_second","Upper_second","Tertiary","Primary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Primary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Tertiary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Primary","Primary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Primary","Tertiary","Primary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Primary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Primary","Tertiary","Secondary","Secondary","Primary","Secondary","Upper_second","Secondary","Secondary","Secondary","Primary","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Primary","Tertiary","Upper_second","Primary","Upper_second","Upper_second","Tertiary","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Primary","Secondary","Secondary","Primary","Primary","Tertiary","Primary","Secondary","Primary","Tertiary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Upper_second","Primary","Upper_second","Primary","Secondary","Tertiary","Secondary","Primary","Tertiary","Upper_second","Primary","Tertiary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Primary","Tertiary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Primary","Tertiary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Primary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Primary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Primary","Secondary","Primary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Primary","Tertiary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Primary","Secondary","Tertiary","Primary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Primary","Secondary","Primary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Upper_second","Tertiary","Primary","Secondary","Secondary","Secondary","Primary","Tertiary","Secondary","Primary","Tertiary","Secondary","Secondary","Primary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Primary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Primary","Tertiary","Tertiary","Primary","Primary","Primary","Upper_second","Secondary","Tertiary","Upper_second","Tertiary","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Upper_second","Upper_second","Tertiary","Tertiary","Secondary","Tertiary","Primary","Secondary","Secondary","Tertiary","Primary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Upper_second","Primary","Tertiary","Upper_second","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Upper_second","Primary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Primary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Upper_second","Primary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Primary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Primary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Tertiary","Tertiary","Tertiary","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Upper_second","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Primary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Primary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Primary","Secondary","Tertiary","Tertiary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Primary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Upper_second","Upper_second","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Tertiary","Tertiary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Primary","Secondary","Primary","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Primary","Tertiary","Upper_second","Secondary","Upper_second","Primary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Primary","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Primary","Tertiary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Upper_second","Upper_second","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Primary","Primary","Primary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Primary","Secondary","Tertiary","Secondary","Upper_second","Primary","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Upper_second","Tertiary","Tertiary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Upper_second","Tertiary","Upper_second","Tertiary","Primary","Upper_second","Upper_second","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Upper_second","Primary","Secondary","Upper_second","Upper_second","Tertiary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Upper_second","Tertiary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Tertiary","Upper_second","Upper_second","Primary","Upper_second","Secondary","Tertiary","Primary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Primary","Tertiary","Tertiary","Tertiary","Upper_second","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Primary","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Primary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Primary","Upper_second","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Primary","Upper_second","Secondary","Upper_second","Primary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Primary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Primary","Primary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Tertiary","Upper_second","Secondary","Tertiary","Upper_second","Primary","Tertiary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Primary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Primary","Upper_second","Primary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Primary","Upper_second","Upper_second","Tertiary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Upper_second","Upper_second","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Primary","Secondary","Upper_second","Secondary","Upper_second","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary",null,"Secondary","Upper_second","Tertiary","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Primary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Primary","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Upper_second","Tertiary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Primary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Tertiary","Upper_second","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Primary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Primary","Primary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Upper_second","Primary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Primary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Primary","Upper_second","Tertiary","Primary","Tertiary","Secondary","Primary","Secondary","Primary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Primary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Upper_second","Tertiary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Primary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Primary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Secondary","Upper_second","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Primary","Upper_second","Upper_second","Secondary","Primary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Primary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Upper_second","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Primary","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Upper_second","Secondary","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Upper_second","Tertiary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Primary","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Primary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Upper_second","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Secondary","Upper_second","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Upper_second","Secondary","Upper_second","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Primary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Primary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Primary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Primary","Primary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Tertiary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Primary","Secondary","Primary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Primary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Primary","Upper_second","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Primary","Primary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Tertiary","Primary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Primary","Tertiary","Secondary","Secondary","Tertiary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Tertiary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Primary","Upper_second","Secondary","Secondary","Secondary","Secondary","Primary","Upper_second","Primary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Upper_second","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Secondary","Primary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Tertiary","Upper_second","Tertiary","Tertiary","Tertiary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Primary","Tertiary","Primary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Primary","Tertiary","Primary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Primary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Primary","Upper_second","Upper_second","Tertiary","Secondary","Tertiary","Primary","Secondary","Tertiary","Secondary","Primary","Secondary","Upper_second","Primary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Primary","Upper_second","Secondary","Tertiary","Upper_second","Upper_second","Upper_second","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Upper_second","Upper_second","Upper_second","Secondary","Primary",null,"Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Primary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Primary","Secondary","Tertiary","Secondary","Secondary",null,"Primary","Primary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Upper_second",null,"Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Primary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Primary","Upper_second","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Upper_second","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Primary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Primary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Primary","Tertiary","Primary","Primary","Tertiary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Tertiary","Upper_second","Upper_second","Tertiary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Upper_second","Upper_second","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Upper_second","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Primary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Upper_second","Secondary","Tertiary","Primary","Secondary","Secondary","Primary","Tertiary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Primary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary",null,"Secondary","Primary","Secondary","Tertiary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Tertiary","Primary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Upper_second","Tertiary","Upper_second","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Secondary","Upper_second","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Tertiary","Secondary","Primary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Primary","Tertiary","Upper_second","Upper_second","Secondary","Primary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Tertiary","Tertiary","Tertiary","Upper_second","Tertiary","Primary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Primary","Tertiary","Primary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Tertiary","Tertiary","Primary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Primary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Secondary","Primary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Primary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Primary","Primary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Primary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Primary","Secondary","Upper_second","Secondary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Primary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Secondary","Primary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Primary","Upper_second","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Upper_second","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Primary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Primary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Primary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Upper_second","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Primary","Upper_second","Secondary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Primary","Upper_second","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Upper_second","Secondary","Primary","Upper_second","Upper_second","Secondary","Secondary","Tertiary","Secondary","Upper_second","Upper_second","Secondary","Primary","Tertiary","Upper_second","Primary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Tertiary","Tertiary","Primary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Upper_second","Upper_second","Upper_second","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Secondary","Upper_second","Tertiary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Upper_second","Secondary","Primary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Primary","Secondary","Primary","Upper_second","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Secondary","Primary","Tertiary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Upper_second","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Primary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Upper_second","Tertiary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Primary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Primary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Secondary","Secondary","Secondary","Primary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Primary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Secondary","Tertiary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Primary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Primary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Primary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Upper_second","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Upper_second","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Primary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Primary","Tertiary","Tertiary","Tertiary","Tertiary","Primary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Upper_second","Upper_second","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Upper_second","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Upper_second","Tertiary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Primary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Secondary","Primary","Primary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Secondary","Secondary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Primary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Primary","Tertiary","Secondary","Tertiary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Secondary","Tertiary","Secondary","Tertiary","Tertiary","Secondary","Tertiary","Upper_second","Tertiary","Secondary","Secondary","Primary","Secondary","Tertiary","Secondary","Tertiary","Secondary"],"Education_years":[6,15,12,6,12,12,15,10,15,15,15,15,10,17,12,10,17,15,14,15,15,14,12,10,12,17,15,12,12,14,12,6,15,14,10,17,6,12,10,17,15,6,12,10,6,12,15,17,14,17,6,17,17,12,12,14,6,10,17,17,6,10,15,15,15,10,12,17,6,10,6,17,10,10,6,12,15,15,14,14,6,14,12,14,10,6,15,21,10,12,6,10,14,14,6,12,12,6,6,17,12,15,10,12,14,10,17,12,10,17,10,6,14,10,6,15,17,6,6,10,15,10,15,15,14,12,6,10,6,10,6,6,14,6,14,12,6,15,10,10,12,12,10,10,10,12,17,6,10,6,12,17,10,17,15,10,12,6,17,14,12,17,14,15,12,12,12,15,6,12,6,10,17,6,15,6,10,14,10,14,6,12,6,17,15,12,17,12,15,10,6,10,10,12,10,15,14,10,12,14,17,17,12,10,10,10,12,12,10,17,10,17,6,15,15,12,14,10,10,12,6,12,6,10,10,12,6,14,17,10,15,12,10,10,17,14,6,12,14,6,15,6,14,10,10,14,10,12,6,10,15,10,15,17,17,10,14,14,12,17,15,15,12,15,10,6,6,17,15,10,10,12,10,11,6,10,6,6,12,15,14,14,10,10,17,14,6,6,6,12,14,12,10,15,15,10,12,15,12,6,15,14,15,6,6,15,12,14,15,10,12,12,14,12,10,10,10,6,12,10,6,10,15,12,6,17,10,14,10,12,12,17,6,10,12,6,12,10,17,12,15,15,12,17,12,17,6,15,15,17,14,6,6,6,17,14,17,10,10,12,14,6,15,14,12,6,12,12,14,15,6,6,10,14,10,6,6,17,10,12,14,6,10,15,12,6,10,6,17,6,12,10,17,6,12,6,12,10,12,17,15,17,14,12,15,12,12,17,10,12,15,10,6,6,17,6,14,12,6,12,12,14,15,17,10,12,17,10,12,10,6,6,17,12,12,17,12,10,15,15,14,6,6,15,12,17,14,6,12,12,17,21,10,15,14,6,10,6,6,6,12,12,10,14,10,17,17,6,10,10,17,12,6,12,14,10,12,6,14,6,10,12,10,12,17,6,11,12,12,6,14,10,17,10,17,12,15,14,10,12,6,10,6,10,6,12,10,10,14,11,12,12,12,10,10,15,17,14,17,15,6,15,10,6,14,12,6,14,10,10,12,10,15,12,6,10,10,6,14,10,10,12,17,15,6,10,10,14,14,15,10,17,15,10,14,12,10,14,17,6,17,15,12,15,15,6,15,17,10,6,14,12,6,10,10,10,15,12,10,14,6,6,6,10,6,12,10,17,15,15,12,12,10,12,12,12,10,12,10,15,10,15,10,10,12,10,10,6,12,6,15,14,12,17,10,17,17,17,10,12,12,15,12,10,6,11,12,14,14,11,14,12,15,10,14,12,6,6,17,10,15,10,10,12,10,10,12,15,12,6,10,11,17,15,10,15,10,10,6,14,10,12,14,14,10,10,17,14,10,10,6,17,6,17,15,10,17,14,12,12,10,6,14,17,12,10,6,6,12,10,10,10,10,10,12,17,6,10,12,12,6,17,17,10,10,14,12,14,21,12,10,17,12,12,6,10,14,10,10,17,10,15,15,12,12,6,12,12,14,10,15,10,6,17,15,12,6,12,12,6,14,6,17,15,10,10,11,17,10,10,10,14,17,6,15,15,14,15,10,10,15,11,12,12,6,10,17,14,12,12,6,10,6,10,12,17,10,14,14,6,10,17,12,14,12,17,10,14,10,12,10,17,12,14,12,12,12,12,12,17,12,6,14,10,6,15,14,12,14,15,10,10,12,12,6,14,12,14,10,14,6,14,15,14,6,14,10,17,14,15,12,6,17,6,17,15,10,6,14,17,14,10,17,15,12,6,12,6,12,6,14,12,12,10,10,10,10,14,21,6,15,12,10,15,12,14,12,14,15,10,12,14,12,17,15,12,12,15,12,10,12,6,12,14,15,15,10,17,12,12,12,6,12,10,14,12,17,10,17,10,10,12,17,10,14,12,12,17,15,6,12,14,10,12,12,10,6,6,10,10,12,10,14,12,12,14,10,10,15,12,21,6,6,12,6,10,15,10,14,14,10,10,15,17,10,10,12,6,15,17,10,15,12,12,14,17,14,17,10,6,6,12,12,10,12,17,10,12,12,10,10,12,10,15,14,12,10,17,12,15,10,12,10,10,15,6,15,17,14,15,12,14,15,14,15,10,17,12,10,10,6,6,15,6,14,10,10,10,6,6,12,14,10,14,15,21,12,12,10,12,6,14,15,14,12,14,10,15,15,12,12,17,15,6,10,12,12,17,10,15,10,14,15,6,12,12,21,12,15,10,14,15,15,12,11,10,14,12,10,6,21,17,12,15,14,10,10,14,6,17,10,6,12,10,14,12,10,12,10,10,6,10,12,12,14,14,14,10,15,10,10,17,10,14,15,10,10,14,17,14,15,14,12,6,12,17,6,10,10,12,12,12,10,10,15,6,12,17,6,10,10,17,12,12,14,15,12,10,10,15,14,12,10,15,10,10,12,17,12,14,6,14,12,10,17,17,6,17,17,10,17,12,12,12,6,10,12,12,12,17,14,10,17,14,12,10,6,14,6,12,15,15,10,12,17,14,15,6,10,14,10,17,17,17,15,15,15,12,12,14,10,10,6,12,12,10,15,17,12,17,6,10,17,17,14,12,6,15,14,10,17,14,12,15,10,10,14,12,10,10,10,10,6,14,6,15,6,14,10,14,12,15,14,12,15,6,15,12,10,10,10,14,10,6,10,6,17,12,17,17,12,14,17,14,10,12,17,17,15,6,6,10,11,17,14,14,10,15,6,12,10,10,17,17,10,12,6,14,14,10,14,12,17,14,12,6,6,6,10,12,10,6,12,14,12,14,17,12,21,17,17,17,14,12,12,15,12,6,10,14,12,6,6,10,12,12,12,12,10,17,17,17,10,14,12,10,12,14,12,14,17,15,17,14,12,17,14,10,12,12,10,17,15,12,17,10,12,21,14,6,17,10,10,6,12,12,17,17,10,17,6,10,17,21,17,6,10,10,12,10,12,17,17,6,10,12,10,6,10,14,12,10,14,17,12,11,10,14,10,10,17,6,12,14,12,10,6,17,14,14,6,10,12,6,15,14,12,21,14,6,6,17,12,12,12,10,12,6,14,14,17,10,10,15,12,17,15,10,15,15,10,17,12,15,15,15,12,10,10,11,10,17,14,21,14,17,12,10,6,6,14,14,6,12,12,12,17,6,15,12,15,12,21,17,6,10,6,14,10,17,6,14,15,14,6,10,10,15,6,10,15,14,12,15,14,10,17,6,6,10,15,12,6,14,10,14,15,6,10,10,10,10,10,17,17,6,14,17,10,10,10,14,15,14,12,15,17,6,10,14,10,17,6,12,17,17,10,17,10,10,17,10,10,14,10,15,10,10,6,15,6,10,12,10,12,15,12,10,10,14,14,12,10,12,6,17,12,6,12,17,15,10,6,14,14,17,6,15,10,6,10,10,10,10,10,14,14,15,10,10,14,10,10,10,14,6,10,21,12,15,12,10,14,12,12,15,17,17,17,17,10,10,10,10,15,10,6,17,17,17,11,15,10,12,10,14,11,15,14,10,17,10,10,10,12,10,12,15,6,12,12,15,12,10,12,15,14,10,10,10,14,10,10,10,10,14,12,10,17,6,6,12,14,12,12,17,17,12,15,15,12,15,10,14,17,15,10,17,17,6,17,6,15,10,10,10,15,12,12,12,14,12,6,12,15,17,12,15,12,12,14,6,15,12,10,6,12,14,10,10,10,6,12,17,17,17,17,10,17,17,12,17,12,15,12,12,6,10,10,6,17,14,6,14,14,17,10,14,14,15,10,10,14,15,14,12,15,12,14,6,12,10,6,6,17,6,10,6,17,6,12,10,12,17,10,12,14,14,6,14,6,10,17,12,6,15,14,6,17,15,10,6,10,10,10,6,17,15,15,10,17,12,15,12,10,10,12,10,10,17,15,14,10,17,17,12,15,6,15,15,17,10,15,12,10,10,14,21,15,10,10,10,10,12,6,6,14,14,17,10,12,10,15,14,12,12,10,12,15,17,6,12,17,15,12,10,15,12,14,10,10,14,15,6,10,6,17,10,12,12,17,10,17,10,15,12,10,15,6,15,10,12,12,6,12,12,12,12,6,10,10,15,12,12,17,6,12,17,6,14,12,12,17,10,12,14,12,14,12,15,17,12,17,6,10,6,17,10,14,10,15,17,14,15,6,10,10,10,6,15,12,6,15,10,12,6,15,17,10,15,15,11,10,15,14,10,10,10,12,15,15,17,15,10,6,10,10,12,17,10,10,17,10,10,14,17,12,12,14,17,12,12,17,17,14,10,6,17,12,6,10,12,12,6,15,17,6,6,6,14,10,17,14,21,15,14,10,12,15,15,17,14,14,21,15,10,15,6,12,12,17,5,17,11,13,5,9,11,5,11,11,17,12,13,11,5,12,14,17,12,5,9,null,9,11,11,11,17,9,9,11,11,12,17,11,11,15,15,14,12,15,17,17,11,12,12,15,11,11,14,11,14,14,12,11,11,9,11,5,11,14,9,5,13,14,14,5,15,14,5,5,11,12,12,11,5,12,5,12,15,11,15,11,17,14,5,11,11,14,5,11,13,11,14,15,12,20,12,5,14,11,15,14,14,12,12,20,11,11,11,12,5,11,17,15,11,17,12,11,9,11,14,9,11,14,11,15,12,11,17,12,14,15,11,14,14,14,14,15,17,15,12,12,14,14,20,11,5,11,12,11,5,13,15,12,14,11,15,15,12,5,15,11,15,15,11,5,11,9,11,14,14,11,9,9,5,11,15,15,5,13,14,15,5,5,14,11,11,11,5,5,9,9,12,5,11,11,15,12,15,17,14,11,11,11,11,12,14,15,14,15,11,11,14,5,5,9,14,11,11,12,13,11,11,11,9,5,17,15,11,14,12,14,5,5,14,15,14,12,11,14,15,14,11,13,11,14,14,11,11,9,17,11,11,14,15,13,12,11,12,12,5,17,11,12,12,15,5,11,11,11,17,17,11,12,14,17,5,14,14,5,11,11,11,13,17,9,12,11,14,11,12,14,17,5,12,11,9,11,15,13,11,5,15,9,5,14,12,11,5,11,9,14,11,12,14,5,12,14,12,14,5,5,14,13,11,9,13,11,11,20,14,17,11,11,12,14,14,15,17,5,11,14,14,14,17,12,15,5,12,14,11,14,9,14,11,11,14,11,17,13,12,11,14,17,14,11,11,11,17,11,14,11,5,12,14,11,14,11,17,11,14,14,15,5,17,9,13,11,15,14,13,13,12,15,14,14,11,15,11,5,5,11,13,14,11,17,14,11,11,14,9,12,11,13,14,20,5,12,12,11,12,15,12,11,5,17,5,15,9,9,5,14,12,11,9,14,12,11,11,11,14,11,14,13,11,14,13,14,20,17,15,11,14,14,15,13,11,15,13,13,11,17,11,17,11,12,9,13,15,5,11,14,5,14,14,14,11,17,17,13,5,17,9,5,14,17,11,11,5,11,15,11,17,15,5,9,11,15,9,11,15,11,12,11,14,5,14,11,17,11,17,12,12,9,5,11,15,17,14,11,5,15,11,11,15,9,15,5,15,17,20,5,14,17,11,17,13,12,11,15,5,11,12,14,5,11,12,17,12,14,5,13,15,20,14,14,17,5,5,12,17,11,17,14,13,15,12,5,11,14,5,11,9,14,11,12,12,11,12,14,11,9,13,17,11,20,12,12,5,5,13,11,5,15,17,5,9,14,14,14,14,11,12,17,17,12,11,13,14,17,11,14,15,20,5,11,11,11,14,17,11,9,11,11,11,15,5,12,14,14,13,15,11,11,11,11,12,17,14,5,11,11,5,11,17,14,9,17,12,14,11,11,14,11,15,14,12,17,11,15,12,14,13,11,9,12,11,17,12,12,5,17,5,13,9,14,5,11,14,11,5,5,14,11,5,9,20,11,11,17,11,11,15,5,17,12,5,12,5,12,15,17,15,15,12,11,5,11,12,12,20,17,12,14,14,12,11,11,17,11,9,17,11,11,11,5,15,14,15,11,9,5,14,14,5,14,5,11,5,9,14,11,11,12,11,14,14,17,12,9,5,17,14,9,12,17,14,11,11,13,5,15,11,15,14,17,11,13,17,15,12,14,11,15,14,5,14,12,14,11,11,12,14,11,11,13,11,14,14,17,12,15,5,11,11,11,11,9,5,11,14,14,11,17,11,15,11,12,11,15,12,9,12,11,14,11,15,12,11,15,11,9,9,11,15,14,9,9,13,15,17,5,9,11,12,5,12,9,11,12,5,9,9,11,11,11,15,13,15,15,11,5,5,5,14,12,14,12,12,11,11,11,11,11,17,14,13,11,9,5,9,5,14,9,14,5,11,5,5,11,11,17,5,17,20,17,5,14,11,5,11,11,11,17,14,12,17,11,5,14,13,5,5,15,11,11,5,12,11,14,13,17,9,14,12,5,12,11,14,11,15,5,9,11,11,15,14,11,12,13,14,9,11,9,11,11,17,13,11,5,11,17,12,13,17,11,17,11,11,17,14,5,11,15,14,14,5,11,5,14,11,9,15,5,15,14,14,17,17,5,14,11,12,17,5,14,12,14,15,14,17,5,14,14,14,9,14,11,17,15,17,11,11,13,11,14,11,14,11,11,11,12,5,11,11,11,12,14,11,12,5,11,14,5,11,14,14,17,17,14,11,11,5,11,17,9,13,11,5,13,15,11,11,11,9,17,5,9,11,14,11,11,14,9,13,17,12,12,15,14,5,14,5,17,12,12,12,11,11,17,11,11,12,15,null,14,14,9,5,11,null,11,14,14,11,14,12,15,13,14,15,17,11,11,11,14,14,11,11,5,14,17,9,17,12,17,15,14,11,11,11,5,14,15,12,5,11,5,5,12,13,11,11,11,11,15,12,14,14,14,17,12,14,5,11,14,15,13,14,11,17,12,5,9,5,17,12,12,11,17,12,14,12,15,11,5,11,11,14,14,13,17,14,14,5,14,11,15,5,14,11,11,15,17,14,14,13,11,9,14,11,17,11,12,17,11,14,11,12,11,5,14,5,14,5,15,17,15,14,15,5,14,13,12,11,9,17,11,15,11,14,11,15,11,12,14,11,5,12,14,12,11,15,15,15,17,9,17,5,14,5,11,11,11,17,13,11,17,null,11,17,12,11,9,12,12,20,15,11,11,9,13,9,14,17,15,11,11,14,11,11,5,5,11,5,11,11,13,11,5,15,14,11,5,17,11,14,17,14,11,11,14,14,12,null,14,5,15,9,5,11,14,15,14,12,14,12,12,15,11,14,17,5,11,14,5,5,12,11,15,15,15,11,11,15,15,5,14,5,17,9,13,15,11,15,11,15,5,14,14,5,14,14,15,15,5,14,5,14,5,14,13,12,14,12,15,14,5,12,9,9,15,11,11,11,12,11,12,12,15,17,5,13,11,12,5,14,11,11,5,14,9,11,11,11,11,12,14,5,5,14,17,15,5,17,11,11,5,11,13,5,14,17,14,14,12,11,11,15,17,17,11,11,5,5,17,9,11,12,14,12,11,17,17,5,11,14,15,12,15,9,5,12,14,14,11,11,14,14,11,11,17,17,14,15,14,11,17,14,5,15,5,13,13,11,11,11,13,9,9,14,14,14,11,17,14,12,15,11,11,17,11,12,9,15,12,11,17,11,17,14,5,12,11,12,12,11,9,13,14,11,5,14,11,14,5,5,11,11,9,11,11,12,12,5,12,17,14,5,14,14,11,12,12,11,9,11,5,9,13,14,12,17,5,14,5,12,14,13,15,5,17,14,11,11,9,14,12,11,13,15,17,12,11,11,14,11,14,9,17,5,13,11,9,14,17,13,11,13,14,11,14,14,17,15,12,11,14,11,11,9,11,5,9,11,17,11,14,14,11,17,5,12,17,11,11,15,17,13,17,15,5,14,14,14,17,17,13,14,11,14,11,14,14,5,17,12,5,5,11,15,11,15,9,13,12,14,15,15,11,14,11,15,12,11,17,13,12,15,11,17,9,11,14,12,11,14,9,14,5,5,12,13,9,5,12,5,5,14,13,14,17,12,5,14,17,5,15,15,11,14,12,5,5,11,12,11,11,5,11,15,12,11,12,5,5,null,11,14,17,14,13,14,13,15,11,12,17,11,11,5,12,null,13,11,11,5,5,17,9,9,5,15,12,12,14,11,5,5,14,11,15,15,11,12,20,12,11,9,11,14,13,12,14,11,5,11,15,11,15,14,15,14,15,11,11,5,11,11,9,9,5,5,11,17,12,11,14,14,9,11,11,11,12,14,11,5,20,14,11,12,14,9,5,11,12,14,5,15,5,14,14,12,15,14,5,14,13,11,9,11,12,5,15,14,11,13,14,17,11,12,11,14,12,14,14,15,15,14,12,11,12,11,11,13,11,17,14,20,11,14,11,11,14,15,15,11,14,15,12,11,12,15,17,11,14,15,13,5,12,12,11,15,9,12,15,14,11,11,14,12,15,11,14,13,13,5,11,5,12,5,5,5,11,5,14,12,13,14,14,12,13,15,20,12,12,15,11,11,9,5,11,11,17,11,17,17,11,11,11,5,11,12,9,12,5,15,14,11,12,11,5,11,5,13,12,14,11,5,15,11,14,5,17,11,14,12,11,14,11,12,17,14,11,13,5,13,5,5,12,5,12,11,11,12,17,17,15,20,15,14,5,12,9,12,11,17,14,17,12,11,15,14,12,12,11,15,13,12,12,11,15,5,13,15,11,11,15,12,11,14,12,5,14,15,11,14,11,11,9,11,5,12,5,17,11,17,14,17,17,5,11,14,11,5,20,11,15,14,12,11,12,9,14,15,15,5,5,14,11,5,14,15,14,11,14,11,15,11,9,14,11,14,11,11,5,13,11,11,11,5,15,11,17,null,12,13,13,15,11,14,17,11,11,9,14,11,5,20,17,14,11,15,12,14,17,14,5,9,17,11,15,14,5,14,11,14,11,12,11,14,11,11,11,15,14,9,11,12,9,12,15,11,14,5,17,14,11,14,11,15,13,14,11,15,15,12,17,13,5,9,11,14,14,14,11,15,5,5,14,17,5,17,13,5,11,5,11,11,20,14,14,17,11,11,15,11,12,17,5,17,11,14,13,5,9,14,15,14,14,11,14,12,15,17,12,5,11,15,11,17,5,11,14,17,11,11,5,17,11,12,12,15,11,11,5,9,11,11,5,17,11,15,13,12,15,12,11,13,5,15,17,17,20,14,17,15,11,9,5,11,14,11,14,15,12,11,15,11,9,14,14,12,12,12,14,11,14,14,12,14,9,9,15,5,11,14,17,15,9,5,12,9,11,12,15,11,9,14,15,11,11,12,11,12,12,11,5,11,5,13,14,14,12,14,11,15,11,11,11,5,14,17,11,11,14,5,15,11,14,11,15,13,5,14,5,5,11,15,11,15,14,13,17,5,5,11,11,13,15,5,12,14,15,17,17,14,15,20,11,12,11,17,17,15,11,11,5,5,11,14,11,15,15,5,14,5,13,12,13,5,14,12,11,11,12,11,13,17,15,12,11,14,12,5,15,5,17,9,14,14,11,9,13,15,11,5,14,11,11,11,17,12,14,17,12,13,12,12,11,11,5,14,9,13,12,5,5,12,17,14,17,11,12,15,17,13,14,15,17,13,11,15,17,11,15,11,15,15,14,17,15,13,12,14,11,14,11,14,11,11,14,15,13,14,11,14,14,15,11,5,14,14,11,5,14,12,15,14,12,9,12,14,14,15,5,5,14,13,12,15,11,14,14,9,17,14,12,14,17,5,13,5,14,15,5,11,11,12,15,9,11,11,13,15,15,11,5,11,9,13,13,13,15,12,11,17,11,12,11,14,9,5,5,9,15,14,11,15,11,5,14,5,5,11,17,5,11,13,12,14,12,17,11,14,17,17,5,17,15,11,11,14,13,14,11,11,17,11,13,17,14,14,12,11,15,14,9,15,12,5,11,11,12,15,9,15,12,5,14,11,13,12,13,11,12,17,17,17,14,15,11,14,17,17,5,5,11,15,14,5,15,17,13,11,5,11,13,17,15,9,12,17,11,14,14,5,17,11,13,12,12,12,15,11,14,9,11,15,11,15,13,11,11,12,14,11,14,11,11,14,15,13,11,13,11,11,11,12,17,14,15,9,14,9,11,14,5,14,5,11,11,12,11,9,14,14,13,12,11,5,11,14,14,12,14,11,12,11,14,14,14,11,11,14,17,11,14,11,14,17,14,12,9,11,9,15,11,14,14,14,5,14,9,14,14,11,20,15,11,17,11,14,11,12,11,5,9,9,12,15,17,12,5,17,14,13,17,11,15,11,12,15,11,5,5,5,12,12,14,11,11,12,14,12,17,15,17,11,14,5,5,5,15,12,15,11,14,5,17,17,11,null,11,12,11,12,12,11,11,11,12,17,11,14,17,15,12,11,12,5,12,11,11,14,9,15,11,14,12,11,15,14,14,12,13,5,5,12,13,12,14,11,15,17,12,15,17,11,11,13,14,11,14,15,15,14,9,14,12,5,11,5,12,15,14,13,17,13,13,9,14,5,5,14,13,15,11,17,11,12,5,11,12,11,17,5,14,14,5,5,11,14,15,9,15,11,14,11,5,11,12,15,14,11,11,11,5,9,14,11,13,13,null,9,14,11,14,13,14,5,11,14,12,9,11,15,12,5,13,14,14,5,11,5,5,14,11,14,14,15,11,11,14,11,11,11,14,11,17,11,11,11,14,11,17,14,13,17,13,11,15,20,11,15,15,12,9,20,17,5,15,15,15,9,14,11,11,11,15,11,13,11,14,9,14,12,13,11,15,11,13,14,12,14,17,15,15,11,12,15,11,11,20,14,17,5,11,17,17,11,13,11,14,14,12,9,12,11,5,13,14,15,9,15,13,14,15,12,11,11,15,15,5,11,12,11,17,11,15,5,11,11,11,12,14,14,5,5,14,12,11,12,11,12,12,9,15,15,15,15,12,13,13,12,11,17,14,14,9,9,17,5,14,11,17,13,11,5,11,13,11,5,11,12,14,11,11,11,15,14,5,15,15,11,20,15,11,15,11,15,13,15,12,12,9,11,14,11,5,12,5,15,17,12,14,15,15,5,5,12,11,15,12,13,14,14,17,14,11,11,20,17,17,9,5,11,20,17,11,14,15,12,5,12,5,11,14,14,17,11,13,11,5,5,5,12,15,11,17,14,9,9,14,14,15,5,17,11,14,17,17,11,11,14,17,17,15,5,9,17,11,17,9,5,14,11,11,14,12,9,11,14,17,15,15,12,5,15,13,9,15,5,13,12,11,9,17,5,14,17,17,15,14,15,11,13,20,11,11,15,11,14,12,12,17,11,5,11,5,5,15,11,9,15,14,14,13,17,5,13,5,13,5,12,11,11,11,15,15,13,5,13,11,13,14,12,17,11,5,14,11,14,14,11,5,14,5,9,17,20,11,14,9,11,14,17,14,15,17,11,12,14,11,11,5,14,15,14,12,17,11,12,14,14,17,14,14,11,12,17,17,11,5,17,17,11,17,5,11,15,15,14,17,14,15,15,15,5,14,14,11,11,12,11,14,15,12,11,5,15,5,14,14,11,13,11,11,5,11,12,5,9,5,15,5,11,15,12,11,14,12,12,14,15,17,11,14,17,11,20,5,14,13,12,17,14,12,5,17,12,12,5,17,14,11,5,11,11,14,13,15,17,11,11,11,11,5,11,12,5,12,11,15,11,13,5,14,5,11,11,12,12,11,5,14,15,15,11,11,15,17,11,14,17,13,11,5,11,9,11,5,11,5,11,11,20,11,9,17,11,12,17,11,15,11,13,11,17,13,11,11,14,12,11,14,11,15,14,17,11,12,14,17,12,5,12,5,11,9,9,11,14,5,12,17,14,15,12,12,5,14,15,12,5,14,16,16,11,16,null,13,16,11,null,11,15,null,16,11,11,11,16,16,11,16,11,11,11,null,16,11,16,15,15,15,13,16,16,16,11,13,16,16,16,11,13,13,11,11,16,13,11,16,13,16,11,15,11,13,16,11,12,11,11,16,11,16,11,15,16,11,null,11,13,16,16,16,16,11,null,11,13,11,12,13,11,11,16,16,11,11,16,11,11,16,11,11,16,11,11,16,16,11,13,16,null,11,16,11,11,11,null,null,16,11,16,11,16,11,15,11,11,16,11,16,11,11,11,13,13,11,11,16,11,11,16,11,11,11,12,16,11,16,16,11,11,16,16,15,11,13,11,16,11,11,11,15,11,16,11,16,11,null,16,11,11,13,11,11,16,16,16,16,11,11,16,11,11,16,11,16,16,null,16,11,16,16,16,11,16,11,11,16,12,16,11,16,11,13,11,16,15,15,16,11,16,11,16,11,11,11,13,null,11,null,16,11,11,11,15,16,11,16,11,16,16,15,11,13,15,11,11,16,11,16,15,11,11,16,11,11,15,16,11,16,16,11,11,16,null,16,16,16,16,11,16,11,null,16,null,null,16,13,15,16,15,13,16,16,11,16,16,16,13,13,11,15,16,13,16,11,11,11,11,11,11,11,16,11,15,13,16,16,11,16,11,null,13,11,15,11,11,16,16,11,16,11,11,11,11,11,11,16,16,15,16,16,16,11,16,13,11,16,15,11,11,11,16,16,16,15,11,11,11,16,11,16,null,11,null,11,11,11,11,16,16,11,11,13,16,15,11,16,null,11,11,null,16,11,null,13,11,16,11,13,11,11,11,11,11,16,11,11,15,11,16,16,null,11,16,11,16,13,16,13,11,11,null,11,16,11,15,15,11,11,16,null,11,11,11,11,16,16,16,11,11,16,16,16,11,11,11,11,null,13,11,13,null,11,11,11,11,11,16,11,16,11,11,16,16,16,16,15,16,16,13,16,11,11,11,16,13,16,11,11,16,16,16,16,13,16,11,11,16,11,11,null,15,13,11,16,16,13,16,16,16,16,16,13,11,11,11,11,11,11,11,16,11,16,16,13,11,11,11,16,16,13,16,16,11,13,11,16,16,15,16,11,null,15,11,11,11,11,16,11,16,null,16,15,15,11,null,11,15,16,11,11,13,16,null,11,16,16,16,16,16,null,16,11,11,16,11,11,16,null,16,null,11,11,16,16,15,13,16,11,15,11,11,11,16,11,16,11,16,11,11,11,null,16,16,null,11,16,11,12,11,11,11,15,16,11,null,15,16,16,11,11,11,null,16,11,16,11,16,11,11,16,11,11,11,16,11,13,13,11,16,16,11,11,11,null,16,11,13,13,13,13,15,11,16,15,11,11,15,11,16,16,13,11,11,null,null,16,11,13,11,11,16,16,11,16,11,11,11,16,16,15,11,null,11,16,13,13,16,11,16,11,15,16,11,11,15,16,16,11,16,16,null,11,16,11,13,12,16,15,11,16,11,13,16,15,13,11,16,13,11,null,11,13,11,16,11,13,null,13,11,11,16,11,16,null,11,11,16,16,11,16,11,16,16,16,11,15,11,15,11,11,11,11,11,16,11,15,16,11,16,13,16,16,11,11,11,16,11,13,16,15,11,11,11,16,16,11,11,null,11,11,16,16,16,16,16,11,16,16,11,null,15,15,11,13,15,16,11,16,16,13,16,11,15,16,11,11,16,null,16,11,16,16,11,16,null,13,16,16,11,16,null,13,11,16,16,13,11,11,16,11,16,11,11,11,16,11,15,13,11,15,11,11,16,11,11,11,11,11,11,16,16,15,16,16,16,11,11,16,15,11,13,13,13,16,null,16,11,16,16,11,11,15,16,16,null,15,11,16,11,16,11,11,11,null,16,16,11,15,11,11,11,13,16,11,11,11,11,16,13,13,16,16,16,11,15,11,null,11,16,11,11,16,11,15,11,11,null,16,15,null,16,11,15,16,11,11,11,16,16,11,15,16,15,11,16,16,null,15,11,11,16,11,16,16,16,11,11,15,15,16,16,16,11,16,13,13,11,16,15,16,11,11,13,16,11,16,11,16,11,11,11,11,11,11,11,16,16,11,11,13,15,11,11,16,11,16,11,13,16,16,11,16,11,15,16,11,11,11,16,11,11,11,16,16,16,13,11,11,11,11,null,11,15,13,null,16,11,11,16,11,11,11,15,16,null,11,null,15,11,16,16,16,11,11,16,11,11,13,11,16,11,15,11,null,16,11,11,15,16,16,11,11,11,11,16,16,16,11,11,16,11,11,16,11,13,11,11,15,15,16,11,11,16,11,16,16,11,null,11,11,16,13,11,13,11,11,16,11,11,11,16,11,null,11,null,15,16,16,11,11,11,11,11,16,13,16,11,11,16,11,16,11,11,null,11,11,16,11,11,13,13,16,null,11,13,8,11,13,8,8,13,13,8,13,13,18,13,9,11,18,13,11,13,8,18,8,8,13,8,18,13,13,13,18,8,11,13,13,18,11,8,9,18,11,13,19,13,13,8,13,8,11,13,18,11,13,13,8,13,13,18,8,13,13,8,13,13,16,18,18,5,8,13,18,18,13,13,18,8,8,18,18,13,13,8,18,13,13,13,19,13,13,5,18,13,13,13,11,8,18,8,18,13,11,13,13,8,11,13,18,13,18,13,8,13,8,13,13,13,8,11,13,8,13,13,18,13,8,13,11,13,8,13,11,18,13,5,13,13,8,13,16,19,18,13,5,13,8,13,13,13,19,11,8,8,8,13,11,15,13,18,13,18,13,11,13,13,9,8,8,11,13,13,8,13,13,8,8,13,18,18,13,13,13,5,8,8,18,13,8,18,13,13,8,13,8,8,8,13,8,11,13,8,5,18,8,11,8,13,13,9,8,18,8,13,8,18,11,8,13,8,8,18,13,18,18,18,8,11,11,13,13,13,8,8,13,18,8,13,13,19,13,5,13,13,13,8,11,13,13,8,13,13,18,13,13,13,18,11,8,8,13,13,13,8,13,13,8,13,11,18,11,18,18,13,8,13,18,18,11,13,18,16,13,13,8,8,13,8,8,11,19,18,13,11,13,13,18,13,13,13,8,11,8,11,8,13,8,13,18,8,13,13,13,8,18,11,13,13,8,18,18,8,13,13,13,8,5,8,18,8,11,8,13,11,18,18,13,13,18,18,11,8,5,8,13,13,13,18,13,21,13,13,13,11,19,8,18,13,18,15,13,13,18,13,13,13,8,11,5,18,13,11,13,21,8,13,9,13,13,18,18,13,13,8,13,13,11,8,8,13,13,13,18,18,5,13,18,8,13,8,11,18,11,13,8,13,13,11,13,8,8,13,13,8,13,8,13,8,18,11,13,13,13,13,13,18,13,11,18,13,18,13,18,18,8,13,18,13,8,13,8,18,5,13,13,8,11,5,19,8,18,13,13,13,13,8,8,13,18,11,18,18,8,13,18,11,18,13,11,19,18,8,13,18,11,8,18,13,8,13,13,13,11,5,13,13,13,13,13,8,18,8,13,8,13,8,18,18,13,8,13,8,15,15,13,13,19,8,18,13,13,13,8,8,11,5,8,11,8,8,18,13,11,13,13,18,9,8,9,8,9,8,11,8,18,13,13,18,18,18,8,13,18,13,13,11,18,11,13,13,18,13,13,18,13,13,18,13,13,13,18,13,18,13,18,13,11,9,13,18,18,13,13,13,8,13,8,11,19,13,13,13,13,8,13,13,13,13,18,8,8,8,8,13,13,18,13,8,13,13,9,13,8,9,13,8,18,8,18,13,11,13,13,13,11,18,8,18,8,8,11,13,13,13,13,13,11,8,19,11,5,8,9,13,11,13,13,15,18,13,13,11,11,13,18,18,13,18,18,13,13,18,11,8,18,8,11,9,13,8,8,18,13,18,13,8,13,8,5,13,9,13,8,18,18,19,8,13,13,13,11,13,5,13,8,13,13,5,8,13,8,13,8,15,13,13,13,8,5,11,13,13,8,13,11,13,18,8,13,18,13,13,13,13,13,13,13,13,13,18,11,13,18,5,18,18,18,13,11,8,11,8,18,13,9,8,13,18,15,18,18,13,8,13,13,18,13,8,13,18,8,13,8,11,18,13,13,18,13,8,5,13,8,13,13,8,11,13,11,19,8,13,13,5,13,18,13,13,9,15,13,8,8,8,8,18,8,11,13,21,13,8,11,13,8,8,18,11,5,13,8,13,8,13,13,18,11,13,13,13,11,8,13,13,11,5,8,13,8,13,18,11,8,11,18,13,8,5,13,13,15,13,13,18,8,19,13,19,18,13,13,8,13,13,13,5,13,13,11,11,13,18,8,18,8,13,9,18,19,13,8,11,18,15,13,8,8,8,18,13,11,13,8,8,8,13,8,13,8,13,13,11,13,18,18,13,18,8,5,18,8,13,13,13,11,18,11,8,13,13,13,5,9,8,13,8,13,18,18,13,8,21,13,9,18,18,13,13,18,13,16,18,5,11,13,11,18,11,13,11,13,8,13,8,8,8,8,13,9,11,13,8,13,11,13,11,11,13,18,21,8,18,11,13,13,18,13,8,13,18,13,18,8,8,13,18,18,13,13,13,18,13,18,11,8,8,13,13,8,13,13,18,8,11,19,13,18,18,11,8,11,13,18,8,11,11,9,15,8,13,9,18,19,13,19,13,13,11,13,18,8,5,18,13,13,18,8,11,18,13,13,18,8,13,13,13,11,19,13,13,13,11,13,18,18,13,8,13,13,18,8,18,13,13,13,8,15,8,18,11,13,13,13,5,13,13,5,13,11,5,8,13,8,13,18,18,13,15,18,16,18,13,11,18,13,13,13,13,8,11,18,8,19,11,13,13,11,8,11,5,13,8,13,21,13,8,13,13,18,13,8,13,8,13,13,13,18,13,13,13,13,8,13,11,18,13,11,13,8,13,8,18,8,8,8,18,15,18,13,15,13,11,18,8,19,18,13,13,11,13,18,11,13,13,13,13,13,13,13,8,13,8,8,8,15,8,8,9,8,8,8,13,11,8,8,8,18,8,13,5,18,11,13,13,8,18,8,8,8,13,11,11,8,18,13,18,5,11,18,11,11,13,8,8,13,13,8,18,13,8,13,13,8,13,13,13,13,8,13,18,18,18,13,8,18,8,13,5,9,8,11,8,11,13,13,18,8,8,5,18,18,18,18,5,13,11,13,5,13,8,13,18,13,11,13,18,15,15,18,13,11,13,18,8,11,8,18,18,13,11,13,13,13,13,13,19,18,13,8,18,18,13,19,8,13,13,8,11,13,13,8,13,8,18,8,13,13,8,13,13,13,13,13,13,13,13,13,8,13,11,18,18,13,8,11,8,18,13,13,13,13,18,13,13,13,9,13,18,11,13,13,13,8,18,13,13,18,8,13,8,8,13,11,13,13,13,8,8,13,13,13,13,13,8,13,11,13,13,13,13,13,8,8,18,8,11,13,13,13,13,8,11,9,13,8,5,13,8,11,19,9,8,9,13,13,13,18,8,13,21,8,13,13,13,13,11,18,18,13,11,13,13,18,8,18,18,8,9,13,8,13,18,13,8,8,13,13,13,8,18,8,11,8,13,18,13,8,13,11,19,8,11,8,8,15,13,13,13,18,13,11,13,19,13,13,13,8,8,18,13,18,13,9,18,8,13,8,13,13,13,13,8,21,13,8,13,18,8,15,18,18,13,8,18,13,8,8,8,13,18,5,8,18,8,18,11,18,13,8,13,5,8,5,5,13,11,8,19,8,13,13,18,13,13,13,13,8,18,13,13,13,13,11,13,11,13,8,13,13,18,8,13,13,13,11,13,8,18,8,18,8,18,18,13,13,11,13,8,18,8,8,18,18,8,13,8,8,18,18,13,18,13,13,13,13,13,11,5,9,13,13,13,8,13,13,8,18,8,13,13,8,13,13,18,13,8,11,5,18,11,18,13,18,13,8,13,13,8,8,18,13,13,13,13,13,13,8,13,8,8,18,11,13,19,13,13,18,8,18,18,11,18,15,18,13,11,5,8,18,8,18,11],"Experience_years":[26,1,32,21,5,20,32,0,7,2,20,15,20,23,37,8,1,3,16,30,9,28,12,20,20,12,10,12,16,31,14,22,12,10,6,1,20,14,20,15,6,47,13,17,8,12,36,30,26,21,33,16,25,6,33,18,36,17,5,10,3,18,9,1,3,5,10,19,35,20,27,8,40,22,15,12,36,30,2,12,1,12,20,5,7,34,15,30,15,0,17,3,7,22,14,7,0,40,35,12,28,7,25,12,15,33,18,18,10,15,20,44,3,9,41,35,18,4,21,23,18,41,37,13,24,22,35,38,44,29,8,25,8,32,5,3,3,8,40,2,19,35,15,41,23,17,12,2,22,24,28,5,15,13,3,8,24,2,39,5,40,41,12,12,7,17,29,12,3,11,35,20,15,38,8,12,19,17,4,6,39,8,27,17,39,17,16,11,41,0,24,25,7,10,12,6,25,21,35,15,4,35,5,22,13,16,9,10,13,14,14,19,13,21,1,40,5,41,30,5,25,8,13,2,20,19,22,15,8,24,8,11,17,22,6,23,11,22,19,1,15,29,26,25,1,10,4,13,12,20,8,16,15,12,7,21,18,10,44,37,23,19,4,37,27,30,13,2,11,15,31,6,25,4,40,19,47,9,1,8,5,10,34,15,6,21,27,10,21,10,30,19,7,7,27,8,8,31,24,10,30,24,19,18,14,4,40,22,9,28,3,1,18,2,22,6,1,23,6,6,30,38,3,21,16,24,31,15,4,7,16,12,22,13,10,16,17,4,11,11,20,10,24,7,4,14,30,3,30,21,7,15,38,4,3,40,16,10,27,12,22,14,2,25,28,18,18,16,22,4,9,20,24,16,20,1,19,15,2,10,6,39,38,2,4,11,18,19,16,2,23,3,15,47,7,4,9,7,15,12,18,13,15,19,13,21,20,16,4,20,15,15,15,42,4,33,30,21,7,9,10,47,8,12,25,5,37,2,23,5,8,30,3,17,19,6,6,9,27,13,16,8,21,10,23,11,4,39,14,16,8,35,14,24,9,14,7,23,25,45,28,32,21,16,35,10,10,25,16,23,2,24,47,34,25,null,30,40,9,12,33,34,21,4,15,19,8,20,25,4,16,9,20,16,16,12,15,16,10,15,6,3,25,13,24,40,14,6,26,3,26,15,9,12,7,24,8,37,15,37,20,29,30,24,17,10,20,12,24,15,14,23,32,22,2,21,47,28,12,12,36,14,7,27,26,23,40,10,38,4,22,34,23,11,23,40,30,26,3,14,5,10,46,23,7,7,31,28,22,13,24,10,36,15,20,5,9,19,3,24,16,38,35,35,20,20,15,3,19,6,36,13,27,43,15,6,18,3,28,27,35,12,9,33,19,33,9,32,10,47,24,30,42,22,20,17,12,13,21,20,15,1,35,8,32,25,25,31,11,0,3,14,6,2,1,8,20,25,20,5,12,30,10,25,11,12,3,8,11,47,4,22,20,35,9,8,10,1,37,14,4,25,1,6,17,10,4,28,3,12,15,29,11,5,8,3,21,14,25,2,15,4,13,10,25,14,10,27,20,13,35,6,10,15,42,36,3,11,26,0,8,2,13,36,27,20,22,27,15,10,36,24,5,6,10,6,2,16,24,14,37,31,10,9,20,10,17,5,1,12,8,16,13,0,6,21,26,10,7,13,9,6,6,1,15,2,20,15,5,24,37,26,8,13,18,31,9,12,19,19,13,4,5,21,18,30,12,6,14,3,0,18,22,34,28,10,3,14,5,12,20,12,16,34,22,3,25,22,16,7,2,10,25,39,5,18,9,46,12,10,41,15,24,3,35,4,19,22,12,20,12,30,10,22,29,30,12,5,5,2,9,26,10,24,19,16,5,4,7,17,33,21,21,10,1,36,30,40,2,9,14,23,19,21,16,1,8,28,8,47,20,22,15,40,19,35,22,40,25,7,21,0,10,14,22,15,12,25,24,20,10,8,12,1,6,38,20,11,8,40,30,15,1,20,3,22,8,11,8,0,4,12,15,33,5,24,6,42,6,5,4,5,6,30,7,22,18,6,13,21,8,13,0,21,28,3,40,13,3,38,30,18,22,4,17,30,3,8,29,10,37,45,42,10,20,16,13,6,14,17,18,17,2,5,29,16,20,13,14,13,4,25,8,11,13,20,25,13,9,16,21,25,13,22,27,16,7,4,5,23,5,35,13,24,14,12,9,6,27,10,20,3,25,35,6,22,27,22,1,20,17,4,17,7,12,25,10,24,30,18,29,13,24,22,16,35,24,5,22,35,6,8,13,20,23,29,1,10,19,4,3,14,13,20,18,21,25,13,14,7,2,28,17,27,9,null,6,23,22,23,35,32,35,33,10,10,22,14,4,7,40,3,6,36,27,29,12,15,27,47,9,12,4,2,12,36,24,25,23,7,16,3,4,38,10,6,20,8,15,10,5,26,7,1,16,10,16,17,8,2,25,32,21,17,4,15,8,5,13,28,3,31,0,42,20,1,26,21,20,5,14,36,21,28,17,35,19,29,1,4,6,15,28,21,12,20,4,19,34,40,40,39,28,10,14,5,3,8,35,14,13,26,30,42,20,18,41,23,26,5,20,15,16,33,30,3,17,6,24,3,35,32,17,2,24,3,16,6,36,2,35,7,8,5,5,13,37,8,10,20,10,12,23,33,14,12,15,38,9,4,2,6,35,45,27,10,12,1,2,15,20,20,14,8,3,0,13,18,18,10,0,5,30,0,13,22,5,4,2,34,8,18,23,28,40,0,7,11,29,30,5,23,1,9,21,40,6,10,36,32,25,11,14,28,25,15,34,18,10,35,15,16,7,1,19,24,4,28,30,15,14,24,2,31,30,30,43,30,20,33,10,17,40,8,25,11,40,12,2,33,13,25,30,21,35,14,41,35,24,29,30,4,30,29,1,21,5,18,10,11,12,19,38,34,25,30,12,38,7,24,7,37,24,34,7,18,9,7,8,11,3,3,11,15,15,8,4,21,7,10,7,30,18,16,20,11,21,10,23,1,30,20,6,20,5,11,16,7,23,37,12,11,5,30,10,35,4,30,23,19,5,2,17,27,13,40,1,27,34,15,2,25,10,26,21,37,3,5,1,4,28,23,20,3,6,4,5,5,4,25,18,25,15,16,20,33,11,12,20,39,18,15,6,46,10,17,17,15,19,7,39,9,9,13,31,26,12,4,4,23,11,36,30,30,42,37,9,36,14,15,10,30,20,14,10,20,33,4,1,5,15,16,25,12,11,31,14,15,34,13,9,23,38,45,18,33,23,20,27,5,7,13,6,6,14,2,20,11,20,2,30,14,19,15,27,12,4,16,30,28,4,7,21,12,8,10,7,0,30,33,14,42,42,25,11,35,25,20,0,1,7,8,20,27,22,25,10,24,20,35,40,11,13,26,12,4,22,23,17,18,7,7,20,17,7,18,7,21,35,5,16,32,46,9,20,11,17,6,40,13,29,3,34,26,2,25,5,22,9,20,16,26,3,8,8,24,27,20,5,7,0,11,3,10,10,27,2,6,13,14,9,12,10,10,30,5,4,11,16,0,14,14,7,29,21,17,35,35,24,12,28,8,4,8,10,33,9,10,11,18,11,15,21,23,9,22,35,18,17,10,6,30,13,21,10,4,24,25,23,5,7,8,21,5,11,5,18,5,19,22,7,10,13,16,17,20,13,16,30,42,13,19,39,10,30,25,7,16,8,3,6,9,15,1,21,10,22,7,2,27,23,22,45,27,26,23,2,36,18,11,23,2,10,35,28,47,5,29,9,5,15,23,12,7,17,15,0,35,38,15,16,1,27,16,10,37,31,12,10,12,11,14,23,20,22,12,17,5,8,27,14,30,9,16,9,11,19,39,2,43,22,40,1,16,30,30,12,15,3,13,34,3,5,17,5,24,37,13,9,25,15,20,19,16,14,11,34,30,3,9,35,14,3,26,16,10,23,16,15,13,23,19,16,30,22,6,28,30,4,25,12,26,15,15,35,23,22,20,14,10,19,5,15,9,22,22,4,9,0,9,11,10,25,32,14,22,10,24,15,7,10,1,31,16,30,5,29,0,18,1,13,8,20,16,4,28,24,11,1,10,10,41,33,22,2,10,24,6,8,35,15,34,7,4,22,35,10,12,11,15,24,25,22,21,20,20,5,36,27,36,19,16,12,25,26,15,7,30,4,9,8,13,13,3,2,30,13,20,20,26,2,5,6,5,23,11,5,18,12,11,30,13,24,6,13,11,28,25,23,20,17,15,5,31,36,13,1,8,32,19,2,23,13,0,25,28,20,19,17,16,3,20,32,18,14,20,7,12,37,35,19,22,16,25,32,4,10,7,14,15,1,32,17,42,18,9,15,19,34,5,11,21,30,7,8,12,28,21,17,9,9,30,17,15,3,30,20,21,2,24,12,25,1,19,12,14,13,15,20,12,14,12,3,18,18,15,3,6,22,25,15,20,30,6,9,9,11,25,20,4,22,39,26,40,12,32,36,32,2,17,36,13,11,4,37,26,11,24,1,31,23,6,22,31,26,5,null,11,30,30,5,16,25,5,28,21,2,38,7,15,15,31,11,35,1,26,1,23,30,30,36,23,20,13,15,29,30,32,28,41,9,6,36,1,3,17,38,6,15,10,1,40,15,27,45,13,28,15,18,9,3,1,3,25,31,38,14,13,13,26,13,37,7,1,33,23,11,23,20,14,20,6,7,28,7,12,28,13,9,23,35,40,32,11,14,30,43,15,34,32,15,37,5,37,33,16,22,30,12,10,29,27,15,23,11,10,10,19,4,12,15,18,15,4,16,7,30,2,1,32,25,25,21,17,2,17,39,17,14,15,6,10,19,3,16,25,29,24,37,32,31,37,24,36,15,23,40,3,26,16,1,15,12,12,40,12,20,36,30,7,12,8,32,7,13,10,32,29,17,25,29,0,1,30,40,10,8,30,6,10,30,26,5,15,24,22,7,7,25,28,14,9,41,16,33,25,8,3,33,37,15,2,20,32,1,15,23,37,12,1,38,23,5,29,27,1,15,14,23,19,29,4,34,39,20,5,33,4,40,11,8,9,14,22,5,26,27,5,9,0,3,7,4,43,37,25,12,30,17,1,13,36,41,33,19,13,31,0,34,2,12,23,3,10,14,4,21,15,7,34,10,19,36,5,38,29,14,2,14,33,35,2,15,7,39,10,9,28,24,3,9,null,34,15,12,27,33,13,17,14,5,22,2,41,15,19,31,22,5,20,5,5,12,24,12,30,35,14,14,14,38,25,34,20,3,15,16,7,11,7,12,35,15,4,10,4,30,11,30,7,30,26,38,24,10,7,36,10,37,4,24,17,13,19,20,33,35,22,17,23,1,10,5,30,5,14,20,31,24,40,null,30,24,20,16,26,8,21,20,32,15,36,24,35,6,20,9,32,9,0,23,37,3,13,30,38,22,33,34,39,5,20,21,26,9,27,14,23,22,27,38,21,20,24,35,24,38,16,3,24,null,14,10,36,4,8,3,9,11,10,6,15,12,35,1,28,25,37,10,26,19,30,7,18,14,12,12,20,5,28,14,43,30,6,1,29,1,29,9,3,3,17,20,3,14,35,41,36,8,30,40,10,38,8,25,0,25,14,36,0,2,1,28,31,20,44,30,35,34,15,10,10,8,10,37,1,5,37,22,19,10,17,36,16,8,17,7,1,33,12,32,40,3,13,28,33,20,1,1,27,4,35,10,1,18,10,24,9,33,41,38,5,9,8,5,23,12,3,46,30,19,30,27,33,14,32,19,26,31,8,10,36,11,2,18,25,4,37,0,16,41,14,29,20,9,10,3,38,20,11,15,38,32,32,35,37,24,13,26,38,2,6,22,9,15,19,43,34,25,11,13,17,5,18,20,3,5,25,30,10,25,30,4,2,18,30,3,9,17,18,8,6,24,25,34,0,18,34,6,15,40,24,40,15,5,3,23,24,8,14,3,42,12,26,24,3,14,35,11,7,34,0,7,34,1,10,36,30,21,27,18,20,15,26,8,25,35,20,28,22,12,7,4,22,18,25,24,24,8,15,33,36,8,10,9,30,1,23,35,13,22,8,10,5,25,13,5,20,38,31,13,28,11,43,24,31,40,27,1,0,33,15,44,12,12,40,23,21,25,13,37,20,20,38,0,30,7,18,18,23,null,37,9,10,25,7,30,16,10,25,2,29,40,10,11,18,20,22,14,20,8,3,23,28,10,4,34,8,28,16,29,31,24,2,37,22,17,21,16,20,7,32,12,0,38,22,1,25,15,38,13,19,21,20,7,34,6,23,12,10,18,3,39,10,40,32,31,28,34,35,10,5,5,16,32,17,20,39,7,13,26,5,24,35,40,10,27,13,39,34,6,39,10,32,27,24,10,36,10,17,22,30,41,43,36,20,11,2,28,1,22,40,25,40,4,13,6,6,6,5,14,1,9,5,41,12,10,24,35,39,6,28,13,33,7,35,6,5,6,27,46,18,37,33,25,11,22,8,17,5,9,20,45,24,1,30,19,21,1,23,18,23,0,7,6,15,23,5,21,24,22,2,9,6,3,18,14,3,28,14,3,38,28,30,2,30,20,18,17,39,25,37,4,18,4,8,20,11,5,30,2,4,4,35,19,10,23,15,3,20,40,42,35,24,33,25,5,7,6,28,27,25,1,39,23,38,12,28,3,11,16,3,28,3,5,13,31,25,33,12,11,18,18,13,11,15,30,17,34,15,25,20,14,29,12,36,17,22,10,4,6,13,27,10,39,7,13,31,9,12,19,9,32,20,30,42,19,27,20,30,15,2,9,38,34,35,10,42,34,6,37,26,22,4,3,5,13,0,17,20,26,20,2,23,6,34,17,32,33,40,7,7,10,7,2,23,33,9,3,20,26,23,31,23,23,25,34,30,8,5,31,6,7,19,1,24,27,36,12,32,17,5,14,32,32,10,5,16,36,7,16,34,24,12,23,35,20,20,23,28,15,6,23,12,28,38,15,3,35,20,26,12,30,17,25,8,26,33,19,26,18,18,20,35,33,9,12,27,null,4,7,31,14,16,15,20,32,22,9,27,11,19,32,17,25,42,null,7,11,40,15,4,26,15,32,20,33,37,13,32,35,12,10,17,31,10,21,20,40,9,14,34,2,38,1,20,30,30,12,14,12,36,27,21,23,23,34,40,17,30,28,33,39,20,1,2,4,42,38,10,4,13,24,8,7,18,1,34,5,39,28,18,36,17,10,32,6,31,10,9,8,24,27,30,20,8,11,23,34,32,9,36,9,32,19,16,11,14,24,30,13,30,33,30,32,36,30,10,3,32,35,0,10,28,34,41,20,7,7,25,38,38,12,9,10,25,21,1,28,27,28,40,3,12,30,15,8,1,15,3,41,15,3,45,12,3,33,35,32,36,6,26,7,34,40,4,3,3,1,26,15,23,12,1,34,28,13,25,41,20,20,14,11,30,17,14,39,3,21,28,21,26,19,22,7,8,null,37,42,4,8,0,35,29,8,40,10,30,12,22,11,11,15,13,9,1,40,8,15,27,23,22,2,37,20,20,40,12,10,26,30,2,12,3,41,17,15,34,29,31,17,36,21,10,1,38,32,40,42,12,22,28,11,23,37,12,18,33,23,29,33,4,32,32,13,30,36,15,17,0,2,34,6,24,13,8,25,26,26,19,4,8,13,33,37,2,30,14,13,2,40,30,42,20,18,24,28,36,11,38,36,13,3,17,30,9,1,33,36,38,7,1,35,28,32,16,null,38,24,37,26,19,15,36,32,34,7,22,1,5,5,36,47,34,32,36,18,12,1,12,20,22,42,11,5,28,15,7,16,24,16,3,22,6,33,8,23,15,15,0,3,20,20,13,45,8,30,7,2,4,9,36,10,5,18,12,33,30,34,33,13,2,35,15,38,6,12,47,12,33,11,25,36,43,10,19,30,9,20,6,13,15,23,27,16,36,17,11,26,10,41,30,13,15,25,25,11,41,5,18,18,10,24,25,17,28,16,8,12,16,14,10,18,18,2,2,13,20,34,10,24,2,15,17,25,29,37,21,1,35,11,23,1,15,27,12,17,10,1,25,22,13,36,27,1,40,25,22,32,19,2,32,null,25,17,38,16,12,13,12,14,26,20,7,20,40,16,25,13,12,11,10,3,17,18,38,3,32,10,28,23,9,34,45,4,2,22,27,32,40,18,2,18,17,20,15,33,14,10,25,22,9,12,2,29,24,22,4,1,39,16,36,36,7,11,32,8,13,28,2,null,38,15,8,20,5,11,20,28,38,32,41,12,17,24,8,6,13,37,19,21,5,10,37,17,37,3,12,20,43,25,20,25,39,15,24,24,4,38,20,26,23,40,12,32,16,24,29,16,17,19,30,30,7,38,10,18,20,40,9,42,22,0,15,38,15,12,15,26,3,30,28,13,3,7,5,6,3,16,30,23,3,1,38,18,18,33,1,32,11,38,30,5,20,28,28,47,20,5,27,38,34,4,1,29,32,18,10,23,7,4,38,18,23,25,12,9,18,16,20,30,15,30,18,40,15,15,26,32,42,31,8,40,2,27,6,28,6,33,22,23,19,20,14,30,0,23,18,21,43,0,20,36,30,33,25,7,47,9,6,9,35,13,3,10,25,28,41,29,20,3,25,12,23,8,46,12,2,16,11,22,39,36,16,10,36,34,18,16,1,36,4,20,25,41,17,14,16,6,36,29,40,6,23,22,20,15,19,12,14,18,15,15,39,38,30,42,13,41,14,8,5,3,24,19,3,29,2,5,13,27,13,32,3,28,5,3,10,33,10,20,32,13,5,13,21,2,28,8,13,35,32,9,4,1,14,38,25,4,4,33,21,7,20,27,6,17,0,22,18,38,6,8,41,38,1,24,30,6,4,13,45,7,19,25,11,23,5,0,5,25,42,39,37,20,27,16,42,35,2,4,17,20,22,8,20,1,8,1,3,21,17,46,10,32,20,26,3,41,22,7,46,39,37,2,26,25,37,10,5,27,30,20,1,6,22,25,24,35,10,17,2,20,22,15,11,11,5,20,35,18,38,10,35,32,12,16,38,12,10,22,14,22,46,29,18,17,35,31,20,33,0,30,28,32,null,16,25,15,3,6,2,23,24,23,21,16,29,17,13,1,37,20,10,22,10,25,6,31,31,10,14,9,35,15,41,6,7,32,14,20,14,34,17,43,38,21,10,4,7,21,10,36,19,1,7,14,17,8,27,4,40,8,37,13,14,16,10,8,13,41,18,20,33,7,5,2,20,24,15,19,30,5,6,28,14,11,31,44,34,12,10,37,28,25,1,8,14,26,10,38,1,15,21,36,23,0,31,39,15,7,14,6,14,39,30,12,19,12,14,27,4,22,21,24,7,4,18,6,0,15,29,37,34,9,42,20,2,9,4,39,23,20,37,27,28,20,23,38,0,7,30,42,31,42,13,20,36,35,24,18,1,11,40,10,16,32,40,20,27,10,40,12,3,9,37,8,30,30,47,13,32,24,15,1,18,29,38,30,11,18,20,2,12,28,17,42,5,34,35,4,31,14,16,39,32,3,30,27,12,8,20,12,11,11,16,30,32,28,1,34,39,35,26,30,12,6,17,2,1,22,15,7,37,15,18,20,29,9,18,28,12,29,16,34,36,1,8,18,38,38,10,12,12,24,19,22,29,16,10,29,20,11,20,13,15,3,37,17,24,22,37,45,25,2,11,1,23,36,26,21,30,7,35,14,17,5,41,20,11,16,2,5,23,2,19,20,28,12,2,1,8,7,5,21,10,31,30,38,7,41,29,25,32,10,11,30,14,33,10,11,41,6,7,2,38,3,30,8,15,14,38,18,17,9,33,44,37,8,19,39,23,33,14,25,30,21,30,38,2,16,5,17,5,17,7,38,2,6,39,20,26,15,13,24,20,13,36,20,30,20,6,0,13,0,31,23,28,40,37,22,15,31,42,38,25,3,4,30,2,1,37,10,18,1,14,28,22,32,0,0,1,7,23,1,13,30,37,12,4,31,32,30,4,4,20,28,25,32,29,19,5,2,11,15,37,15,3,9,15,34,41,13,3,1,3,26,28,33,10,28,35,3,30,1,34,1,20,10,8,27,12,4,37,9,26,23,39,39,21,22,4,4,2,3,18,33,34,26,8,32,31,35,4,28,27,15,37,7,15,2,41,30,6,39,14,4,3,35,18,13,14,11,19,20,22,13,33,8,27,20,22,11,10,12,3,6,15,29,4,12,8,13,2,24,11,39,32,10,17,24,14,39,7,28,38,16,10,1,0,38,35,24,5,12,31,30,21,16,25,3,22,11,37,37,1,10,17,15,32,11,11,18,10,8,26,39,5,1,6,29,35,22,1,6,28,21,40,11,32,36,7,32,17,25,19,4,15,33,null,30,5,2,39,5,3,28,11,5,25,13,31,29,22,42,17,32,8,24,38,22,18,30,28,6,7,2,8,0,25,20,39,15,30,13,5,30,25,2,null,7,0,25,25,13,24,18,7,37,6,20,27,10,20,2,6,5,8,22,27,5,25,43,30,2,36,25,6,38,9,33,35,20,21,26,0,0,39,45,30,15,35,7,33,17,5,6,6,5,3,2,0,35,34,15,1,35,16,5,9,5,19,20,44,22,17,18,9,32,10,10,0,7,34,40,23,0,20,26,6,5,9,41,33,6,6,15,12,37,27,46,32,24,16,23,5,5,31,4,33,41,16,18,34,30,41,25,36,32,39,4,7,15,14,null,38,13,15,10,30,18,17,13,9,30,14,12,8,25,39,10,20,13,38,40,8,42,33,27,31,6,12,30,35,16,3,41,10,4,14,15,22,22,26,5,22,4,8,13,40,15,27,10,12,7,6,1,19,10,19,20,0,20,9,3,2,38,22,32,18,2,26,12,12,15,27,6,39,18,8,11,25,7,6,14,25,15,15,14,36,3,18,20,11,16,19,5,32,14,0,19,15,14,30,37,32,20,11,14,3,20,10,12,20,20,36,10,15,0,0,23,32,6,36,34,4,16,12,15,7,18,24,25,36,27,5,21,3,40,30,8,18,21,35,6,6,38,15,12,0,33,34,10,27,13,2,4,1,9,5,37,18,1,30,14,17,20,1,17,24,10,1,8,18,22,17,34,37,40,24,6,35,8,10,24,18,15,13,36,12,25,2,3,40,10,11,30,8,20,20,20,6,1,6,12,35,34,10,6,15,0,32,15,0,8,12,12,2,2,40,17,30,7,4,16,23,23,12,6,11,33,23,4,2,45,27,18,25,0,27,23,41,20,40,25,42,9,3,5,15,14,3,31,20,24,4,35,40,9,38,16,4,1,16,30,13,27,7,25,22,34,24,2,6,0,28,39,35,7,40,9,5,25,13,2,20,33,5,39,29,8,15,22,35,8,30,29,25,15,12,22,2,2,30,18,12,33,10,31,39,24,14,1,32,2,20,19,35,37,13,27,36,1,35,25,3,15,17,28,1,15,10,47,12,2,15,35,30,20,5,30,11,10,15,20,16,5,22,17,28,43,22,12,12,32,8,33,15,42,37,23,25,3,12,37,24,20,7,3,11,7,17,1,26,10,14,34,15,40,6,0,16,30,18,7,20,17,28,28,21,10,39,20,21,41,14,8,15,4,1,34,16,13,12,10,37,21,14,14,27,11,31,8,28,30,19,24,27,8,6,1,2,36,18,19,24,1,13,25,38,11,10,29,7,13,39,44,26,27,1,20,15,38,3,4,32,7,26,27,8,3,25,0,12,13,23,10,1,21,42,5,30,11,28,12,30,23,20,9,35,18,4,14,1,29,21,29,29,16,7,34,38,7,37,32,24,13,37,15,3,32,33,9,13,31,3,31,22,15,5,32,10,5,28,29,23,2,30,41,30,15,20,33,25,11,17,7,14,12,13,7,23,25,8,31,3,30,15,31,5,14,42,14,35,11,22,30,40,26,21,15,28,34,36,1,4,31,3,41,18,18,13,3,11,40,33,8,34,10,32,9,6,7,15,30,3,7,41,22,28,14,27,18,30,18,34,29,31,0,9,25,15,30,18,32,16,7,1,26,26,45,28,10,14,18,12,14,26,28,35,18,31,16,21,6,9,14,6,47,23,11,8,8,7,11,11,14,31,33,18,6,45,10,5,34,24,8,9,18,9,30,19,6,16,5,30,11,8,21,40,44,0,16,25,47,4,25,27,7,34,31,2,22,5,42,4,17,2,30,18,1,18,8,2,10,20,46,23,19,6,1,47,6,45,10,25,41,29,8,12,23,2,14,20,26,31,4,31,19,1,5,33,3,37,26,null,25,14,16,14,6,6,24,12,33,24,36,15,27,17,20,7,6,24,13,23,8,27,19,12,34,35,32,40,36,3,22,19,31,25,29,15,14,29,11,30,3,4,21,19,39,19,29,18,20,32,8,7,29,8,26,24,20,20,10,25,12,12,16,40,25,6,19,4,11,16,15,7,39,26,24,6,11,26,18,13,30,7,7,37,33,43,8,13,23,35,15,31,15,33,4,31,20,13,13,37,40,38,4,14,23,6,35,2,13,19,31,3,32,10,28,37,18,26,39,2,15,26,8,23,0,25,30,17,27,14,5,27,30,19,7,26,8,17,25,0,4,28,16,0,1,20,17,9,46,10,5,10,16,15,17,20,27,20,24,17,31,15,29,17,38,13,22,12,11,30,5,8,10,4,20,34,37,17,6,25,22,15,2,27,34,19,12,18,12,29,43,26,3,24,27,18,36,17,7,37,3,10,35,41,42,34,43,12,27,46,35,8,15,1,18,2,10,35,16,35,22,15,35,12,20,6,8,31,14,26,3,16,4,32,8,16,23,15,43,11,28,9,37,45,34,13,10,2,7,32,3,24,32,40,22,25,12,22,8,12,12,11,34,7,1,8,26,7,47,18,15,18,40,10,27,27,9,10,32,41,18,17,17,10,17,15,24,14,15,15,22,11,13,32,8,37,18,10,21,41,15,18,8,24,28,34,26,5,11,20,31,25,13,4,14,45,25,17,14,28,18,35,47,12,15,15,11,17,34,8,35,4,3,20,38,41,10,13,15,11,5,2,4,13,17,18,9,18,20,22,6,8,15,18,7,24,1,20,25,28,19,0,15,47,45,11,22,45,27,30,6,12,23,7,34,5,3,24,11,9,7,12,28,7,11,21,20,38,34,11,18,30,40,11,47,16,11,31,15,8,1,18,25,3,45,31,40,16,27,32,33,30,14,26,19,3,16,12,12,41,47,30,41,34,9,22,30,29,13,32,10,14,7,21,17,22,25,20,20,24,5,35,41,17,16,10,38,15,25,14,7,21,26,20,27,45,25,38,6,6,39,5,10,4,21,23,38,24,18,15,22,26,35,22,15,4,8,5,34,11,24,3,17,34,20,25,47,18,5,36,10,35,30,42,34,39,10,31,22,10,17,2,5,24,43,26,11,22,14,20,38,26,7,23,5,42,25,10,7,21,33,18,21,37,4,26,15,25,35,4,34,43,13,34,24,32,16,13,1,20,8,30,19,35,19,24,5,15,24,37,0,25,23,14,14,40,15,17,2,10,20,37,15,41,16,16,46,12,23,0,14,24,12,2,14,21,15,30,9,20,22,11,12,2,17,20,19,27,15,27,20,19,3,41,37,19,8,14,1,12,20,7,26,42,6,2,10,10,0,40,16,22,30,36,30,4,8,22,8,38,13,13,7,40,15,23,35,28,16,10,22,10,22,10,14,37,18,19,5,21,17,18,17,7,4,14,24,7,4,38,11,24,34,39,20,17,6,24,30,24,25,8,32,29,10,12,40,15,23,5,35,42,5,22,8,25,26,6,6,26,1,12,8,30,5,23,14,43,18,14,5,27,32,28,32,14,10,47,7,1,30,10,30,30,21,6,27,27,11,15,17,15,38,6,20,2,11,24,26,34,6,15,43,14,2,12,14,10,45,27,22,4,30,30,18,35,22,20,43,30,32,17,42,26,44,4,14,15,34,6,14,28,6,22,10,24,45,30,12,30,34,37,35,11,29,26,22,12,14,44,13,24,13,6,40,33,14,32,1,8,32,5,6,16,22,8,40,11,9,7,12,31,38,26,17,7,12,32,20,15,2,30,38,22,47,43,25,20,15,22,0,25,10,20,10,26,27,20,30,15,17,26,26,14,29,16,20,1,18,20,14,10,31,9,4,34,10,25,14,5,9,15,30,47,15,32,44,47,30,30,9,15,28,18,4,43,24,21,35,47,15,34,15,15,12,25,36,30,43,15,11,33,1,30,1,12,12,11,36,23,15,40,11,37,13,43,15,32,6,25,32,26,25,1,6,10,20,30,17,15,17,2,23,4,4,18,40,20,45,7,11,7,15,22,30,30,20,24,8,12,20,10,10,18,18,30,20,22,9,28,25,8,20,6,23,23,20,4,30,15,3,6,12,12,11,18,14,6,17,9,14,24,16,11,19,37,26,16,36,29,25,7,7,26,20,22,20,22,15,14,10,6,21,10,11,21,8,35,12,10,25,10,16,25,24,20,22,16,35,11,11,23,32,34,31,12,11,3,13,10,20,25,33,14,3,16,21,25,6,6,28,17,28,20,36,20,2,5,37,21,12,2,5,19,4,10,20,6,7,1,15,40,21,11,16,34,26,23,10,1,13,4,10,28,11,20,17,11,25,24,20,2,39,16,23,30,28,5,9,20,20,15,32,16,20,20,22,28,5,23,18,19,27,26,26,31,8,10,9,22,6,16,28,18,37,12,21,20,30,9,22,18,19,11,6,28,28,11,32,2,5,27,10,13,4,11,18,12,6,18,15,22,20,24,10,20,12,30,34,8,39,18,1,5,19,18,10,15,30,17,18,15,3,10,null,11,14,31,8,37,18,11,20,16,20,34,40,26,36,35,39,3,20,32,25,18,17,3,37,11,17,11,24,20,28,11,3,4,24,15,1,28,3,35,15,12,40,10,17,37,20,10,18,2,8,40,14,12,14,17,5,10,34,12,27,17,14,17,4,1,4,15,24,14,16,38,12,20,4,26,3,17,12,17,6,28,1,24,30,17,6,1,35,8,8,25,16,16,3,4,13,5,1,24,8,34,23,22,10,20,10,29,24,20,15,33,36,9,17,24,24,33,28,16,10,10,8,25,6,38,5,37,23,12,22,15,9,14,18,37,6,19,7,20,8,27,37,36,15,35,22,1,12,25,20,20,32,30,8,10,28,10,4,20,15,3,25,23,9,10,15,5,4,20,29,15,17,11,6,3,37,34,25,16,14,23,30,18,28,27,13,24,5,37,15,4,38,17,20,27,6,30,20,11,22,33,8,8,6,1,25,8,37,35,38,8,2,15,45,15,5,15,39,10,35,33,10,25,8,34,1,15,8,4,20,29,37,35,15,20,13,21,8,35,1,20,2,10,30,30,14,21,4,25,24,20,41,5,8,14,30,0,21,8,5,22,27,34,18,15,8,32,15,22,9,6,32,21,8,20,22,13,15,2,3,20,26,4,21,20,17,5,7,5,15,31,11,1,38,25,1,6,12,14,15,30,13,10,22,8,27,27,15,15,25,25,13,15,19,13,24,4,16,10,20,10,13,25,13,35,24,12,19,16,4,1,40,1,20,28,28,10,22,9,25,17,21,30,17,23,10,1,9,30,1,39,20,5,36,11,25,20,33,7,4,25,1,2,6,32,8,5,2,20,18,10,10,2,30,8,2,36,23,35,1,10,0,14,10,21,22,30,3,20,22,38,31,18,6,20,28,4,11,30,38,11,19,13,40,30,10,28,9,12,34,12,30,35,12,16,40,20,6,19,5,19,4,2,10,7,9,1,15,2,30,7,26,34,17,15,30,7,10,38,30,20,15,26,12,12,11,24,17,30,6,24,18,19,19,12,9,15,33,5,10,7,39,26,23,27,20,22,2,7,23,10,13,7,34,0,20,14,33,14,36,24,3,37,24,6,11,39,8,35,5,22,15,20,30,19,6,5,20,32,20,4,16,13,6,18,12,35,6,2,12,11,20,36,36,29,36,14,3,10,19,16,1,7,32,28,16,10,30,11,18,7,12,1,15,12,1,12,20,24,22,22,24,20,16,25,31,13,11,13,28,28,26,22,12,1,20,6,30,19,22,25,15,27,19,25,11,20,20,33,5,20,15,12,16,11,30,16,14,5,22,12,15,20,25,15,25,11,20,19,1,26,21,10,3,5,25,42,30,8,11,0,37,22,28,3,21,30,38,14,30,5,28,21,18,16,18,0,27,20,21,7,30,39,19,39,32,25,30,7,14,18,9,20,18,5,38,40,35,39,16,4,5,7,37,24,5,16,25,17,24,15,0,34,22,47,4,4,20,26,19,9,20,5,1,21,14,9,7,27,17,19,36,18,33,28,30,40,2,19,35,9,33,18,40,14,11,15,20,13,25,30,8,10,5,33,8,22,4,5,16,18,34,20,10,20,7,30,13,4,5,46,25,37,10,30,16,5,9,2,12,3,10,7,9,22,22,21,33,28,32,1,38,26,17,39,12,19,17,31,1,25,32,30,5,23,15,21,17,28,17,9,5,23,20,37,18,15,4,10,10,34,15,30,31,29,15,8,11,6,6,2,20,20,10,29,6,35,5,5,28,3,21,22,32,26,33,10,20,15,22,37,23,24,17,2,4,17,19,41,33,34,25,4,34,20,4,23,27,5,9,4,10,15,5,26,20,10,4,7,27,20,8,29,12,14,10,30,26,34,19,6,26,34,2,16,23,7,17,18,6,32,23,20,13,23,21,1,7,23,19,1,5,32,24,5,24,30,33,2,14,20,14,30,25,14,20,22,18,20,20,8,13,30,20,12,2,14,5,12,20,22,35,16,10,35,5,10,30,22,10,20,2,15,1,3,28,34,34,1,23,33,25,10,13,14,10,20,22,23,32,2,18,20,5,17,30,10,17,11,13,3,3,17,28,7,19,3,6,13,22,4,36,40,3,16,16,17,10,26,7,12,10,38,8,32,12,10,20,15,10,8,13,2,23,8,24,28,16,10,1,6,1,30,7,28,34,10,25,37,29,20,38,25,16,35,10,25,5,27,28,20,12,21,30,13,3,30,21,10,24,29,25,31,10,20,20,25,14,25,6,21,6,5,25,21,13,13,20,15,15,18,10,16,16,10,1,8,17,25,27,8,31,37,26,3,14,4,20,11,23,11,27,22,24,34,35,18,10,27,38,30,16,40,5,26,22,40,6,24,31,8,25,24,10,13,35,15,8,13,8,1,25,30,9,25,1,41,15,10,13,18,15,22,21,18,1,30,20,7,1,43,5,39,24,17,16,16,6,1,2,22,32,25,9,13,18,22,27,8,16,12,14,23,15,15,8,11,4,21,22,8,43,16,27,34,4,28,14,32,20,22,28,15,18,27,4,37,5,19,16,10,13,28,11,14,6,2,13,4,25,32,7,20,3,25,23,20,10,14,12,13,6,15,22,27,32,13,8,18,23,27,20,10,26,23,14,15,2,30,13,30,21,4,2,28,34,30,10,25,34,15,19,14,27,17,4,7,20,3,25,25,11,10,18,5,10,37,11,35,23,21,1,36,1,11,12,35,19,45,7,4,27,37,9,38,11,11,22,11,15,9,26,12,25,24,33,10,13,12,30,18,31,30,15,31,23,23,11,26,28,17,5,20,12,38,25,15,16,20,12,24,37,14,5,21,26,35,30,15,18,6,19,15,10,18,15,5,23,17,3,20,35,10,2,26,20,30,20,10,30,35,23,39,16,32,7,22,21,22,14,2,2,15,8,10,35,8,10,27,10,26,6,21,19,11,2,11,11,9,34,27,9,32,17,20,15,35,15,28,24,20,18,8,25,18,20,20,35,8,15,18,4,3,14,10,24,5,13,33,1,23,2,34,20,19,7,11,8,28,1,30,33,2,20,30,30,5,22,12,20,20,10,25,11,33,20,3,3,4,38,15,14,3,13,7,20,22,9,22,20,4,30,14,10,20,2,8,16,4,24,6,19,29,13,20,24,14,34,2,2,20,10,4,7,16,22,31,7,8,2,37,23,5,5,16,2,23,20,7,7,10],"Partner":["Yes","No","Yes","Yes","No","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","No","Yes","Yes","No","No","No","Yes","Yes","Yes","No","Yes","Yes",null,"Yes",null,"Yes","Yes","Yes","No",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes",null,"Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes",null,"No","No","No","Yes","No","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","No","Yes","No","No","Yes","No","No","Yes","Yes","No",null,"No","Yes","No","Yes","Yes","Yes","Yes","No","Yes","No",null,"No","Yes","Yes","Yes","Yes",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","No","No","Yes","No","Yes","No","Yes","Yes","No","Yes","Yes","Yes","No",null,"Yes","Yes","Yes",null,"Yes","Yes",null,"Yes","No",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","No","Yes","Yes","No",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","No","No","No","Yes","No","Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","No","No","Yes","No","Yes",null,"Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"No","No","Yes","No","Yes","No","No","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","No","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","No","No",null,"Yes","No","No","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","No","No","Yes",null,"Yes",null,"No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","No","Yes",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes",null,"Yes","No","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","Yes",null,"Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","No","No","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","No","No","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes",null,"Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","No","No","No",null,"Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes",null,"Yes","Yes","No","Yes","Yes",null,null,"Yes","No","Yes","Yes","No","Yes","No","Yes",null,"No","Yes",null,"No","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"No","No","No","Yes","Yes","No","Yes",null,"Yes","Yes","No","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","No","No","Yes",null,"No","Yes","No","No","No","No","No","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes",null,"No","No","Yes","Yes","Yes","No","Yes","No","Yes","No","Yes",null,"Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","No","Yes","No","No","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","No","Yes",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"No","No","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","No","Yes","Yes","Yes",null,"No","Yes","Yes","Yes","Yes","No","No",null,"No","No","No","No","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","No","Yes","Yes","Yes",null,"Yes","No","Yes","Yes",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"No","Yes","Yes","No","No","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","No","No","Yes",null,"Yes","No","No","Yes","No","Yes","Yes","No","Yes","No","No","No","Yes","Yes","No","Yes","Yes",null,"Yes","No","Yes",null,"Yes","Yes","Yes","Yes","No","No",null,"Yes","Yes","Yes","Yes","No","No","Yes","Yes","No","Yes",null,"Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"No","No","No","Yes",null,"Yes","Yes","Yes","No","Yes","Yes",null,"No","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","No",null,"Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","No","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","No","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","No","No","Yes","No","No","Yes","No","Yes","Yes","Yes","No","Yes","No","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes",null,"Yes","Yes","No","No",null,"No","No","Yes","No","Yes","Yes","No","No",null,"No","Yes",null,null,"No","Yes",null,null,"Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","No","No",null,"Yes","Yes","Yes","No","Yes","No","Yes","No","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","No","Yes","Yes","No","No","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","No","No",null,"Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","No","Yes","No",null,"Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes",null,"Yes","No","Yes","No","Yes","Yes","No","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","No","No","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes",null,"No","Yes","Yes","No","Yes","Yes","No","Yes","Yes","No","Yes","No","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes","No","No","No","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","No","No","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","No",null,"Yes","Yes","No","No","Yes","No","Yes","No","No","No","No","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","No",null,null,"Yes","Yes",null,null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes",null,"No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"No","No","Yes","No","No","Yes","Yes","No","No","No","Yes","Yes","Yes","No","Yes","No","Yes",null,"Yes","Yes","Yes","No","Yes","No","No","No","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","No","No","No","Yes","No","No","Yes","No","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","No","No","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","No","Yes","No","Yes","Yes","Yes","Yes","No","No",null,"Yes","No","Yes","No","Yes","Yes","No",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","Yes",null,"Yes","No","Yes",null,"No","No","Yes","Yes","Yes","No","Yes","No",null,null,"Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","No","Yes","Yes","No","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","No","No","Yes","Yes",null,"No","Yes","No","Yes","Yes","Yes","No",null,"Yes",null,"No","Yes","Yes","No","No","No","No","Yes",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","No","No","Yes","No","Yes","No","No","Yes","Yes","No","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","No","Yes","Yes","No","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes",null,null,"No","Yes","Yes",null,"No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","No","No",null,"Yes","Yes","Yes","Yes","Yes","Yes",null,"No","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","No","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","No","No","No","Yes","No","Yes",null,"Yes",null,"Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"No","Yes","Yes",null,"Yes",null,"Yes",null,"No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","No","No","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","No","Yes","Yes","Yes","No","No","No","No","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","No","No","Yes","No",null,"Yes","Yes","No","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","No","Yes","Yes","No","Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"Yes",null,"Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes",null,"Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No",null,"Yes","Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","Yes",null,"No","No",null,"Yes",null,"Yes","Yes","No","Yes","No","No",null,null,null,"Yes",null,"Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","No",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","No","No",null,null,"Yes",null,"Yes","No","Yes",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,null,"Yes","Yes",null,null,"Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes",null,null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","No","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,null,"Yes",null,"Yes","Yes","Yes",null,null,"Yes","Yes","No",null,"No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","No","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","No","Yes","Yes","Yes","Yes","No",null,"Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","No","Yes","No","Yes","Yes","Yes","No","Yes",null,null,"Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes",null,"Yes","Yes",null,"Yes","No","Yes","Yes","Yes","No",null,"No","Yes","No",null,null,"Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","Yes","No","Yes","No","Yes","No","No","Yes","Yes","Yes","No","Yes","No",null,"Yes",null,null,"Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","No","No",null,"Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","No","Yes","Yes","No",null,"Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes",null,"No","Yes","No","Yes",null,"Yes","Yes","Yes","Yes",null,"Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,null,"Yes","Yes","Yes","Yes",null,null,"No","Yes","Yes","Yes",null,"Yes","Yes","Yes",null,"Yes","Yes",null,"Yes","Yes","Yes","Yes",null,"No","Yes","Yes","No",null,"Yes",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","No","No","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,"No","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","Yes",null,"Yes","Yes",null,null,"Yes",null,"Yes","Yes",null,"Yes",null,"Yes","Yes","Yes","No","No","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","No","Yes","No","Yes",null,"No","Yes","Yes",null,"Yes","Yes",null,"Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","Yes",null,"No","Yes",null,"No","Yes","Yes",null,"Yes","No","No","Yes","Yes","Yes",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes",null,"Yes","Yes","Yes","Yes","No",null,null,null,"Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes",null,"Yes","Yes",null,"No","Yes","Yes","Yes","Yes",null,"No","Yes","Yes","Yes","No","Yes","Yes",null,"No",null,"No",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","No","No","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes",null,"Yes","No","Yes",null,"Yes",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","No","Yes","Yes","No",null,null,"Yes","No",null,null,"Yes","Yes","Yes","Yes",null,"Yes",null,"Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"Yes",null,"Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","No","Yes","No","No",null,"Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes",null,"No",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes",null,"Yes","No","Yes","Yes","No","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","Yes",null,"Yes","No",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes",null,null,null,"Yes",null,"Yes",null,null,"Yes","Yes","No","Yes","No","No","No","No","Yes","Yes","Yes",null,"Yes","Yes","No",null,"No",null,null,"Yes","Yes","Yes","Yes","Yes","No","Yes","Yes",null,"No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","No","Yes","Yes","Yes","Yes",null,"No","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"No","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","No","Yes",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes",null,"Yes",null,"Yes",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes",null,"Yes",null,"No","No","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,null,"Yes","No","Yes","No","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes",null,"Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","No","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","No","Yes","Yes","No","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,null,"No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,"Yes",null,"Yes",null,null,"Yes","No","Yes","No","No","Yes","Yes",null,"No","Yes",null,"No","Yes","Yes",null,"Yes","Yes","Yes","No",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes",null,null,"Yes","Yes",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","No",null,"No","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes",null,null,"Yes","Yes","No","No","No",null,"Yes","No","Yes",null,"Yes","Yes","Yes",null,null,"Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","No","Yes","Yes",null,null,"Yes","Yes","Yes","Yes","No","Yes",null,"No","Yes","Yes","Yes","Yes","Yes","No","Yes",null,null,"No","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","No","Yes","Yes","Yes","Yes",null,"Yes","Yes",null,"Yes","Yes",null,"No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","No",null,"No","Yes","Yes","No",null,null,"Yes",null,"Yes","No","Yes","Yes","Yes","Yes","No",null,"Yes","No","Yes",null,"Yes","No","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes",null,"No","Yes","Yes","No",null,null,null,"Yes","Yes","Yes","Yes","Yes",null,null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","No","No",null,null,"Yes","No","No","Yes",null,"Yes","Yes",null,null,"Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No",null,"Yes","No","Yes","Yes","No",null,"Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","No",null,"Yes","Yes","Yes","No","Yes","No","Yes","Yes",null,"No",null,"Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","No","No","Yes","Yes","Yes","Yes","No","No",null,"Yes","Yes","No","Yes","Yes","Yes",null,"Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes",null,null,"Yes","No","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes",null,"Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","No","Yes","Yes","No","No","No","Yes","Yes","No","Yes","No","Yes","Yes","No","Yes","Yes","No","No","Yes","Yes","Yes",null,"Yes","Yes","Yes","No","Yes","Yes","Yes",null,"Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes",null,"No",null,"Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes",null,"Yes","Yes","No","Yes",null,null,"Yes","No","Yes",null,"No","Yes","Yes","Yes","Yes","No","Yes",null,"No","Yes","No","Yes","Yes","Yes","Yes","No","No","Yes","Yes","No","Yes",null,null,"Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes",null,"No","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes",null,"No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes",null,"No","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","Yes",null,"Yes","No",null,null,"Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","No","Yes","Yes","Yes",null,"Yes",null,"Yes","Yes","No",null,"Yes",null,"Yes","Yes",null,"Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes",null,null,"Yes","Yes",null,"Yes","Yes","Yes","No","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes",null,"No","Yes","Yes",null,"No","No","Yes","No",null,"Yes","Yes",null,"No","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes",null,"No",null,"No","Yes","Yes","Yes",null,"No",null,"Yes","Yes",null,"No","Yes","Yes","No","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","No","Yes",null,"Yes","Yes",null,"Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","Yes","No","Yes","No","Yes","No","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","No","No","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","Yes","Yes","No",null,null,"Yes",null,"Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,null,"Yes","Yes","Yes","Yes","No","No","Yes",null,null,"Yes","Yes","No","Yes","No",null,"No","Yes","Yes","Yes",null,"Yes","Yes","No",null,"Yes",null,null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes",null,"Yes","Yes",null,"Yes","Yes","Yes",null,null,"Yes","No","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","No","No","No","Yes","Yes","No","Yes","No",null,"Yes","No","Yes","Yes","Yes","Yes","Yes",null,null,"Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"No","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","No","Yes","Yes","Yes",null,"Yes","Yes",null,"Yes","No","Yes","No",null,"No","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","No",null,"Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,null,"No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No",null,null,"Yes","Yes","Yes","No","Yes","Yes",null,"Yes",null,"Yes",null,"Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes",null,null,"Yes","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"Yes",null,"Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","Yes","Yes",null,"Yes",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"Yes",null,"Yes","Yes",null,"Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","No",null,"Yes","Yes","No",null,null,"Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes",null,"No","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","No",null,"Yes",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","No","No",null,null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","No","Yes","Yes",null,"Yes","Yes","Yes",null,"No","Yes","Yes",null,"Yes","Yes","Yes","No","No","Yes","No","No","Yes","Yes","Yes","No","No","Yes",null,"Yes","Yes",null,"No","Yes","No","Yes","No","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes",null,"Yes",null,"No","Yes",null,"Yes","Yes","Yes","Yes","No","Yes",null,null,null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","No","Yes",null,"Yes",null,"No","Yes","Yes",null,null,"Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","No",null,"No","Yes","Yes","Yes",null,"Yes","No","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","No","Yes","Yes","Yes",null,"Yes",null,"Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","Yes",null,"Yes","Yes","No","No","No","No",null,"No","Yes","No","Yes","No","Yes","Yes","Yes","Yes","No","No","Yes","Yes",null,"No","No","No","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","No","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","No","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","No","Yes","Yes",null,"Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes",null,null,null,"Yes","No","Yes","Yes",null,"Yes","Yes","No",null,"Yes","Yes","Yes","Yes",null,null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes",null,null,"No","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","No","No","Yes",null,"No","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","No","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes",null,"Yes","Yes","Yes",null,"Yes",null,"Yes","No","Yes","Yes","Yes",null,"Yes","Yes","No","No","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"Yes","Yes","Yes",null,"No",null,null,"Yes","No","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes",null,"Yes","No","Yes",null,"Yes",null,"No","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","No","Yes","Yes","Yes",null,"Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes",null,null,"No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,null,"Yes","Yes","No","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes",null,"Yes","Yes",null,"Yes",null,"Yes",null,null,"Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes",null,null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","No",null,null,"Yes","Yes",null,"No","Yes","Yes","Yes","Yes","Yes","No","No","No","Yes","No","Yes","Yes",null,"Yes","Yes","No","Yes","No","Yes","No","Yes","Yes","No","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No",null,"Yes","No",null,"No",null,"Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","No","Yes","Yes","No","Yes",null,null,"No",null,"Yes","No",null,"Yes",null,"Yes","No","Yes","Yes","Yes","No",null,"No","Yes",null,null,"No","Yes","No",null,"No","Yes","Yes","Yes","No",null,null,"Yes","No","Yes","Yes",null,"No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","Yes","No","Yes","No","Yes","Yes","Yes","No","No","No","No",null,"No",null,"No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","No","No","Yes",null,null,"Yes",null,null,null,"Yes","Yes","Yes","No","No",null,"Yes","No","Yes",null,"Yes",null,"No",null,"Yes","Yes","Yes",null,"No","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes",null,"Yes","Yes",null,"No","Yes","Yes","No","Yes","Yes","No","No","No","Yes",null,"No","No","Yes",null,"Yes","No","Yes","Yes",null,"No",null,null,"No",null,"Yes","No","No","No","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","No","Yes","No","Yes","No","No","No",null,null,"Yes",null,"Yes",null,null,null,null,"Yes","Yes","Yes","No","Yes",null,"Yes",null,"Yes","Yes","Yes",null,null,"No","Yes","Yes","Yes",null,"No","No","Yes","Yes","No","No",null,"Yes","No",null,"Yes","No",null,"No","Yes",null,"Yes","Yes","No",null,"No","Yes","Yes","Yes","No","Yes","Yes","No",null,"Yes","Yes","No","No","No","No","No","Yes",null,null,"No","Yes","Yes",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,null,"No","Yes","Yes","Yes","Yes",null,"No",null,"No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes",null,"Yes","Yes","No",null,null,"Yes","Yes","Yes","No","No","Yes","Yes","Yes",null,"Yes","No","Yes","Yes",null,"No","Yes","No","Yes","No","Yes","Yes",null,"Yes","No","No","Yes",null,null,"No",null,"Yes",null,"Yes","Yes","No","Yes","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,"Yes",null,"Yes","Yes","Yes",null,null,"Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","No",null,"Yes","Yes","No","Yes",null,"No","Yes","No","Yes",null,"No","Yes","No",null,"Yes","Yes",null,"Yes","Yes","Yes",null,"Yes","Yes","No","Yes","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","No","No",null,null,"Yes",null,"No","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes",null,"Yes","Yes","No",null,"Yes","No","Yes","No","Yes","No","No","Yes","Yes","Yes","No","No",null,"No",null,"No","Yes","No","No","No","No","Yes","Yes","No","Yes","Yes","No",null,"No","Yes","Yes","Yes","No",null,null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,null,null,"Yes","Yes","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","No",null,"Yes","No","Yes","Yes","Yes",null,"Yes","Yes",null,"Yes","No","No","Yes","No","No","Yes","Yes",null,"Yes","Yes",null,"Yes","Yes",null,null,null,"Yes","Yes","No","Yes","Yes","Yes","No","No","Yes",null,"Yes","Yes","Yes","Yes","Yes",null,"No",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"No",null,"Yes","Yes","No","Yes","Yes","Yes","No","Yes","No","Yes","Yes",null,"Yes","Yes",null,"No","Yes","Yes","Yes","Yes","Yes","No",null,"Yes",null,"Yes",null,"No","Yes","Yes","Yes","No","Yes",null,"Yes","Yes",null,"Yes",null,"No","No","No",null,"Yes","Yes","Yes",null,"Yes","Yes","No","Yes","No","No","Yes","No","Yes","No","No","Yes","Yes","Yes","Yes","Yes","No","No","No","No","Yes","Yes",null,"No","Yes","Yes","Yes",null,"No","Yes","Yes",null,"No","Yes","Yes","No","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","No","Yes","No","No","No",null,"No","No","Yes","No",null,null,null,"Yes","No",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","No","No","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","No",null,"Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","No","No","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes","No",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","No",null,null,"Yes",null,"Yes","No",null,null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","No","Yes",null,"Yes","Yes",null,"Yes","Yes","Yes","Yes","No","No","No",null,null,"Yes","No","Yes","Yes","Yes","No",null,"Yes",null,"No","Yes","No",null,null,"Yes",null,"Yes","Yes","Yes","Yes","No",null,"Yes",null,"Yes","Yes",null,"No","No","No","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes",null,"Yes","Yes","No","Yes",null,"Yes","Yes",null,"Yes",null,null,"No","No",null,"Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes",null,"No","No",null,"No","No",null,"No","Yes","Yes","Yes","No",null,"No",null,"Yes","Yes","Yes","No","Yes","Yes","No","Yes","No","Yes","Yes","No",null,"No","Yes","Yes","Yes",null,"Yes",null,"Yes","No",null,null,"Yes","Yes","Yes","No","Yes","Yes","No","No","Yes","Yes","Yes",null,"Yes","Yes","No","No","Yes","Yes","No","No",null,null,null,"Yes","Yes","Yes","Yes","No","No","Yes","Yes","No",null,"Yes","Yes","No","Yes","Yes","Yes","No","No","No","Yes","No","No","No",null,"Yes","Yes","No","No","Yes","Yes","Yes","Yes",null,"No","No","Yes","No","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No",null,null,"Yes","Yes","Yes",null,"Yes","Yes","No","Yes","No","Yes","Yes",null,"No","Yes","Yes","Yes","No","No",null,"Yes","No",null,"Yes",null,"Yes","No","Yes","Yes","Yes",null,"Yes","No","No","Yes","No","No","No",null,"No","Yes","Yes","No","Yes",null,"No","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"No","Yes","Yes",null,null,"Yes",null,"No","Yes","Yes","Yes","Yes",null,"Yes","Yes","No","Yes","No",null,"Yes","Yes",null,"Yes","No","Yes","No","Yes","Yes",null,"Yes","Yes","No","No","No",null,"Yes","No","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","No","Yes","No","Yes",null,"Yes","Yes",null,"Yes","No","Yes",null,null,"No","No","Yes","Yes",null,null,"Yes",null,"Yes",null,"No","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","No","Yes","No","No","Yes","Yes","No","Yes","Yes","No","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes",null,"Yes","Yes","Yes","No","No",null,null,"Yes","Yes","Yes","No","Yes","Yes",null,"No","No",null,"Yes","Yes","No",null,"Yes","No","Yes","Yes","Yes","No","No",null,"Yes",null,null,"No","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","No","Yes","No","No",null,"Yes","Yes","No",null,"Yes","Yes","No","No",null,"Yes","No","No",null,null,"No","No","Yes","No","Yes","Yes","Yes",null,"No","Yes","No","Yes","Yes","No","Yes","No","No","Yes","No","Yes","Yes","No","No",null,"Yes",null,"Yes",null,"No","Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","No","Yes","Yes","No","Yes","Yes","No","Yes","Yes","Yes","Yes","No","No","No","Yes","No","No","No","Yes","No","No","No","Yes",null,"Yes","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes","No","Yes","Yes","No","Yes",null,null,"Yes","Yes","Yes","Yes",null,"No","Yes","No","Yes","Yes","Yes",null,"Yes","No","No",null,"Yes",null,"Yes",null,"Yes","Yes","Yes","Yes","No",null,"No",null,"Yes","No","Yes","No","No","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"No",null,"Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes",null,"Yes","Yes","Yes","No","No","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes",null,"Yes","Yes","No",null,"Yes",null,"Yes","Yes","Yes",null,"No","No","Yes","No",null,null,"No","No","Yes","No",null,"Yes","Yes",null,"No","No","Yes",null,"Yes","Yes","No","Yes","Yes",null,"No","Yes","Yes","Yes","Yes",null,"No","Yes","Yes",null,"Yes",null,"No",null,"No","Yes","No","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No",null,"No","No","Yes","Yes","Yes","No","No","Yes","Yes",null,"Yes","No",null,"Yes","No","Yes",null,"Yes","Yes","No","Yes","Yes","No","No","Yes","Yes","No","No","Yes","Yes","Yes",null,"Yes","No","Yes",null,"No",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"No","Yes","Yes","No","No",null,"No","No","No","Yes","No","Yes","Yes","Yes","No","Yes","Yes","No","Yes",null,"No","No","No","Yes","No","Yes",null,"No","Yes",null,"No","Yes","No","Yes",null,"Yes",null,"No","Yes","Yes","No",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"No","Yes","Yes",null,"Yes","No","Yes","No",null,"No","Yes","Yes","No",null,"Yes","Yes","Yes","No","Yes","Yes","Yes",null,"Yes",null,"Yes","Yes","No",null,"Yes","No","Yes","Yes","No","No",null,"Yes","Yes","No",null,"No","Yes","Yes","Yes","No","Yes","No","No",null,null,"No","No","Yes","Yes",null,"No","Yes","Yes",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No","Yes","Yes",null,"Yes","No","Yes","No","Yes",null,"Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes","No","Yes","Yes","No","Yes","No","Yes","No",null,"No",null,"No","Yes",null,null,"Yes","Yes","Yes","Yes","Yes",null,"No",null,"No","Yes","Yes","No","Yes","No",null,"No","Yes","Yes","Yes","Yes","No","Yes","Yes",null,"No",null,"No","Yes","Yes","Yes",null,"No","No","No",null,null,"Yes","No","No","No","No","Yes","Yes","Yes","Yes",null,"No",null,null,"No","Yes","Yes","Yes",null,"Yes","No",null,"No","No","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes",null,"Yes","No","Yes",null,"Yes",null,"No","Yes","Yes","Yes",null,"Yes",null,"Yes","No","No","Yes","Yes","Yes",null,null,"Yes","Yes",null,"Yes","No","Yes","Yes","No","Yes","Yes",null,null,"Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","No","No",null,"Yes","Yes","Yes",null,"No","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","No","Yes",null,"Yes",null,"No","Yes",null,"Yes","Yes","Yes","Yes","No","Yes",null,null,"No","Yes","Yes",null,null,"Yes","No","Yes","No","Yes","Yes","Yes","No","No",null,"Yes",null,"Yes","No","Yes",null,"No","Yes",null,"No","Yes","No","No","Yes","Yes","Yes","Yes",null,"Yes","No","No","Yes","Yes","Yes","Yes","Yes","Yes",null,null,"Yes","Yes",null,"Yes","Yes","No",null,"Yes","Yes","No","Yes","Yes","Yes","Yes","Yes",null,"No","Yes","No","Yes","No","Yes","Yes","Yes","No","Yes","No","Yes","Yes","Yes","No","No",null,"Yes","No",null,"Yes",null,"No","Yes","Yes",null,"No","Yes","Yes","Yes","No","Yes",null,"Yes","No","Yes","No",null,"Yes",null,null,"Yes","Yes","Yes","No","No","Yes","Yes","No","Yes","No",null,null,"Yes","Yes",null,"Yes","Yes","Yes","Yes",null,"No","No","No",null,"Yes","Yes","No","Yes","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","No",null,"Yes","Yes",null,"Yes","No","Yes","Yes","No","Yes","Yes","No","Yes","No","Yes","Yes","Yes",null,"No","Yes","No","Yes","Yes","Yes","Yes","No","No","Yes","Yes","Yes",null,"Yes","No","Yes","Yes","Yes",null,"Yes","No","No",null,null,null,"No",null,"No","Yes","Yes","Yes","No","No",null,"Yes","Yes","Yes","Yes","No","Yes","Yes","No","No","No","Yes","Yes","No","Yes",null,"No",null,"Yes","Yes","Yes","Yes","Yes",null,"No","No","Yes","Yes","Yes","No",null,"Yes","Yes","No","No","No",null,"Yes","Yes","No","Yes",null,null,"Yes","Yes","Yes","No","No","Yes","Yes","Yes",null,null,"Yes","Yes",null,"No",null,null,"Yes","Yes",null,null,"Yes","Yes",null,"Yes",null,"Yes","No","No","Yes",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes",null,"Yes","No","Yes","No","Yes","Yes","Yes","Yes",null,"Yes",null,null,"Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","No","Yes","Yes",null,"No","No","No",null,"No",null,"No","Yes","Yes","Yes",null,"Yes","No","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","Yes",null,"Yes",null,null,"Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","No","No","No","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","No","No","Yes","Yes","No","Yes","Yes","Yes","No","No","No","Yes","Yes","Yes","No","No","Yes","Yes","Yes","No","No","Yes","No","Yes","No","No","Yes",null,"Yes","No","Yes","No","Yes",null,null,"Yes","Yes","Yes",null,null,"Yes","Yes","No","Yes","Yes","Yes",null,"Yes","Yes","No","Yes",null,"Yes","No","Yes","Yes","Yes","No","Yes",null,"Yes","Yes","No","No","Yes","Yes","No","No","No","Yes","Yes",null,null,"No","Yes","Yes","Yes","Yes","No","Yes","No","Yes","No","Yes",null,"Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes","No","No","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"Yes","Yes",null,"No",null,"No","Yes","Yes","No","Yes","Yes",null,"No",null,null,"No","No","No","No",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes",null,"Yes","Yes","Yes","Yes","No","No",null,"No","No","Yes","Yes","Yes",null,"Yes","Yes",null,null,"No","Yes","No","No","No",null,null,"Yes","No","No","No","No","Yes",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","No","No",null,"No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No","Yes","No",null,"Yes",null,"Yes","Yes","No","Yes","Yes",null,"No","Yes","Yes",null,"No","Yes","Yes","No","No","Yes","Yes","No","Yes","No","No",null,null,"Yes","No","Yes","No","No","Yes","Yes","No","No","Yes","No","Yes","No","No",null,"Yes",null,"Yes","Yes","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","Yes","Yes","Yes",null,"Yes","No","No","Yes",null,"No","Yes","Yes","No","No","Yes",null,null,"Yes","Yes",null,"No","No",null,"Yes","No","Yes","No","Yes","Yes","Yes",null,null,"Yes",null,"No","Yes",null,"Yes","No","No",null,"Yes","Yes","Yes",null,"Yes","No",null,null,"Yes",null,"Yes",null,"Yes","No","No",null,"Yes","No",null,"No","Yes","No","No","No",null,"Yes","No","No",null,"Yes",null,"No","Yes","Yes","Yes",null,"Yes","No",null,"Yes","Yes","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","Yes","Yes","Yes",null,"Yes","Yes",null,"Yes","Yes","Yes","Yes","Yes","Yes","Yes",null,"No","Yes","Yes",null,"Yes","Yes","Yes","Yes","No","Yes","Yes",null,"No","Yes","Yes","No","Yes","Yes","Yes","No",null,"Yes","Yes","Yes","No","No","Yes","Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","Yes","No",null,"Yes",null,"Yes","No","Yes","No","Yes","Yes","Yes","Yes","Yes","No","Yes","No","No","Yes","No","Yes","No","No",null,"No","Yes","Yes","Yes","No","Yes","Yes","Yes","No","No","No","No",null,"No","No",null,null,"Yes","Yes","Yes",null,null,null,null,null,"No",null,null,"No","Yes","No","No","Yes","Yes","Yes","No",null,null,"Yes","Yes","Yes","Yes","Yes",null,"Yes","No","Yes",null,"No","No","Yes","No","No","Yes","No","Yes","No","Yes","Yes",null,null,"No","Yes","No"],"Nationality":["National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","Non_national","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","Non_national","National","Non_national","National","Non_national","Non_national","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","Non_national","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","Non_national","Non_national","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","Non_national","National","National","National","Non_national","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","Non_national","National","National","National","National","Non_national","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","Non_national","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","Non_national","Non_national","Non_national","National","Non_national","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","Non_national","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","Non_national","Non_national","Non_national","Non_national","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","Non_national","Non_national","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","Non_national","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","Non_national","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","Non_national","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","Non_national","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","Non_national","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","Non_national","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","Non_national","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National",null,"Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","Non_national","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","Non_national","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","Non_national","Non_national","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","Non_national","National","National","Non_national","National","Non_national","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","Non_national","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","Non_national","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National",null,"National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","Non_national","National","Non_national","National","National","National","National","National","National","National","Non_national","Non_national","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National",null,"National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","Non_national","National","National","Non_national","National","Non_national","National","National","National","National","Non_national","National","Non_national","Non_national","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","Non_national","Non_national","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","Non_national","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","Non_national","National","Non_national","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","Non_national","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","Non_national","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","Non_national","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","Non_national","National","National","National","National","National","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","National","National","National","National","Non_national","National","National","National","Non_national","Non_national","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","Non_national","National","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","National","Non_national","National","National","National","National","National","National","National","National","National","National","National","National","National","National","National","Non_national","Non_national","National","Non_national","National","National","National","National","National","National","National","Non_national","National","National","National","National","National","National","National","National","National"],"Numeracy_score":[197.03147,233.45845,286.23223,257.98386,173.51494,340.63604,297.33531,204.08047,199.69123,255.93877,231.29253,313.31605,257.17049,355.58683,237.29418,253.74056,277.74961,287.68197,299.97336,285.40754,253.80524,307.81891,206.05305,161.89142,222.60918,271.14036,314.81801,292.55192,268.12182,241.98739,205.79386,213.6569,218.84629,299.18467,221.2316,312.61005,189.81926,293.67644,185.45184,243.11505,261.93832,129.43954,232.1705,228.91936,231.42258,277.07703,189.87237,338.37713,303.99996,347.69256,227.85936,104.62494,365.54538,204.10801,267.07392,234.24614,271.42698,231.60234,314.92838,337.20677,183.31821,120.23276,260.51263,244.10504,341.24979,256.46254,184.254,272.89008,224.40041,102.25105,288.77577,277.53504,181.47424,266.14112,219.89002,233.12325,293.17293,231.57105,235.75735,263.02652,179.45978,282.82927,211.48565,331.5747,243.49998,253.62519,299.55661,269.50628,162.84757,308.18584,168.20434,215.51045,241.09464,258.2721,183.67457,64.1617,286.02091,188.74967,213.80523,324.51993,268.63631,300.48263,220.25831,199.09563,253.42104,229.83905,275.83844,259.1026,232.17476,277.41827,251.95958,206.8506,273.78674,283.05083,272.09857,231.47983,272.5967,302.00647,203.09672,321.39473,301.89639,238.75911,238.86691,346.5663,331.93333,228.63112,256.56654,212.29109,326.2028,215.7863,121.05491,238.48106,276.23297,270.24916,287.85277,264.29337,221.38347,280.84329,211.02273,245.81139,269.76612,245.99641,221.99708,204.60073,251.75632,224.17108,287.36381,172.39177,290.22167,182.52378,265.29457,291.40899,272.23107,323.25733,285.68649,262.65019,256.50958,270.0297,302.0013,286.48051,247.14843,278.58707,264.16265,289.82732,159.09532,309.45016,256.21821,308.27292,225.21315,238.65551,261.50393,222.58897,278.36305,208.18041,256.06026,163.94084,223.97367,258.34355,302.51592,299.01961,245.79642,265.18943,218.93567,331.19787,288.44499,226.07176,341.58406,258.19932,227.35057,312.39301,173.16762,266.50637,280.96874,246.18791,245.51693,266.30852,244.32999,155.38849,196.07727,254.22274,293.4749,288.52837,296.48063,239.96994,241.06474,197.55392,246.1534,225.15319,290.66235,343.17129,185.4296,303.83003,236.41929,294.88354,250.67242,207.57398,221.42907,166.21316,152.67838,297.334,181.57826,229.56721,242.96674,205.06645,198.06623,279.55716,217.91418,271.90993,325.29459,292.0568,307.39628,344.84367,213.99924,224.99132,236.7913,260.09484,180.99053,254.1297,258.94308,221.95272,240.65498,319.03571,242.73601,228.55502,180.59649,256.23257,284.5607,227.91014,211.84459,265.93053,320.35973,270.96227,306.36717,317.17468,240.48751,158.92191,270.62254,208.75273,226.45717,281.73552,259.02727,278.16848,185.79361,266.96315,200.03909,188.83869,175.56536,298.87856,293.93665,238.45445,260.97385,242.10207,136.03056,207.92281,278.87135,289.99669,165.25459,247.46972,266.27259,281.9834,231.26473,215.59524,151.31285,219.48409,321.26248,281.57965,200.00148,108.92279,136.02002,263.39027,274.89833,289.246,292.37778,328.77543,278.79934,188.9191,235.71835,223.68068,297.86417,151.01149,299.04225,330.60949,279.24521,201.266,187.51991,138.59721,277.58049,276.51906,257.57912,188.72622,252.30503,231.87019,279.10489,218.75487,260.78217,192.10289,272.54645,243.92614,260.13512,222.04589,233.41899,195.90376,241.31737,232.84606,194.82392,319.59473,233.47867,262.611,216.44638,282.41698,236.97292,316.59244,228.66579,195.31848,236.01116,261.00573,262.9048,282.60171,267.49289,289.17137,346.094,279.84569,249.52957,272.8784,267.9016,204.64747,123.80001,215.44365,234.20836,314.28386,308.25051,239.64565,123.71132,199.71555,280.26213,289.1046,185.66045,243.17433,248.3219,204.14106,249.5761,220.2863,207.43517,292.45357,245.20781,230.98058,288.87439,262.3029,282.75341,348.23572,238.79716,264.73287,218.47619,252.09281,330.12746,198.27035,198.98681,197.39529,305.65889,208.3534,205.38695,209.15868,180.79373,298.05609,274.03674,248.10449,301.28457,251.55551,308.61485,256.41419,274.45797,204.70535,290.91865,128.31906,282.68927,201.53444,275.71597,271.9975,171.12871,293.92904,280.60987,295.95707,292.20434,296.09089,259.14687,325.36522,301.13569,239.93269,285.44016,314.95315,249.14984,200.18056,238.98606,191.40451,291.23879,230.48469,264.65103,325.45398,262.20796,225.58645,182.94487,289.14653,221.81845,289.44665,311.70225,272.6529,252.1763,230.87861,314.74894,308.82721,180.77747,218.35958,235.47151,210.29579,209.68812,330.6829,211.14576,253.6471,228.0327,258.58912,249.75653,201.83974,206.52088,235.38277,308.15797,248.78489,335.96298,172.52844,283.17211,255.7994,291.30932,271.37446,205.50167,288.99623,215.51594,234.03809,250.23007,195.56763,252.61476,231.051,298.11644,233.85554,248.89601,285.31749,180.77219,267.79469,288.32298,223.68288,251.26321,201.54987,251.79927,325.73281,255.43999,211.51948,248.49037,208.06683,223.14266,110.09906,196.74134,222.58381,256.78679,270.36932,244.99864,240.58808,308.66627,261.4846,279.87488,353.49185,252.43006,230.0599,262.47479,228.90301,276.00555,261.00328,323.52893,277.15297,284.41073,306.08902,300.69484,239.33598,244.54291,285.64823,205.41315,235.27111,210.67521,275.43912,218.67292,188.3651,248.86591,213.01917,265.17697,256.35747,264.7954,194.12883,235.72211,262.11285,264.1044,297.3123,266.88029,251.6297,235.52119,296.69653,148.64821,267.13963,303.99766,286.65133,97.68491,203.79453,269.50603,299.53873,267.92283,283.94381,284.61861,237.0521,213.97015,258.37984,253.52926,214.67213,210.7935,247.9465,225.13783,257.20229,329.17208,260.6184,191.61692,323.04349,250.22673,284.69655,322.44984,274.12754,227.91543,344.18449,326.47846,195.92131,284.96526,210.20698,264.03839,218.14119,291.93718,232.93376,230.01944,318.34633,252.78915,295.73461,177.12078,198.85402,310.99008,273.68122,267.60648,196.34344,305.4148,272.29931,220.39046,307.12534,174.75413,227.48362,255.14833,267.71835,245.98216,261.73134,219.28177,216.67089,194.87866,254.01349,317.28802,303.79907,197.86666,299.44966,294.62549,266.04733,259.84698,252.26114,246.19608,233.97039,332.48165,241.98849,223.07684,206.63521,206.18258,311.39797,280.43163,273.61455,318.99934,231.37114,212.51191,165.22103,235.36064,238.83064,168.96365,206.14577,298.19637,195.87411,162.44176,271.3031,287.62979,339.70577,295.51877,286.17489,316.36018,174.23787,227.42223,274.16126,226.30423,236.91725,159.00359,262.92367,288.40125,271.71254,331.48278,233.21575,193.0145,182.34203,258.70023,298.29571,272.80766,297.49944,128.91505,300.45878,220.4218,173.07186,316.89153,222.05883,250.9952,255.44206,222.26811,303.51756,290.85552,211.70596,219.4883,150.09872,129.31132,210.70293,252.03209,256.58236,265.6382,331.15111,143.00812,227.10699,160.20278,279.73672,214.99367,264.15268,304.01105,279.15136,207.25849,263.75642,369.20921,270.8387,247.64094,248.38291,218.3733,285.77686,261.02527,307.02771,279.63341,235.93041,296.62952,256.59372,278.85933,315.31145,151.02522,226.64109,271.10518,295.093,326.17745,337.73149,210.76478,202.89146,253.76127,248.69188,219.43584,275.00934,218.80456,205.60219,268.58718,295.3807,145.95751,272.97458,331.40686,298.91737,244.36882,237.0263,269.45558,270.62242,300.65377,294.59142,217.60951,267.66055,295.9223,278.07135,233.4425,284.90369,282.55019,234.88315,213.13429,193.37816,312.40606,199.70976,251.21337,312.492,308.56798,278.99442,308.68587,247.42193,241.44083,237.80572,370.51322,280.74586,246.61201,281.49725,279.4949,299.02418,233.782,278.892,265.04229,274.40243,219.52465,247.53294,301.44896,219.80029,299.97456,274.51979,329.07319,292.22824,246.47391,179.73175,238.88499,243.05974,202.45143,242.96574,225.36421,204.93784,339.45764,197.45739,265.76554,303.90658,224.6102,307.5313,214.35134,221.51817,278.94858,191.26657,217.09521,227.65409,250.56616,183.22576,255.3052,274.08476,279.30589,265.34273,254.58515,198.16552,239.22483,249.55137,286.34521,280.10939,162.58765,258.37431,253.94374,119.62205,200.54665,242.16917,275.84541,241.36282,263.51198,277.2813,330.25268,305.94936,254.21655,233.20697,204.91392,236.46138,151.42547,308.12263,270.50109,297.76265,205.64328,198.03422,310.64774,302.08828,230.05106,142.96315,254.65952,175.40826,221.25498,293.9923,284.5019,295.76312,317.41392,301.59281,206.79258,235.73571,299.85758,299.63469,176.37463,206.69641,236.63796,228.14565,191.24446,291.67539,258.7328,266.34611,294.56486,225.9233,221.30366,251.44105,202.3538,339.43821,283.29847,316.54788,353.12993,190.82786,325.11425,158.07935,240.04132,318.6737,234.24951,296.01375,281.72058,295.10509,274.29773,286.70123,289.81829,248.2169,216.15082,141.98672,236.30802,177.15111,267.04996,90.57605,253.93536,255.757,240.85647,229.79042,241.46848,189.95248,280.03623,240.66394,293.40887,227.05551,282.19581,201.19252,165.05261,297.01545,228.93247,194.21325,221.57798,253.51668,228.60079,316.27325,276.63877,169.96474,264.91823,265.38217,253.07835,214.60004,278.34474,231.95797,294.56231,213.43795,198.65479,160.01543,267.20332,285.17484,245.08136,293.54301,143.02193,268.56463,237.09145,299.16415,261.58672,232.85173,181.12912,229.82202,217.59728,220.82892,325.32819,282.35204,321.46137,201.29135,262.682,254.59375,297.45736,217.36064,295.86466,343.86369,287.74556,288.57785,314.60782,272.3677,264.039,215.31569,243.86057,302.38222,206.20247,243.50516,118.61919,69.70996,205.37951,229.30947,248.58689,269.48609,210.0209,328.07854,241.37785,292.91117,149.18104,279.02983,297.32795,233.48654,273.28235,228.94864,180.47444,260.82938,249.34144,215.7485,273.67005,247.25635,224.70525,237.29836,260.53254,210.11811,322.51388,290.71242,290.41827,286.96785,243.91373,166.44934,305.22501,303.53238,296.9114,187.71403,265.71404,266.09673,246.01844,339.14328,283.45219,317.76667,272.87297,260.34042,284.28929,237.66582,241.92353,284.69251,281.21437,288.63763,272.51209,244.87125,146.07428,248.08087,232.76914,259.25151,242.31194,262.32685,272.28413,302.59795,199.70263,301.04971,209.73358,315.79981,277.11936,272.75292,145.50771,293.60742,249.96481,226.8675,300.46919,285.04605,275.96661,323.0321,200.23412,287.28226,283.17589,268.90181,300.84698,260.76395,282.17382,216.21953,258.81523,271.34185,271.44326,257.39511,246.05173,253.0428,238.70351,306.69999,262.42626,226.68415,205.33647,279.18675,219.97948,207.35159,253.65816,272.21524,328.50305,299.71431,302.08975,301.97281,282.66439,247.50852,246.82687,276.64919,293.21662,268.87457,244.31399,340.7248,281.88093,274.81445,255.48904,275.32423,273.6589,240.96716,288.59514,250.28636,231.55232,316.31235,286.4809,244.3106,235.85863,253.08739,180.44431,178.56828,285.68994,243.14679,181.09726,285.14676,318.00348,212.75289,243.02677,243.46031,193.924,209.57524,303.80426,319.65221,282.42124,202.45491,295.17627,171.91844,239.8282,189.30942,356.17873,315.96442,251.03326,237.70149,233.42538,261.78133,207.3045,277.48073,180.30227,301.25065,245.10058,244.27906,292.91184,220.92739,333.97826,254.42823,264.49734,264.27417,110.07717,248.5564,249.15387,186.94377,224.02433,238.09151,307.22418,276.85131,250.7512,227.2728,276.88948,224.85307,244.81365,249.92063,129.97883,321.12481,248.81362,218.8448,234.75652,287.96374,333.73035,299.63627,322.5649,236.04476,264.78538,103.55491,219.88771,295.57957,209.91779,238.14527,158.88302,225.28134,304.62146,211.87432,255.24794,219.10761,304.9078,302.04014,290.33033,219.20584,157.8134,278.26502,273.19446,295.08686,254.00096,294.23282,309.12822,258.14392,236.61743,203.26026,260.25238,235.8951,284.50038,222.52497,195.52478,285.14683,209.03726,218.96223,317.39968,300.36337,267.34249,243.25688,241.68777,213.04046,244.28265,253.23116,301.95465,279.16659,239.71804,277.80391,232.28964,149.22781,277.23957,277.3248,286.15623,250.17093,106.03632,228.08644,298.73248,309.73892,304.38854,278.69969,265.19914,136.57379,304.06639,223.65883,226.00563,301.89169,257.71546,303.55748,240.02243,236.31203,242.45662,123.5379,261.80987,298.38835,323.35887,319.33987,184.20001,104.01253,230.26877,291.36175,271.15405,322.96094,262.651,249.97992,286.18644,286.21722,253.25729,234.06134,272.97397,299.60636,205.52235,268.48617,208.34785,194.56549,299.2711,224.94913,281.08521,282.00981,327.10333,296.74185,228.38046,136.98811,332.52731,230.04818,265.53192,293.553,283.08436,256.79804,231.19845,267.73603,280.65066,271.21711,247.16484,259.24796,277.72566,268.94007,212.5393,130.17445,251.60876,186.32946,211.77006,237.906,274.35003,218.48734,311.91968,268.22286,189.09474,276.1018,281.15245,281.75872,278.64791,243.09985,279.29287,299.71874,262.78287,148.41741,302.88549,193.50047,169.01497,212.80251,266.06487,330.77333,249.33032,235.71285,249.41007,296.26311,280.06209,264.44655,288.9879,250.98314,295.46176,224.22649,282.55746,290.52228,277.03266,279.20806,269.11998,278.39873,254.05168,131.99023,226.14274,232.87834,188.33363,334.90845,288.72056,308.41469,217.12221,191.64436,203.83587,250.22487,259.62464,272.55685,220.4146,282.50263,182.29171,238.69494,121.04518,291.45806,273.93465,226.82441,209.32054,216.96371,316.24884,221.54794,192.1849,101.94363,272.35628,188.21755,257.80823,216.90703,247.38039,164.79409,243.72533,257.30178,257.07201,235.21736,297.28446,282.92427,316.61849,333.26725,306.33012,327.66966,207.75384,276.19194,209.06027,261.89176,221.46062,200.01868,213.15168,333.54109,311.19615,140.46833,265.7028,171.33375,259.10835,324.57561,234.84711,257.72209,152.42703,264.45259,288.92945,289.79045,260.44437,302.88873,193.78337,222.57358,306.0556,275.52252,329.45544,195.96643,290.83991,277.74486,222.49675,263.27728,319.10462,304.32293,303.55142,286.66781,290.65565,299.6676,231.14189,277.78623,294.03911,258.74613,292.29278,287.01858,258.11778,312.05909,243.89693,231.33531,324.59327,226.45928,240.4107,227.32431,275.7058,158.5292,285.52965,263.5986,214.7942,325.48436,196.48989,233.0039,196.73175,284.76625,269.09955,159.20063,281.03176,261.23461,153.27329,286.81179,231.58343,259.00909,314.20651,243.39382,305.40284,234.2252,184.05206,210.17082,292.85834,281.07309,215.21903,261.32603,295.51356,238.6169,264.18022,288.19889,227.36564,305.91521,301.32355,318.79143,288.27219,242.98792,221.80827,300.34817,192.97908,131.23173,90.35356,276.46821,266.39168,268.68892,287.42071,228.56865,286.41437,138.69639,331.69028,276.25704,223.82557,311.00008,256.23233,229.76472,148.04401,221.37427,296.24802,318.93947,286.75546,249.23405,309.54136,284.91067,250.91583,286.44429,337.79276,212.63473,225.34001,216.21097,202.49174,304.03428,247.94827,320.63985,301.89412,216.25181,235.44694,253.332,224.94228,325.65626,277.7837,243.93088,241.40376,243.65527,205.22569,230.3714,183.0705,272.12497,274.169,297.57096,301.29631,261.47406,208.01714,219.37012,207.72756,221.36501,232.015,288.21096,316.365,253.93476,224.53681,245.23346,275.72371,146.95109,256.16689,247.98178,219.86525,237.58578,325.16619,303.30374,214.46989,267.66149,208.54361,272.61771,234.48654,395.9043,192.80665,278.71468,288.53293,324.621,273.20364,91.69556,239.8793,289.30122,239.25768,168.85606,288.57188,253.95359,290.03712,257.77338,227.49047,275.71223,260.80309,79.15697,63.6659,256.33938,248.06325,313.58232,173.61988,233.65947,158.12157,277.06923,214.33797,208.09447,202.70099,193.78486,264.69291,328.15138,237.84965,278.11405,283.81792,230.32865,289.75349,319.66859,230.93333,207.06347,327.20385,242.6017,282.10022,238.07251,292.96863,305.95475,279.33033,274.23749,200.51082,255.1519,262.88015,320.67801,140.89482,232.641,279.33146,234.39809,206.59549,250.60632,229.59577,270.39611,304.08407,172.84701,173.56988,216.89787,242.65382,272.7842,250.32919,285.50237,146.69005,283.42558,156.10355,191.03565,265.6099,225.64468,177.27333,277.57125,294.06302,266.30816,226.25254,246.16367,237.58242,211.48276,270.56324,292.06316,230.23939,303.40804,272.72857,250.04694,269.8486,236.37335,360.49304,270.39018,269.15173,268.2867,217.93363,339.73491,263.76936,236.3641,137.63086,255.32964,245.09599,291.7148,253.09669,299.10148,228.17965,298.78866,281.75458,257.92928,249.38012,207.46617,257.84737,242.86979,293.5448,214.65034,278.0833,288.18739,231.8047,338.14335,258.71554,253.43979,368.70337,221.16311,293.23489,205.09012,233.14623,245.58565,309.02096,283.21658,268.16119,343.30679,261.50003,252.96142,302.02724,225.79555,254.83457,270.45932,202.90038,305.60351,317.91386,356.44001,262.45716,303.92618,158.51019,320.50713,228.82424,299.52324,268.88905,265.28406,232.03214,238.90335,273.25041,273.55971,200.86974,255.58376,232.07119,206.58899,260.20856,307.18698,206.52564,318.99054,255.77793,246.79069,240.20859,226.08298,294.68769,307.45158,270.59407,243.71217,193.64896,215.3646,250.30775,252.89689,238.04542,279.94519,206.71401,318.14905,260.88591,297.18729,293.51203,255.35423,226.17588,205.15131,321.34816,266.19389,187.43412,294.42539,326.75546,259.59943,269.23584,260.5455,215.23539,343.66535,164.50515,300.10461,285.52804,198.70614,227.01125,341.67492,316.59345,246.84298,202.44654,222.5692,255.02468,263.37276,262.05211,254.6724,325.19077,224.48041,313.21754,274.473,261.90813,341.93214,213.87292,247.99181,263.38345,309.29953,288.82068,279.10338,301.01255,288.04023,240.79677,217.16967,314.59275,241.15061,236.5721,198.02878,344.7011,251.53908,157.09204,238.37891,264.40296,209.26993,246.18168,298.03531,266.86399,255.78486,292.78329,185.64592,265.99421,284.08596,297.09842,285.29154,264.75215,330.99742,167.74344,176.20124,300.17888,259.00674,240.18324,132.23733,350.58929,252.9101,244.34707,252.2798,248.72965,319.73504,255.85652,217.25563,291.48821,258.10234,244.31341,194.53623,283.83157,282.26768,238.07118,262.41869,206.00853,288.04481,336.76031,308.93427,269.00098,181.71708,165.30312,220.55224,310.00851,198.27599,122.62001,118.87504,283.9666,208.91502,226.00072,241.66665,335.44733,323.10231,173.85142,227.54017,181.40015,248.31721,261.70182,246.19705,223.02145,215.15237,301.75761,256.20817,235.70617,259.14708,265.81861,267.6347,291.94792,291.51477,205.61289,229.54892,213.89955,135.89764,191.94628,290.51165,327.86683,316.18937,249.13868,269.56971,327.43058,308.49981,318.61172,321.65712,193.75259,301.06424,265.18129,301.19198,313.08093,282.02023,211.37259,220.22864,255.39158,264.04526,269.2198,224.52124,339.54177,233.40589,308.25549,269.00674,219.07758,128.98832,315.77335,249.29584,277.17312,298.59262,278.76378,338.65723,284.73292,194.24704,291.33969,201.27157,229.08024,286.74988,211.86233,182.72408,238.83811,246.4023,293.59931,274.59081,242.3262,228.9655,364.18509,279.81188,248.27091,241.15841,246.89072,251.96797,335.71312,249.17136,256.78728,293.50402,222.85025,303.22308,209.71033,245.91511,318.17988,243.5964,244.04318,221.06188,305.05574,299.93677,308.61679,177.90317,295.88623,128.2454,292.34941,233.16397,235.57793,304.98775,242.87558,147.75764,310.13938,290.9311,266.52459,283.16576,220.46181,306.045,250.75493,290.36374,221.76386,298.25836,266.85046,241.28314,198.11375,280.47085,227.10718,286.79478,259.22487,201.28077,278.83522,236.99629,256.3888,217.75241,313.54404,248.48041,339.43854,295.86687,201.38864,285.75698,228.70604,266.31018,261.28833,224.16964,305.04899,266.34344,300.7629,291.79228,333.77647,280.86187,314.84337,291.66767,285.53377,228.4173,230.66973,152.61882,319.47706,203.39662,234.41092,223.79589,249.49274,348.51762,310.85874,323.42108,194.15227,291.18814,248.87794,268.85161,243.68731,344.35834,257.84964,180.27936,263.88204,244.47665,247.62832,226.04242,274.15337,296.7527,297.31734,297.82193,305.17209,204.79272,230.35509,241.38739,327.54272,162.96973,245.75298,310.40499,229.42251,210.10666,318.16645,315.10849,201.79506,204.40183,126.6535,255.33288,289.92848,231.275,285.45455,191.42157,232.85068,332.92263,295.35739,260.26086,259.08695,286.5466,175.76355,255.9373,201.6362,289.1257,249.98274,232.90862,286.65579,242.12099,300.17803,275.71575,242.73737,310.44745,268.82198,117.80116,288.55339,239.26018,279.94289,232.10804,295.91904,307.31578,244.32131,276.67485,219.91888,222.5016,227.63804,315.44913,263.38125,285.34312,233.66947,284.64759,190.83194,212.97583,312.51942,264.76187,294.39066,287.50385,282.06383,304.83204,227.96877,274.42983,276.71761,177.97648,238.9484,240.71373,247.41167,175.53505,315.18068,196.94996,315.46862,183.54304,281.39784,297.28591,208.75835,267.22963,213.85931,328.21111,261.03785,225.31599,235.22883,170.304,234.6257,225.63552,311.72424,263.43972,213.65374,213.30508,318.59473,332.798,155.72352,156.22349,242.60267,305.67373,256.44206,328.10295,278.48232,259.42766,291.6162,268.92709,268.49025,240.25936,317.57848,283.51034,336.89438,213.60666,285.33034,259.37244,300.13004,318.78717,285.76215,318.9519,347.46177,293.68267,252.08622,325.07986,280.87648,314.39144,353.12869,247.3248,235.61573,258.0028,315.71508,242.5397,112.66125,223.91406,336.64537,144.33047,172.47511,301.03062,303.22705,303.4833,204.11109,310.75037,319.51023,199.87049,234.62146,220.67272,267.81896,243.76254,216.85884,284.77499,162.14968,112.48014,326.17258,343.72001,271.49801,383.65922,249.2388,304.18288,297.15156,240.51416,168.28874,279.81769,322.98004,181.56973,230.94267,248.14435,299.21796,292.0859,273.78169,287.58242,323.8136,327.25023,219.35658,249.85014,305.07448,315.54072,253.99346,323.60816,269.8772,327.25088,224.76832,276.16153,291.32244,359.20602,283.05141,238.85843,317.79433,297.48489,304.98843,235.08203,359.26492,241.36096,228.97285,298.02249,282.74739,254.56472,163.6612,213.26796,324.62388,217.45856,318.66838,306.17193,257.10512,241.35445,257.49636,349.7079,341.25508,247.56539,291.23217,235.40575,233.42764,265.00673,275.71722,315.10073,279.73176,279.20853,259.24226,255.86376,359.36428,332.81959,218.26377,139.43406,210.55945,245.34066,284.80456,193.80117,275.48869,393.54258,336.36599,190.42369,212.59883,269.11901,296.98025,326.94239,153.84279,280.72772,266.24765,305.65903,353.91631,223.31277,277.71023,313.38758,310.21586,239.11627,275.38749,278.36422,195.44822,224.57326,219.26512,225.84608,243.97542,309.03786,332.3439,166.2512,303.24199,175.60245,323.7097,216.09865,230.15554,344.71475,213.85684,207.3776,155.7153,221.85271,215.09012,242.0214,186.66755,344.11084,245.93139,209.0021,192.01575,320.64601,291.29889,305.01075,314.2823,272.43213,170.39476,217.04247,222.90951,341.59249,280.66815,240.44373,341.84397,287.21549,269.22382,291.33358,223.43293,303.95168,243.13081,184.69431,205.87692,274.00479,234.69152,184.72387,223.26876,283.7595,273.46634,93.73367,249.89396,259.47678,133.97469,306.22129,237.74206,209.05365,356.42549,null,375.99259,119.46181,241.26206,324.95405,306.62696,320.67587,312.62349,231.6774,244.21598,311.86679,275.67235,222.03773,244.99376,271.39411,288.25262,305.14517,265.38713,241.0138,244.39068,285.44258,154.77259,284.20556,284.06083,334.17581,292.57459,265.74345,279.0839,229.58226,258.88937,224.68456,311.08842,244.80117,314.91498,307.87773,339.42117,220.6091,228.37034,284.17543,242.91116,304.27284,293.22776,231.80592,291.31459,302.09492,287.73088,241.65471,273.51434,266.47591,109.22973,239.4323,223.34002,111.57676,299.32833,329.26743,251.24291,280.01077,228.85104,283.63899,267.74986,263.13828,311.79567,299.58017,54.66627,292.01022,271.07052,253.29036,281.65708,252.01689,299.32998,265.16054,285.26091,284.71543,267.09709,137.66373,274.35093,214.00846,199.1162,153.05778,202.8767,189.29336,258.97384,216.46241,252.0066,328.30946,99.96102,305.89481,234.6648,339.76792,309.88109,207.97499,223.93299,314.7888,236.89974,294.4909,305.74662,216.67557,277.08149,240.63519,351.78062,288.86608,299.737,149.93623,231.49661,228.52804,315.6684,290.12873,310.47673,285.22463,236.70783,201.02136,302.23054,288.63162,321.91607,308.541,191.68979,257.78107,165.45116,278.15238,234.8572,288.60848,267.22265,95.46172,343.55961,243.5476,249.88128,283.41126,258.98985,299.37318,275.70605,274.37032,260.36696,182.57224,379.26678,278.97766,150.56044,273.99553,181.40665,328.45218,256.00274,320.75108,182.27837,122.12768,251.16212,244.8868,298.58821,278.40177,245.07904,375.62649,222.03488,311.05721,335.93725,336.23723,281.55496,299.1616,230.97646,280.96337,295.80672,287.34566,268.42803,284.95396,233.89971,229.63196,338.05077,307.02899,281.53786,303.28489,280.94168,242.96505,255.49861,207.62622,250.53604,299.01354,287.68979,225.83515,193.45762,353.16033,142.4808,181.43728,251.94146,253.11496,107.98721,238.31642,288.15012,338.83501,328.07053,267.72172,292.00148,321.3746,292.28218,357.96448,316.11385,279.68463,331.46332,225.99552,331.04492,225.85026,267.00811,238.74211,190.15873,309.97692,294.29196,274.23549,254.09164,354.17311,280.31957,270.13896,262.31464,315.20951,165.26261,329.43827,205.73362,232.20926,275.33782,220.49252,258.80773,301.33837,278.87885,285.15243,355.35723,293.94399,316.85547,316.56459,315.29139,333.87663,235.30029,210.24087,327.60769,323.50071,233.93516,226.7276,366.82102,257.73622,334.69866,204.47912,326.7071,225.71243,317.73538,342.16998,198.88752,276.91835,322.7201,191.73258,306.62842,225.19369,344.93909,204.79713,273.89229,304.63808,282.27229,276.45447,312.32653,235.79347,174.58078,262.83982,328.32649,305.14378,244.61453,210.45503,286.38701,349.93318,213.11228,278.81705,301.53344,134.60638,276.59972,281.86962,364.05991,223.74321,224.30511,263.3446,210.6208,354.75412,222.41646,235.21451,166.10038,328.16936,207.15563,339.09539,171.90635,302.40842,261.43745,311.20878,235.97118,154.12761,331.74821,271.18781,288.83157,301.13738,202.15139,286.71477,277.93829,310.10665,342.95936,321.24264,266.83766,263.76482,152.8765,283.51352,267.83645,336.01655,244.76373,240.0196,289.89108,258.41178,298.20751,180.69166,280.25201,245.49841,284.75483,212.3416,138.46057,324.30008,259.49779,289.01464,290.37194,243.4916,296.11912,266.53392,269.51896,101.08866,205.32822,316.83595,264.14447,221.03633,262.94794,376.99468,223.23572,199.73968,274.97694,285.01607,278.63699,313.09027,326.14284,316.37129,255.72144,271.48925,211.31375,243.11188,295.65963,221.82878,182.09609,283.24695,242.3052,279.01999,300.0475,264.58933,281.32041,244.32621,314.80674,267.81512,280.06734,277.98856,334.1086,165.37342,346.6955,261.31428,215.89244,181.03518,174.99616,220.98089,263.49658,132.46169,294.07365,235.25557,244.94715,210.39224,294.77989,308.0375,267.77684,233.379,250.5585,304.25256,318.33,304.43349,310.3013,286.94821,225.8416,277.77701,322.0101,181.86472,258.20027,292.55444,318.92563,86.32485,248.29445,150.09254,210.14422,240.82658,268.2495,230.97577,99.28856,275.802,182.58247,194.42761,282.85856,212.74313,292.17389,275.05783,294.93019,255.13905,320.45166,243.45265,285.90315,262.14723,312.27772,310.39351,288.57008,311.53344,232.00745,258.86615,195.32112,159.22015,262.73845,342.36257,310.12242,239.50353,273.58741,281.63464,265.83795,279.44939,243.09375,264.69771,217.60065,285.42594,350.15642,295.03907,365.2759,186.13312,259.93591,245.80246,231.1485,244.30229,264.35083,204.75474,274.13018,311.54278,310.1825,255.82944,274.67369,270.20299,347.43222,181.68877,227.49823,209.67646,255.66498,200.00947,239.92925,316.80939,201.69438,240.93263,210.50771,309.99406,220.45426,146.03969,245.8954,170.89313,239.295,223.38934,279.29662,208.49861,282.80804,292.38292,195.32236,337.20322,261.97105,237.00895,338.61419,87.14672,278.92293,291.00721,297.37286,313.89194,333.10552,304.0204,207.2582,246.29107,222.06006,247.16674,304.32706,338.56157,227.17038,310.22809,297.81758,258.81866,273.84419,172.06196,235.90113,309.60582,252.81636,243.60191,317.2027,267.5757,193.31394,209.42793,137.84362,295.91993,297.16422,272.72641,204.93368,275.8616,255.58493,344.93763,328.70734,259.13627,326.70731,260.26402,278.50035,292.2865,269.95121,332.04108,275.45349,258.14726,300.44092,210.41996,326.02023,343.43348,323.71722,292.42175,284.62793,186.1246,302.11615,351.36384,286.31172,321.21553,348.17308,296.39546,283.27066,193.01871,279.22512,193.12736,270.51526,228.71698,335.65231,230.9571,264.56557,254.56668,186.07186,323.42494,292.72755,271.30918,261.81462,249.05404,322.78008,245.64004,243.60928,291.37855,279.61369,331.97523,251.78117,327.72024,362.31562,180.28141,327.36755,235.34314,281.04259,247.52119,274.04485,311.4318,357.8377,339.66968,315.67611,163.56794,186.98758,252.26855,216.43574,259.0437,235.80443,264.26902,194.4687,214.31661,289.8386,259.47837,310.38351,225.84328,338.73945,237.17764,267.7248,222.51835,314.07404,242.57908,256.80482,295.31074,297.23428,355.7817,244.87375,263.52873,265.49606,263.79028,336.48841,249.88728,171.93001,327.99173,264.01505,316.65477,341.84712,265.08678,239.94577,308.59957,278.11456,419.18193,256.19162,275.87963,173.42046,259.30801,268.77644,243.78321,240.43335,206.15994,243.10717,240.49944,285.41812,200.90247,267.27817,300.46952,256.97621,312.27798,308.33069,300.44546,305.94095,211.63389,184.84744,243.45731,250.02236,275.83994,320.44012,281.79549,259.63046,304.24414,310.86148,219.94983,198.74097,138.31768,221.145,332.97552,185.44324,289.61617,228.60488,300.58219,241.43764,195.93386,111.50426,330.83964,324.27824,344.13353,282.38474,308.38399,264.68784,214.95222,160.89029,220.94136,330.83453,83.60766,221.30601,328.43427,199.17898,179.41764,289.13802,205.77608,175.92178,260.5629,202.41122,235.87109,361.99675,304.54167,188.96796,237.13461,220.97248,255.61647,259.5997,289.81024,180.92421,195.63078,276.29407,289.0184,329.87645,202.01693,298.56133,240.22354,194.38173,278.00176,334.55419,229.56377,287.71678,288.56148,251.74888,311.67819,249.27881,311.53213,147.26407,282.15849,175.11754,248.76734,306.20276,274.04997,307.19313,319.54041,178.93157,311.71061,261.68886,380.27296,249.02586,290.26983,189.41665,215.80066,223.28333,344.60571,315.56981,232.07308,225.18534,240.70162,352.9587,248.88514,285.77724,365.86517,151.39779,272.08738,267.31757,239.62355,353.51244,313.4374,144.31286,250.9583,337.98117,256.4665,204.42249,96.90738,271.56586,174.80721,317.8664,268.92838,299.38566,301.19575,254.30635,309.33873,246.62366,286.75646,315.79883,239.38525,209.11389,240.36733,276.87708,305.36013,310.06363,309.27973,241.89931,348.77269,261.9683,302.39524,200.17347,295.47453,144.93889,217.58273,254.15392,261.32038,285.98409,283.79649,244.46161,332.73428,304.99804,285.70483,224.77658,269.42899,259.60644,251.26576,235.12163,266.38056,335.03573,253.03637,215.54484,251.40867,332.16559,252.22153,248.98821,183.41909,287.98464,247.63414,324.1504,219.30821,302.44095,253.6745,314.7937,270.83511,156.20607,246.99074,330.60603,277.45785,380.84792,333.82396,348.78345,222.99556,239.6799,171.03338,226.58671,287.25918,222.22183,299.19649,225.37167,158.19135,247.87647,341.47888,248.07699,279.7749,225.00407,239.59115,222.30309,146.02889,212.34616,241.23974,318.07715,208.1402,286.54186,240.3626,238.17722,337.09205,311.108,207.17212,288.40684,251.90094,274.92378,181.51008,271.07875,225.93659,388.12701,266.85534,314.46981,214.37668,217.38092,234.64914,291.1688,255.10297,238.02759,287.87995,298.30794,296.22352,259.03506,251.83031,259.3982,178.48398,282.62919,174.90153,215.79177,216.57626,230.62778,311.2594,361.05016,274.0872,262.00805,236.93937,302.21689,275.94495,356.41693,275.00792,212.1737,180.13534,252.54899,213.34413,209.30463,257.94856,251.91486,264.82147,324.44662,283.32291,330.71803,259.84939,253.09595,231.60953,253.80408,197.17236,194.49648,242.2645,319.04649,296.157,285.3902,309.44232,151.08782,172.39626,254.66408,158.40662,292.54766,254.53083,230.7758,226.74696,262.98799,280.79485,354.96392,275.5314,296.14841,308.22048,282.16995,360.67455,358.78466,288.96176,265.8659,238.82849,236.49914,313.17681,242.3535,231.12996,218.06067,304.62692,238.97318,186.27159,273.12388,231.18589,311.00315,264.38825,274.60512,245.86791,341.01011,229.48668,348.80167,223.06887,247.09736,231.98241,178.67106,244.69418,275.85065,318.31721,260.50929,235.09148,340.1835,349.8276,269.64067,200.08384,235.03276,237.78851,370.6262,230.3045,270.12099,146.15949,250.3565,325.51141,357.98497,279.6521,327.60863,241.47866,203.32872,253.35609,279.04605,272.65739,284.82334,252.72001,320.63262,420.76629,251.25602,356.4009,174.5748,288.07511,316.80566,242.52832,281.56886,248.09804,332.58008,221.84296,241.77962,317.42451,345.33166,211.10652,319.47089,301.6475,311.45707,328.01959,292.93125,296.46401,244.91752,293.41886,246.36866,332.22455,204.12538,255.08196,219.17908,369.61828,93.71554,168.78844,264.34168,253.97805,287.85147,301.32165,311.89504,298.87779,269.69911,301.34254,248.73005,305.84818,308.02272,281.2865,291.22931,224.46149,270.06705,228.91211,224.74442,274.83461,230.77046,233.44937,276.67552,163.15614,263.17731,284.1559,237.74179,350.35594,230.15132,279.03793,196.64794,342.60918,347.00035,329.05937,254.40112,244.08385,228.06651,313.58083,232.09759,275.86223,318.14108,338.3761,254.20324,152.52445,310.03602,218.06026,148.10555,225.16854,204.84582,141.45293,252.16253,254.01653,210.95652,312.39178,246.92872,238.78211,220.90054,396.49815,329.73765,162.84787,198.95569,269.07122,284.55696,318.13212,280.95363,344.35787,195.94554,261.14153,316.45783,290.3026,205.1286,212.52215,375.10296,202.44891,303.68336,204.05578,172.89503,162.59944,251.68255,274.05948,252.09979,293.47328,374.7703,242.59204,296.15013,318.38199,229.71121,327.46597,266.74925,159.10927,294.9031,275.87317,273.46213,230.81418,268.97497,230.35776,320.05481,312.66856,294.07689,193.70795,127.73677,308.37698,347.25448,62.17967,306.25611,188.18173,310.56383,234.14165,229.9865,321.33995,313.12011,257.7789,238.53466,334.77246,203.32408,296.09428,316.35895,175.56869,254.08106,208.5588,294.05039,303.12188,233.91548,312.11558,127.58555,317.25523,155.81562,327.2258,273.50773,300.8996,271.00088,325.78484,309.37846,249.27594,84.43327,232.99969,202.00747,215.55699,172.45163,164.75116,254.59289,162.93596,246.15648,211.61741,317.14109,311.54978,237.61099,322.98905,117.34575,235.90326,172.86031,268.27389,212.29349,328.83512,236.16551,306.73394,243.18923,272.27173,220.6396,303.73496,191.65333,212.13466,184.85793,198.16097,223.42882,275.98486,226.52788,212.71066,345.95739,289.57281,203.59862,313.07872,265.36039,275.92402,132.35449,246.79648,282.00661,244.58299,213.1197,240.0446,329.06946,150.92795,361.3303,329.88319,264.69852,305.78248,266.34992,217.06243,266.03514,272.96056,187.33328,142.77805,284.63665,308.44008,250.12447,221.58565,328.36761,300.96831,248.93127,260.41228,330.34856,240.75341,291.84492,324.94502,342.10756,289.95359,283.07342,184.53182,216.06587,235.75401,278.75442,339.8255,267.13088,246.92365,288.95626,295.70808,220.13179,228.97033,172.99529,322.21419,273.89482,249.58202,290.36234,254.79995,312.49747,302.19762,177.72891,325.04347,262.07153,268.19801,269.55717,286.05962,278.1509,272.79965,261.99645,297.98783,247.5513,338.88789,344.42567,270.6415,278.86272,324.15528,325.16192,215.08033,330.01847,256.04254,270.68683,351.14888,280.73013,233.12541,260.85591,300.53184,359.10153,291.53796,317.99983,192.62571,330.65195,326.28655,196.26075,272.6642,237.70899,288.43216,361.87841,280.95352,261.44674,253.73722,377.31775,302.76413,188.92113,285.12178,197.10809,321.54755,241.44577,175.02563,259.51788,199.88728,112.18687,272.14474,279.93968,332.41861,249.48953,165.66974,322.08641,294.88306,298.4102,227.02005,353.96493,275.36249,241.28694,314.14756,266.87924,254.68784,336.76588,258.71947,144.42841,191.42274,258.43124,295.70055,310.06395,331.59259,176.88232,239.5597,205.02104,194.32089,231.40045,306.96602,345.59084,238.51897,363.00421,260.17122,242.67504,215.31557,216.313,223.67894,258.46009,259.2161,291.5768,181.71264,268.37928,310.80037,165.10988,232.71001,319.214,262.42537,290.99445,153.58505,356.10761,188.69171,273.61919,245.0278,291.92002,306.7946,307.88772,206.1584,180.75483,272.8192,364.20992,235.59119,392.69275,217.35815,326.6643,336.45172,285.77384,216.01399,213.80954,215.66071,236.54022,180.67356,218.92434,232.86627,299.01987,258.22276,293.78736,242.27037,331.36854,337.83916,243.69693,270.45434,249.90864,213.92982,287.33142,224.09194,239.18866,269.1246,322.45235,281.941,356.14261,241.22879,135.19029,322.43446,248.85962,262.92007,246.34889,288.954,298.1943,266.72277,226.2446,282.17142,224.44902,291.6562,304.89592,249.4668,250.82512,294.07913,208.58415,225.90636,290.54694,316.92362,182.30502,287.77687,290.21947,292.61279,299.56601,263.93367,295.19613,250.02027,263.18409,297.21276,284.11125,266.92971,205.48192,199.61858,227.91291,266.17516,245.09578,287.23754,232.04503,364.84914,179.48258,237.01258,243.28453,264.42221,248.87407,381.7374,229.63248,277.17529,255.73876,231.02233,288.06191,237.70317,262.68662,166.69352,219.8085,183.11208,179.17883,244.91673,290.6841,264.32418,315.82605,237.22883,226.16035,251.3353,325.77378,186.95964,352.94211,248.12419,168.90124,267.46995,269.37134,215.48455,112.87485,269.97861,249.10969,284.668,271.45744,244.61901,282.53926,313.53671,310.25491,239.18545,259.8642,222.36254,283.1108,197.65022,333.83548,205.87026,302.54313,295.42552,326.35398,317.63094,297.02077,197.17221,258.24293,291.26503,224.56209,230.66159,239.29427,236.07948,243.23102,290.50206,264.2707,224.33399,214.73516,139.64743,102.43736,334.5706,223.75302,299.18149,181.27913,323.87196,242.51405,299.52415,316.37158,230.3654,144.11964,231.88757,336.70573,242.54059,247.16969,278.83404,246.578,306.02728,361.60589,283.80851,220.78237,322.12935,307.59325,228.53548,316.43074,196.68234,263.61485,263.5549,158.3418,254.28596,328.08622,326.42979,306.29319,306.89173,301.93688,206.59496,295.9933,315.27194,265.0279,192.42681,257.55092,183.67125,283.63608,215.52242,240.57672,214.23584,291.63584,291.50101,221.5581,254.54544,321.3474,308.47203,237.06278,267.56326,199.08425,230.93627,235.20773,198.60782,276.11348,85.62927,283.1535,214.00566,262.75011,298.61638,291.27479,234.83232,153.41786,203.8334,279.07331,278.41527,169.44816,268.2219,218.05088,213.45676,282.6522,289.21786,318.66637,307.61795,233.0539,321.6384,270.52881,233.41754,257.70601,190.0121,250.81401,222.92118,301.86037,208.80974,245.12978,263.15772,266.63778,298.10213,192.24236,275.00826,185.19249,244.43789,247.63041,306.04779,279.15387,321.01461,305.19465,244.34546,244.57875,230.79844,269.96555,158.50043,211.98171,264.16686,189.55794,327.52162,250.41053,392.72003,200.1405,250.17716,216.02494,228.73865,230.9429,312.12856,284.02375,272.35009,287.35453,296.76227,231.80765,178.98422,238.01585,312.68083,319.84222,258.86569,269.66011,264.56184,288.23342,237.51021,355.10354,265.60877,223.15975,305.6033,241.92851,307.55698,319.99674,275.13945,170.65595,224.45702,253.86956,262.5515,290.72274,242.61503,301.34128,237.11226,296.98732,207.01733,182.65739,221.30824,246.22272,231.41741,189.88582,246.54673,238.00468,204.17186,286.42624,249.4039,225.59916,269.70117,260.14745,281.11185,309.08575,368.00186,376.3716,241.76663,239.9486,262.95936,281.06893,246.23041,247.36799,126.1348,249.75442,259.62629,284.32061,213.81241,320.0625,305.05431,277.57245,253.75053,251.40621,110.8538,256.05123,320.78465,215.90902,236.23815,209.72258,328.04014,306.6461,184.10433,308.79899,150.51046,203.52913,231.45099,205.45017,209.60688,169.5917,315.16016,165.28687,263.36052,403.32431,251.00711,276.12807,224.51185,327.04619,227.30628,359.05328,302.38046,276.22522,297.73297,305.82241,258.20489,314.83757,323.96464,207.16519,295.44638,141.50793,288.65193,191.43712,140.73548,272.21828,222.48831,332.32686,234.72519,260.23294,324.86349,363.31218,279.62382,333.28599,294.95092,304.25493,280.41668,216.97364,343.05896,224.93967,305.21483,225.79496,290.16006,258.20521,300.33242,265.73303,236.01819,215.21027,336.79807,278.08156,311.25536,238.20013,304.06488,234.67313,206.70268,243.81603,257.668,254.09723,208.16122,255.23836,270.34091,306.10387,247.28326,311.4442,217.85403,319.63623,262.87058,302.32094,333.04391,312.728,342.94804,229.21208,276.14681,261.74111,217.55875,237.59144,292.22406,271.05498,302.42317,240.031,307.02483,255.3771,286.28412,239.3342,334.40393,321.84707,141.02123,242.75318,313.51495,199.23546,167.64133,364.95126,208.71927,327.89581,297.22004,313.48685,278.64378,193.16057,316.84523,290.26803,302.91588,323.72125,150.73528,179.97578,229.16908,204.84942,201.89676,267.08092,366.93234,393.90568,246.52064,336.7587,260.52574,350.68644,285.71799,227.35288,299.25839,227.29063,303.93922,217.0379,247.48368,118.28097,275.18592,272.18571,219.22491,229.17726,235.57331,321.09637,235.62947,361.37204,236.7306,318.10248,278.66982,288.62483,317.92088,219.27379,269.67355,315.62437,231.05124,252.83078,239.66143,197.00184,242.06407,221.84157,335.5736,275.16496,243.86887,241.63883,294.40715,298.69234,307.12263,291.85407,261.59545,104.82525,192.66323,321.63984,191.93724,311.68918,257.29537,161.97015,294.58921,263.78393,256.96142,226.96894,282.16855,241.64597,331.29795,240.32175,149.59429,213.22096,297.62916,274.15572,245.93642,222.85245,289.45633,187.04402,312.19016,311.47085,265.13458,338.53537,193.2527,378.39274,329.2051,323.44441,294.33892,273.89957,332.71271,238.61161,323.51333,175.81114,297.6851,299.22425,303.12034,299.00048,305.67572,187.1856,253.23004,296.17727,321.93435,263.40135,284.69822,266.409,404.32259,215.80887,247.32115,242.43305,324.74438,275.25884,268.8201,176.60194,191.29011,262.68491,200.5949,300.89403,135.38085,341.96049,270.86849,285.07755,296.93165,218.34254,246.16182,354.90263,247.0486,234.66287,288.59259,182.5188,313.29719,281.39411,238.46198,257.56992,228.97457,264.5262,229.77568,273.72465,318.08815,312.38943,214.90327,275.20501,290.55766,345.92916,332.77197,315.79729,240.53235,245.97898,372.7966,243.73887,322.46265,152.95604,192.04198,230.12111,285.45227,218.7963,283.98813,214.93089,317.72977,257.08507,209.94679,217.90425,336.79908,218.93378,216.94947,113.67269,261.91546,292.72339,259.8317,68.36629,216.88335,192.91085,309.33874,256.89847,241.80646,279.88013,233.65108,244.65132,251.53264,236.91896,338.05164,296.12989,289.48195,310.98481,204.05266,246.10183,287.75522,245.12891,243.22992,232.25897,247.14823,299.14241,247.80469,250.26415,277.3337,249.42009,212.34027,275.59067,258.93172,268.65811,313.99545,311.94788,304.29686,242.43116,239.59864,354.00374,198.75871,198.60487,276.50643,269.75761,307.41773,204.19501,217.67197,242.26651,199.20825,255.53158,323.52802,288.77064,314.64022,260.70899,191.74313,280.89727,261.55957,218.7933,289.29423,331.01876,283.09709,279.98366,248.27671,308.79667,249.83304,244.73716,260.06817,229.52508,321.06093,321.94197,275.69481,207.38706,202.25688,244.36146,329.60423,285.58973,276.54225,222.02965,252.13648,213.76234,281.7237,207.12614,247.98372,243.45488,184.58418,328.22291,272.15624,162.62116,227.16201,354.60212,115.38375,192.04213,216.49715,308.8796,297.93475,311.67119,239.15344,119.1534,199.66428,168.67369,196.59975,257.20953,361.01778,273.97432,298.46103,331.40397,203.62152,270.72546,197.73717,212.75434,236.75422,290.19768,232.02293,303.30119,179.18554,265.53212,309.60467,249.13892,318.45962,260.99571,307.19435,261.20179,375.32224,40.52129,204.93898,286.84792,279.04359,282.09722,306.23038,206.99864,250.5346,218.79242,186.1183,262.2062,299.19894,267.53917,278.64363,291.63496,224.1786,311.59761,246.81467,277.43676,279.21297,256.35379,269.21794,319.64071,280.27938,179.66439,241.5267,293.28214,233.06721,255.52852,298.83637,314.05189,307.95271,150.08903,398.32278,263.52769,193.27638,329.63183,264.55368,300.03472,178.3757,296.96128,286.49133,287.25843,323.05777,239.94921,321.24289,277.63771,164.90917,306.87165,222.26609,232.59386,214.1881,317.61769,241.09649,333.75367,314.00674,356.83354,288.66519,288.60331,268.94017,233.17242,255.47734,130.18481,315.54174,291.0164,291.07318,304.47291,145.88893,186.00418,262.51622,329.20879,248.30879,300.57555,160.32142,256.0035,219.90669,289.68375,257.60397,292.28885,313.3448,304.35733,245.47277,256.08231,281.21072,324.98021,265.92968,329.9871,252.4131,295.79889,296.48092,317.57603,332.92448,315.70807,297.88756,235.66985,315.22451,254.90796,333.70065,313.97806,319.45303,201.962,285.7841,306.7252,305.77681,227.85229,258.34207,241.76741,279.71262,210.17028,339.17312,287.40013,246.47605,359.0901,354.82055,202.93976,250.23626,262.2852,240.80756,276.64539,199.46558,354.98077,158.23222,268.0626,303.38281,297.56502,305.80771,185.33647,300.75112,331.73538,302.73199,311.00053,307.48305,236.39364,268.23906,302.14247,166.48943,293.42632,188.41592,334.78447,273.10954,336.3113,160.86054,269.80324,207.6329,286.7073,297.42836,219.34056,262.89725,167.48513,246.43219,334.80714,267.8486,197.18566,273.19783,195.15606,222.84942,310.95335,263.39896,116.26928,279.96038,133.81053,271.39428,238.8154,282.6013,290.54065,251.24729,177.44511,360.10958,259.5338,307.76504,235.56625,308.20457,279.35554,188.22535,159.14409,265.14658,268.97321,248.53093,192.02163,270.53154,222.1901,135.01143,278.81974,239.45497,331.11226,213.05415,306.35495,221.6406,261.13941,214.82588,300.42585,276.11535,277.06738,309.40683,177.62639,299.17746,273.44003,351.48915,109.84136,323.83666,334.77443,263.85627,187.60501,305.72691,240.33325,285.10843,208.58172,232.17049,328.73818,229.01742,292.62133,328.24064,246.12163,315.77824,255.04776,196.66019,243.05636,247.06475,172.40846,346.75992,270.58567,212.50958,252.68013,204.17289,273.76576,264.96975,214.65969,231.42884,245.53636,85.40325,307.55448,234.40315,245.51479,252.10219,186.48448,151.23606,274.96913,366.26343,218.21227,343.99834,259.36373,290.39065,241.17175,271.69244,345.46074,280.67265,178.82639,195.43238,187.43016,226.97555,315.25136,181.35399,329.26493,332.74594,274.18648,234.86563,288.15239,191.861,278.79674,327.92008,363.39277,118.51959,300.82841,333.74866,300.57481,256.14955,290.73613,208.46669,340.22422,289.02545,218.44229,270.18264,251.989,307.3021,307.09361,250.69612,270.69043,248.01855,144.97484,300.6421,236.04878,305.70392,245.04999,246.93347,140.0702,211.30692,296.70989,220.77367,266.03226,272.02259,223.70506,366.52209,343.0128,288.19465,278.96228,320.40187,263.06416,262.95044,276.21679,281.17702,331.03875,201.51331,268.39769,266.42272,280.62919,260.91792,317.54375,350.32036,237.90016,260.72929,232.95735,236.62028,283.32367,323.00216,212.26104,253.53662,287.202,257.74967,225.82265,214.30213,231.92993,198.56496,224.28034,324.65129,257.46122,296.5011,295.47497,201.07238,282.70242,189.72277,318.19803,264.25009,289.29521,264.68079,245.02451,234.72527,288.65808,179.5253,305.23306,222.42867,336.73956,358.12316,287.83791,257.68462,260.0455,226.21385,266.53763,313.31157,232.20355,309.51349,383.53856,241.26934,191.63426,309.06476,243.1648,238.68334,326.48172,296.81577,321.547,320.12132,271.29596,324.99863,232.72425,285.41854,253.45775,278.1206,198.81978,244.31407,283.61277,207.92389,266.63286,252.93877,244.8401,321.38985,140.19288,341.82786,196.134,260.51498,365.81062,236.47913,355.22977,234.92727,331.18981,239.20254,232.20256,250.71236,234.26468,244.55931,300.91694,305.04177,294.55145,214.50452,229.53846,301.99887,305.02051,301.49065,423.875,309.50382,312.54304,259.88192,267.37075,223.32284,173.33496,215.68583,340.07029,228.39263,283.62773,265.5433,285.78619,122.28946,304.72718,283.90665,260.88294,313.3374,220.52192,268.36463,129.01293,267.25305,244.80772,214.48881,278.32296,242.1557,265.599,210.28512,247.26101,243.11253,350.06461,311.78616,247.83436,275.40197,258.63895,202.36659,272.37506,238.03897,151.23742,187.38524,215.67824,326.58428,216.03169,278.60856,228.1693,284.93584,285.08332,290.10547,167.20989,355.41103,291.89086,241.95552,160.87288,317.56464,289.00831,353.21788,340.68172,234.17519,293.64156,289.45833,264.14172,273.88086,335.66987,260.09333,203.66964,245.75834,342.10403,309.49534,259.95345,285.85524,276.33156,287.63116,234.93238,293.99673,324.03292,170.19145,254.11528,200.8509,278.84463,226.35351,298.12994,263.33406,304.78276,263.03864,217.16366,191.26136,314.60724,225.89272,177.12232,317.45264,271.73916,295.80006,235.19746,316.87011,228.335,293.62585,143.94294,287.9828,335.44144,251.09416,281.75314,106.41647,247.88229,277.87547,143.42341,220.41229,209.53613,326.46352,297.2269,237.79681,288.76544,241.04537,280.32181,210.06041,220.00536,221.18598,300.42046,287.45196,265.45398,345.07378,288.20823,266.51171,251.30161,193.02836,246.57565,209.78471,236.58998,280.68732,304.11203,267.68691,273.63288,248.92274,343.89474,269.8728,261.88434,266.45708,215.6999,295.45649,262.08871,280.93002,247.3578,275.11006,268.12461,183.3009,250.49716,324.41828,344.11473,159.35748,253.84438,182.11459,201.2493,229.25064,222.56126,308.08527,312.66867,306.49107,263.78835,262.68643,271.69365,269.94704,203.68838,291.58013,268.2428,251.5607,327.07597,200.7795,232.09455,262.60852,280.11522,237.74562,255.46997,161.9614,296.48893,295.56446,285.47799,134.45918,299.38777,341.84036,237.8584,361.77732,305.48979,317.85977,244.45047,347.20591,339.50928,217.74649,271.56688,338.19679,317.64196,187.22039,307.55785,179.71312,289.19524,199.04249,325.5767,261.61236,null,279.47138,273.6999,178.73936,351.15223,300.7309,335.51994,245.3674,278.34323,300.83369,282.18406,278.99918,274.92245,280.23515,274.40702,266.85849,334.49193,259.9043,261.38642,265.46739,239.27848,277.71682,276.05239,304.08804,305.72746,144.35921,196.36241,275.2006,274.32517,207.33721,335.51162,140.62054,345.93132,237.22809,330.40071,249.08129,343.57056,164.66352,249.38774,251.04601,286.73935,222.51545,317.24333,292.46833,272.58339,223.5775,270.41564,322.67156,255.48757,242.30685,337.97596,271.64811,169.26295,258.46154,300.85297,277.51806,374.72475,266.24906,308.74629,224.54852,205.10368,219.68459,246.1478,254.36496,328.91872,285.10683,213.56838,142.2707,238.25551,301.14191,156.84678,278.5686,314.30128,304.15471,303.88664,329.46839,359.85504,262.08346,283.72307,279.72826,322.68532,260.0825,300.15445,257.93251,247.85543,300.50595,347.24167,289.5303,249.94923,250.48378,297.28827,219.27244,334.31568,260.26791,289.95056,264.08502,193.464,190.51974,305.26791,224.38881,265.24404,183.77745,267.77066,379.63004,245.72715,212.87943,306.34164,293.30302,283.18421,152.04627,186.25668,354.94979,313.51832,212.61573,257.60624,276.6931,146.03979,319.94427,276.25474,327.77545,244.28581,354.91732,299.96251,84.95899,196.53846,304.92841,263.53706,318.41279,112.90423,310.89952,304.86232,311.25601,320.11568,226.96814,278.32658,267.7711,261.38868,146.60403,160.65974,311.44269,227.09855,361.13602,349.6139,221.00257,267.2729,274.01085,323.32599,265.7437,297.39761,222.77863,281.53462,331.32279,264.77336,260.99478,201.61615,260.70285,294.44978,295.95971,279.4564,353.62356,300.26224,253.00468,277.57315,280.84342,194.18552,300.72191,272.5559,328.09268,332.42307,123.74037,206.27351,198.38914,264.90806,198.4623,234.9117,325.37779,196.84648,232.12648,252.70974,301.89497,284.63456,235.86684,248.95389,278.25538,326.32029,163.03728,302.90148,281.15786,215.38084,356.25016,254.89343,231.82348,172.41415,239.35243,341.70073,329.4753,298.34138,140.91313,293.66317,229.18308,178.15723,397.83437,232.22158,218.64019,260.87099,294.97945,273.18839,304.2661,285.92296,321.93396,205.72247,282.75384,342.84317,268.08328,265.98312,337.23254,84.396,298.82129,247.93167,273.75527,311.34856,225.13343,290.61829,325.40821,342.09263,292.1385,205.97865,218.33597,237.65207,323.13033,271.22069,249.58683,252.56535,265.32181,239.02946,205.58991,309.5716,206.02801,249.39425,266.93968,265.08573,245.75003,304.66969,336.10991,306.73393,234.13833,207.47156,261.45323,214.15738,231.57879,318.97271,215.05711,210.58638,258.46685,306.77315,318.66973,276.11938,378.98445,259.58184,306.35558,158.57802,183.11755,235.02138,281.24648,238.8193,221.99486,268.21671,245.46023,282.33772,326.46126,242.16844,289.44059,233.54963,297.53987,287.84746,262.00922,272.27917,218.49666,129.3236,287.65639,292.65584,294.31169,266.75139,257.15081,110.3865,297.4047,186.52811,223.15667,243.29987,310.12698,240.40791,290.58875,239.45133,176.28381,296.5848,322.49067,272.40247,320.28742,337.65111,231.42601,262.73536,367.95193,203.55737,293.71589,275.79002,298.86338,287.00353,341.3584,259.13977,321.81129,211.66974,289.19737,326.66341,285.74343,293.32018,318.39317,326.72444,196.84322,301.57854,244.2081,272.95514,190.23397,155.2724,365.81506,340.41883,283.28614,301.69705,266.62545,286.1516,293.07757,264.60164,322.79467,301.57897,288.74784,266.57634,320.26114,332.90933,181.51609,307.50521,251.86419,201.92818,213.04923,288.49829,226.90659,302.32448,245.87379,320.23568,222.46282,141.70304,283.44082,174.86759,280.08492,323.53731,218.33147,280.61244,244.63024,263.55633,236.34662,286.5263,305.67444,147.69925,270.7903,137.70196,310.89982,148.78867,219.46652,268.37469,271.43625,252.99511,356.92021,232.04984,287.0341,238.34005,138.35453,334.99513,235.39312,311.14893,323.26749,211.12002,304.58014,203.58811,329.89013,246.15499,270.15123,312.5251,200.85992,255.0941,237.09948,345.98432,241.13476,307.98951,171.10469,338.11703,300.57242,277.08119,172.51466,262.63415,270.38788,324.44244,240.56282,340.27856,323.20263,227.1784,262.40112,197.88782,221.11467,221.43001,195.34374,247.17464,259.81727,267.00619,261.41746,381.06651,173.00845,276.82863,259.24877,297.4325,189.09499,219.89063,312.20699,277.85828,233.39548,291.97902,216.39625,303.7667,317.55401,279.25058,266.75396,242.83139,309.62768,338.94376,248.01987,312.10431,290.36917,248.56535,292.90039,212.29211,234.17664,274.43532,339.2175,238.22193,230.98249,191.62813,283.18975,229.94272,369.95142,252.48827,181.21829,317.94951,212.56718,267.81841,337.38176,218.28819,238.87029,232.01027,292.6486,319.90551,315.05787,259.12294,286.35682,271.41862,276.82814,null,261.76646,283.32721,299.14003,283.35969,323.03473,390.35236,275.55537,220.97873,160.58387,346.77914,290.68248,99.98603,305.99771,185.90649,303.03308,303.98217,311.86451,201.93746,343.53182,154.36836,262.23033,319.64743,326.61891,294.78614,285.43392,330.56673,175.39598,230.27614,211.84241,303.97917,127.9435,297.68569,177.8113,258.88715,271.16533,303.3059,146.65565,330.81579,306.33145,205.99217,211.72373,249.10433,199.71926,156.1961,262.86124,271.6235,203.6045,229.7662,317.16501,195.59968,305.83112,267.08209,255.33352,170.78761,275.65342,251.76426,204.92995,228.87356,262.50718,276.92273,268.09847,275.50524,244.60841,294.15039,295.76329,241.47801,258.64825,239.55608,242.26815,313.6431,220.16289,333.61402,297.16815,242.54943,285.11864,338.87717,296.23999,230.9358,240.18354,255.94594,282.27413,327.62467,239.96065,291.25694,308.93168,323.47864,318.15556,316.94574,367.82271,231.53197,202.14391,234.96252,232.67812,250.04069,310.86648,303.57135,245.55146,248.17612,246.68087,208.04273,222.9261,288.95074,276.36492,326.42927,272.60283,240.04576,224.69784,208.7859,227.17757,242.7929,366.48141,286.54504,274.20354,252.22051,278.04682,312.20405,275.32533,273.99379,268.4379,272.06314,224.32605,284.3175,226.774,230.32518,247.37477,247.23785,283.34906,265.13819,294.6094,230.50107,260.54305,299.91456,136.0784,234.13109,230.4707,186.68132,266.89224,143.35088,299.87047,178.27704,326.8931,202.71705,307.0789,235.26712,286.61406,312.82716,213.52951,232.844,314.35084,311.81347,234.24345,177.40666,326.927,212.40026,291.43893,298.84138,273.57153,161.28081,242.1055,292.71955,229.79878,315.25581,217.03458,241.43943,261.39163,217.14231,270.03757,235.29633,246.22108,293.11948,379.08525,213.16562,319.06302,233.42513,332.71685,291.46752,220.14569,249.71901,261.60467,293.78953,272.16957,177.44984,246.58759,265.82938,269.86224,279.69255,214.25288,275.48373,286.46485,217.7563,280.94513,246.47253,285.54243,332.95686,273.34388,228.83246,286.87538,378.10985,209.21541,312.4025,234.90434,345.99645,313.5073,194.30562,256.76944,270.94893,272.43981,286.01989,258.51771,206.06643,218.37219,223.39854,315.63883,237.88477,276.33116,270.18784,272.18384,190.98106,225.17343,308.43505,295.7165,270.81555,200.17946,258.45743,240.36491,236.82392,265.4114,237.90525,166.42057,167.01758,267.26138,231.68366,218.37581,230.0546,267.54678,216.22659,282.21212,271.18626,311.62366,216.02847,143.64571,221.40697,294.17844,288.00363,274.75884,216.10315,252.24674,325.59221,284.26852,255.5141,210.24715,338.12844,297.40169,298.54122,194.96993,273.49039,269.58346,208.51834,248.03237,270.50646,207.80489,276.09702,265.0879,267.96107,219.13006,305.83847,273.0922,290.75356,193.99009,287.83194,174.92014,382.6571,306.0202,242.62116,286.8888,304.10948,215.36811,293.0315,265.19472,284.12047,249.00577,265.54423,289.14703,292.77441,286.88554,178.80951,255.44766,193.04835,242.19479,327.30812,284.99289,202.34876,252.52009,273.8809,352.47046,298.20729,219.2789,242.41211,322.27106,221.65889,343.71719,283.5434,193.88867,318.47014,310.5341,255.81546,308.35165,314.45911,265.95307,276.15103,154.08297,204.33282,283.61768,286.00287,246.03723,171.63864,241.59408,292.73469,247.67971,241.74784,258.64613,289.18278,231.6668,241.53475,276.97619,306.8951,198.47407,214.29948,184.17418,286.61118,241.20827,234.74187,321.49392,307.91032,198.60711,272.70749,225.36571,280.12787,181.03135,362.35654,274.22083,346.73207,290.88446,279.72059,338.18467,267.99821,238.75937,242.15725,244.58731,370.42177,236.26897,230.80044,287.15773,323.43818,264.76777,317.00657,247.65166,215.81284,309.08805,174.78552,252.86178,304.88772,287.97827,286.17638,204.75384,268.63115,218.96945,289.70227,226.50429,248.49445,294.9469,313.92889,300.67577,274.01729,289.90621,312.4326,307.94097,218.21483,248.07311,310.66014,175.0617,213.50702,276.54906,234.85092,285.37746,272.04103,185.5269,244.29677,264.21508,288.37452,219.27065,299.34831,208.03948,273.20989,260.51865,258.99166,202.97432,253.47378,251.12228,257.17834,288.58012,233.33372,284.47894,255.36457,144.67465,299.35366,232.86446,233.25831,256.70792,336.89499,222.93398,278.13398,268.52738,248.02666,206.09515,347.8791,257.82701,274.86973,310.40552,350.78903,262.64091,289.10757,302.31849,144.70436,201.9812,225.66936,177.18626,289.76098,244.90021,245.83976,308.64762,317.27662,331.38437,317.41358,330.01683,302.00004,334.77742,180.84875,186.05297,303.20859,200.90216,275.77083,226.52113,305.37023,73.60704,290.16549,189.58806,262.3943,287.29167,155.60101,263.31415,235.82191,326.69552,318.86369,259.68368,329.98875,292.00257,252.38218,332.08691,263.88728,329.38916,268.39444,329.95079,290.93899,309.77317,229.11831,252.68425,249.89113,263.16948,290.31708,267.0602,180.86392,370.94887,252.75783,225.1245,284.36381,275.61684,246.66215,168.17699,246.80152,261.08394,222.06297,181.88958,215.39022,268.70528,278.48759,269.51154,288.38201,242.82216,244.435,251.08767,209.16984,260.06193,301.58028,236.73322,292.41576,222.24472,290.39712,261.29794,186.81553,260.47567,264.93266,105.52363,262.21253,281.44439,321.45602,330.81177,279.76499,268.15164,238.51542,268.41541,301.32992,349.99308,315.7719,251.21218,268.88581,266.33456,183.2945,211.85168,273.40962,225.26651,368.43291,237.90949,246.20639,188.09679,317.41882,249.29158,159.24744,244.78812,185.6655,252.82706,204.48615,255.64763,284.00091,278.87492,314.23205,268.07953,268.47244,178.31056,283.83753,284.2125,285.6161,264.85436,306.94774,297.80524,248.3061,233.58988,317.26395,216.64183,342.43072,275.61962,287.56768,291.33049,205.26706,279.11154,284.31337,261.17644,276.66171,203.89482,244.02037,273.46104,120.6963,293.84141,291.33318,208.86964,112.5435,354.29549,344.68759,269.28562,269.90641,286.33194,192.13634,297.02504,219.5686,346.98918,170.7902,309.65875,242.52868,269.63887,291.24774,236.08439,251.7834,214.59657,231.86193,195.62391,329.82081,281.87615,210.67978,274.25708,226.14158,184.40475,260.48054,209.06578,224.64547,209.56287,155.95626,296.50422,229.67752,281.86174,276.14989,326.16201,258.61194,245.83581,178.43894,281.10075,236.32877,333.34913,303.59304,316.46177,251.48644,323.49642,287.25541,225.64662,334.62759,255.27897,247.72551,191.76963,293.58028,282.69619,280.22819,197.82595,215.18518,317.18136,349.06658,213.1829,272.92293,249.89669,312.01507,289.3818,230.92601,307.16899,285.92083,249.47976,253.42723,273.19073,210.62692,260.71553,202.94387,246.28763,160.71674,341.2083,235.06629,326.03359,335.2769,232.27918,208.48106,233.42492,90.11079,174.30872,225.10196,235.45401,313.48605,255.6163,325.02617,187.87157,339.53965,267.38317,313.70329,248.83874,308.8163,234.23639,332.71872,256.50056,273.32641,259.81977,237.27112,268.88987,267.07231,227.23699,217.14057,310.70537,291.70616,267.72922,296.80626,326.60534,372.35315,220.89371,304.46948,271.59546,247.61474,251.97888,316.8534,310.18164,335.31184,245.26478,274.01171,267.23474,301.41707,283.15272,289.17809,230.69968,288.82149,193.75781,257.38435,190.61145,323.93931,257.55938,244.22696,278.22304,261.89593,324.83694,313.90039,206.35275,216.52724,244.93999,263.2587,308.22823,332.71402,237.44301,272.77215,301.13935,337.32139,274.10525,203.71825,242.07093,147.14406,282.52374,216.39645,291.77018,261.14305,243.95402,304.65614,226.08829,304.33066,267.17005,316.55727,248.50248,303.08916,315.91339,270.74273,199.55111,269.42336,310.55039,297.43921,225.65645,256.51052,228.50262,262.9551,248.08287,180.6646,271.69095,281.72479,346.94507,294.7716,221.52312,224.69511,169.61052,314.67667,210.15213,238.4907,223.6405,237.53229,288.90946,283.6157,257.40166,254.99267,267.89958,316.64153,227.79508,258.89114,304.04884,170.87122,161.59225,246.6055,349.52755,330.94996,189.92756,307.83205,276.94688,315.89936,355.33054,289.74552,240.17498,176.80738,257.69231,297.15924,254.38349,241.76482,327.48941,236.58089,217.56974,277.92634,290.17093,301.9484,291.77813,159.01653,346.71734,320.58783,266.0895,231.52712,240.16564,160.09549,298.63527,192.07887,297.23093,298.28556,267.39173,284.4319,188.05976,326.17985,283.36408,281.06139,199.12708,258.10188,187.83743,298.82669,244.41138,244.24493,299.28697,294.17933,280.15748,280.67727,265.85933,259.70448,256.76468,296.87943,250.24927,259.34247,270.62127,204.95557,289.25939,305.67198,295.37753,301.17733,223.99103,286.74289,276.1875,206.42222,199.31664,271.3055,230.24738,297.08217,292.14282,328.49149,299.74674,253.17704,318.95902,170.80836,293.83777,220.67054,265.57455,313.74043,319.06612,225.09879,281.89777,295.03626,313.52297,276.78612,131.30397,144.40449,239.83727,389.53519,335.60175,260.43964,261.56661,211.10585,281.66191,268.94681,214.49733,279.22305,322.29664,202.64041,265.31335,306.97631,201.46765,249.74433,222.41027,155.01949,279.55968,241.47574,259.52482,300.8968,273.84023,203.39166,249.81994,239.40718,251.65846,210.73363,190.50844,256.3411,258.28253,292.51614,274.36108,345.04427,344.81095,271.48686,314.03825,252.21136,295.05921,312.14143,228.23393,295.68257,230.37337,230.66895,298.47398,287.99579,292.36326,363.86141,255.45501,218.82882,202.1685,233.05653,289.68315,203.76784,255.6419,245.10948,213.33293,311.63939,227.92453,245.66328,319.89805,352.87001,349.35833,244.21759,327.59438,319.78464,225.15388,177.68486,243.25836,243.22245,226.45777,202.77579,235.94944,233.96517,321.79905,285.67615,283.55828,300.14608,226.45646,238.18676,260.68338,336.82952,269.77235,286.23766,271.50105,273.29595,293.32488,317.91563,274.71137,258.57633,156.37213,315.95542,230.16445,326.54422,198.82878,234.78396,255.37671,235.81376,235.11039,239.24974,261.01103,334.23281,211.69958,139.54368,263.33366,203.94909,269.46582,243.72041,278.50039,329.09143,259.32889,214.20842,254.98363,201.50459,261.29396,234.10274,234.5351,242.26179,240.10996,283.22272,228.12991,329.33827,268.51192,301.52216,249.90002,305.49559,285.62167,254.95711,343.89591,228.27123,139.36519,299.93819,257.39878,172.94232,232.44663,302.45773,227.97739,348.19047,341.98477,215.49446,298.10765,236.6319,257.99036,265.57153,250.48059,295.09794,231.07352,271.71185,226.63104,286.96869,241.8658,268.85799,293.63808,273.57959,286.82137,271.18265,275.85647,288.57284,185.96689,246.50609,165.44177,204.70475,305.271,349.8803,352.75252,300.4105,185.46265,245.18683,233.75242,240.44664,280.01217,232.48289,277.98142,267.1805,260.19833,310.60623,266.63526,226.26917,309.62957,333.96312,279.61534,267.84165,320.26714,248.67942,232.10187,256.70339,190.61964,274.19751,301.66253,274.74479,324.55227,197.3237,240.03998,292.57817,235.8754,219.17505,286.08298,236.39711,243.42116,236.01068,242.10755,221.73185,225.92105,337.04558,258.2073,336.18061,267.70528,164.4361,319.43493,283.12565,217.84542,224.77647,229.99582,290.43439,408.80453,248.81233,312.50004,294.37407,271.38804,174.84282,243.7249,226.22809,295.95658,279.46997,238.99236,218.05185,260.62728,252.34711,186.37487,162.91442,243.99908,244.5479,218.45329,205.77464,222.50534,210.40378,188.85985,305.04773,218.18262,331.29026,246.9688,215.15257,312.63442,213.40566,266.50827,336.18347,215.63014,191.82017,323.03032,214.56763,224.13712,235.029,260.95666,334.3973,332.10999,295.1362,235.18909,211.66945,304.85909,258.08444,257.14666,298.75629,222.66728,152.10518,218.46433,271.3164,234.3945,187.98321,304.05375,202.39354,301.04407,266.14215,267.93763,298.64055,265.00456,269.86413,163.16071,290.23112,362.57171,255.70466,291.20007,255.62747,241.1176,292.75234,215.79469,278.33904,331.97005,273.64882,240.70777,266.01798,291.48382,329.38019,367.75885,250.62166,327.81385,282.05984,236.14127,243.3456,91.5437,282.33787,299.47602,257.27111,313.46306,311.9509,228.39402,259.59471,271.82899,252.61466,188.51956,274.82845,253.33197,217.22248,234.10316,285.68992,277.11269,155.09498,255.41157,307.88037,222.0269,234.89375,314.64308,300.0587,354.54801,280.57734,164.14046,221.43288,270.71045,224.61351,273.8371,199.48193,304.97486,300.52456,210.41108,256.66675,289.21468,302.29434,264.77048,238.41815,242.51738,319.56358,191.07467,346.01569,308.03259,337.2002,263.16302,260.84212,145.60781,289.91524,283.58064,230.29819,301.46917,276.3353,187.0106,344.63083,262.08515,278.81978,294.67777,213.88325,276.2618,327.83885,251.10743,254.66347,205.58656,314.77209,314.42655,334.53275,280.70512,209.8619,221.80883,208.66742,258.05702,233.77607,260.53099,241.48671,192.82241,297.38445,194.58169,250.21397,197.03649,298.52947,295.02938,185.80363,350.90538,185.22363,236.88441,260.78388,348.9611,309.26426,298.93895,294.80028,89.5779,233.19323,219.9137,292.87422,238.25664,240.80704,282.24867,158.87807,291.85675,184.92357,252.91101,233.84181,389.83031,291.35954,255.31523,325.50837,263.9551,212.74148,286.53969,219.5069,212.75782,205.22085,281.16929,233.27847,278.25406,204.02143,316.9496,301.05358,260.74445,273.00652,280.4705,241.88488,309.51979,260.71629,192.77467,282.92289,245.36793,205.33964,239.45865,283.0789,227.26934,294.68539,257.72114,268.84675,311.9826,262.14984,265.48602,233.60634,223.01795,181.01955,254.79727,280.52097,227.6522,304.49802,313.45222,251.51785,297.16073,205.28896,225.55437,112.33766,242.49878,241.80967,273.02902,222.90981,316.3314,181.51118,263.60349,240.26478,311.59682,274.5374,312.81912,209.43624,304.19655,299.73852,286.08006,233.08129,324.11561,225.66164,262.62472,289.87018,284.75952,264.63308,222.08086,320.71161,246.40881,267.44267,322.34652,282.5346,253.94745,281.70758,334.22204,182.48795,255.41157,216.27012,212.68147,187.03095,261.78527,267.22804,297.45129,224.02997,226.61496,250.45925,263.09618,294.48614,260.69206,250.99379,238.29992,275.61942,310.07903,322.58423,234.7559,314.05918,169.24135,302.48142,180.24733,277.52706,269.09089,305.09169,312.16915,232.36367,254.4311,250.58512,259.72288,283.38745,211.43393,191.47953,259.10744,279.97406,197.21254,309.9357,311.55618,261.49822,305.53847,277.92185,310.98356,285.62121,255.68515,231.56442,323.77776,238.8582,209.16402,262.04123,306.17103,238.11525,208.09621,306.53352,279.35121,258.85806,266.71055,262.91608,231.64128,292.5036,126.43111,262.44452,273.90808,244.23257,215.71623,227.65389,238.5825,267.19041,252.978,314.67364,333.76372,320.80887,308.38872,304.40888,192.68895,214.34552,256.31318,203.40942,249.07307,303.01867,307.37828,233.56802,227.7607,327.30931,258.1398,260.04166,202.54206,333.14985,192.91046,212.71648,325.53099,234.69116,304.42202,222.47719,202.01151,277.88226,337.07498,315.85183,278.9961,263.66373,214.10064,323.89731,296.012,270.47147,255.30982,260.23251,266.42764,304.37116,284.60535,247.57564,235.75363,226.22795,215.19051,339.46888,208.82525,247.45769,232.60781,321.07788,288.19023,288.91145,258.23498,262.19531,305.61489,328.79482,200.4064,252.26623,244.43251,311.29827,184.75031,326.91888,271.98217,239.74282,268.7501,283.52772,248.60124,250.1713,235.34286,344.58028,295.51545,205.64016,151.92283,229.85106,258.02268,310.40007,315.05985,280.32875,324.36553,259.43563,290.82986,276.75876,251.19882,234.05615,94.70979,250.06692,250.58663,300.45595,215.78154,143.33563,273.62985,249.62826,277.57933,187.96282,309.67576,252.46197,291.11451,241.59747,287.84637,203.07797,238.5903,227.71817,191.78758,279.45802,200.51068,287.70554,222.35019,215.61799,270.88948,279.63173,295.69716,277.87371,300.75463,280.79286,213.51082,212.6386,272.43278,214.94786,264.77956,245.94664,211.26427,290.41302,183.33345,306.19931,185.0701,248.83663,247.79142,225.36757,262.48614,274.06056,336.73062,320.3922,293.16489,286.99686,244.30883,276.39318,260.69418,230.4017,299.64393,236.36255,298.07739,228.32858,271.00039,230.39752,241.2062,207.70958,274.72636,237.0904,342.56241,303.58709,287.74558,249.56259,246.71667,321.45427,152.45422,333.50043,353.18088,242.99296,316.13057,260.77612,282.46645,128.1447,287.41582,265.92573,193.89702,287.89869,273.79095,264.25736,184.22152,285.55625,238.37178,298.31171,356.34901,277.66275,223.43383,301.84143,241.74907,180.15365,264.36491,277.02142,214.8256,291.09688,244.6437,248.01646,160.39431,260.25087,310.4915,188.00645,173.04186,201.73913,227.05272,184.86248,279.42932,308.74814,215.54135,299.3572,213.12319,309.46968,247.59366,282.86662,224.35768,209.78867,262.94717,247.29864,234.87167,304.6769,306.29937,214.22994,307.64912,280.07667,252.30708,290.91747,130.81806,250.89343,272.42943,280.30516,258.58833,279.43108,231.14302,282.10855,132.60374,297.80288,159.72659,273.1494,230.90251,317.3498,229.83089,127.44084,309.07493,234.94696,280.15015,233.02826,216.13023,310.40008,177.18753,283.27979,213.06757,178.18996,248.23561,150.31679,304.50273,211.66442,255.11862,307.65759,263.00482,253.24411,206.12467,270.36819,251.42952,275.24991,245.0627,278.2833,211.50988,260.43653,253.77161,297.32334,277.27536,232.78886,300.84122,323.57417,309.0927,248.59768,260.13671,270.97729,364.11254,223.44612,343.81798,301.32887,176.85997,217.51497,236.85566,265.70819,261.56296,275.48091,243.4384,343.26347,286.01444,196.59136,297.7393,259.3199,272.85206,187.77168,188.08513,284.84941,281.6127,224.656,254.12799,274.40921,246.72137,199.64849,235.45938,323.4518,254.04865,227.01918,219.39709,226.92033,257.27442,239.16917,281.88158,268.16839,219.61183,331.42234,237.78658,262.88173,216.12921,285.22853,290.25378,264.19841,246.48689,256.87053,248.06977,220.51989,288.30398,280.79162,196.27871,298.422,257.30564,252.31487,169.87456,142.18713,370.15777,338.05428,269.52888,230.07971,256.45711,284.05305,337.16085,274.68954,246.00208,277.62282,325.13902,282.17301,220.23942,240.89363,216.82282,168.58084,253.47884,288.67835,290.10388,179.14403,248.79653,321.0769,282.68738,312.42757,317.09478,304.47479,211.29173,287.31822,264.79303,237.01006,241.47756,287.11767,311.5577,233.52907,282.7937,290.55251,294.33756,228.0749,245.45425,264.78895,184.23782,180.75783,336.35465,227.21272,196.72376,101.72614,243.69226,285.24803,300.11925,304.41624,105.71109,276.09741,289.07392,87.05733,298.42878,299.52847,269.52621,276.99756,295.70035,297.3386,201.12807,252.68596,199.52624,271.72546,319.04567,212.34677,217.37162,314.12007,234.20802,290.55673,277.86673,183.46338,270.83678,186.61488,333.89646,229.5271,254.5127,266.77981,247.13693,278.96359,314.24458,277.01206,270.81784,115.13707,299.3163,188.90296,307.40464,246.48702,262.92626,228.02924,261.28308,287.81006,171.22247,298.34499,317.93814,340.50204,300.90299,261.23914,286.05537,274.66624,276.811,271.52347,273.54102,218.90316,285.42886,147.49566,272.73217,308.75785,159.31685,270.63035,315.72011,247.60034,314.19953,245.21975,270.82404,260.86529,229.82703,234.37077,258.29334,225.99456,266.71832,271.95426,327.47973,294.87235,305.26271,274.53138,303.34883,171.47013,283.71175,309.5981,302.25615,207.16515,267.33639,268.59457,342.47542,241.84521,222.35545,272.09713,249.83039,200.1267,326.11354,288.01231,299.25912,318.00903,272.64175,244.283,276.27767,199.79995,263.69138,246.11044,171.4712,321.507,201.27054,284.95605,367.78298,285.47049,257.86342,227.61644,209.18493,291.65166,365.97032,269.08933,310.46083,256.79555,252.11968,269.72693,323.77027,290.24727,235.4507,227.22516,305.96421,233.63121,239.28757,264.19109,317.46504,283.53305,164.78592,230.44262,253.78384,223.82874,233.06467,251.53024,292.5897,244.88979,258.17759,256.38695,321.89137,200.37856,359.88951,259.22546,266.14263,233.91975,288.08907,318.59415,241.31295,284.21548,268.07282,226.33784,277.18697,325.00809,229.15328,266.21943,255.14293,289.19922,300.70766,217.36403,266.34404,231.79405,258.21803,297.7019,310.1057,238.38034,218.32942,177.08937,273.26697,291.6668,263.22451,219.2761,332.2583,204.61454,250.57514,299.28135,234.29824,319.13155,327.99605,167.52552,296.8332,197.65506,297.54697,394.1258,155.29735,214.84756,288.58675,214.68952,198.7031,253.23266,223.25963,308.8752,255.87853,177.88037,247.91961,217.27404,310.20593,266.02696,328.04929,223.47679,263.414,227.84713,315.7514,303.73272,284.14458,128.41079,239.26102,277.1297,274.07369,209.88743,202.32352,255.67322,319.30377,118.72833,305.69569,263.10261,314.72762,290.69431,264.10644,266.90876,212.66396,311.45951,300.5189,321.81235,306.46683,249.25155,257.09967,275.53628,325.52114,259.32232,256.8852,275.54645,259.98507,283.22794,330.10793,325.37628,176.48583,236.92317,204.62504,277.99396,230.27898,255.50908,187.61843,212.50291,283.722,269.83301,300.25141,294.09846,217.28415,245.32004,279.46053,330.35742,204.23781,340.71006,289.42972,280.04524,269.77272,295.32134,228.71036,254.84067,212.69853,87.01008,269.29358,281.9188,271.69913,301.15653,269.60429,329.38137,278.22672,284.68133,185.30329,249.12695,184.3321,231.51765,235.811,211.19715,241.18641,225.07817,305.39034,228.49724,276.18822,244.91444,336.99834,261.41057,228.12182,259.67289,235.75839,289.93973,286.07372,216.07544,267.46294,253.79473,278.00447,264.55658,304.06832,337.31965,179.50387,264.35177,337.56183,276.61452,294.56418,234.08894,276.97031,261.07611,267.17046,333.77633,264.28478,246.16483,286.18059,288.10183,272.19658,268.43691,360.14963,191.07829,217.56347,303.66787,290.57723,179.26706,230.4838,283.79409,312.31948,311.81415,266.7963,222.79265,265.04851,358.82178,193.40989,289.56608,199.25752,260.23255,284.41171,273.79663,223.93663,294.86689,251.60785,126.3733,281.84508,202.72942,260.66669,226.55158,338.01301,309.27434,219.69637,293.45468,257.63749,275.80316,248.21499,256.03286,310.19113,260.43254,220.9329,260.29925,238.66271,268.31535,317.58491,219.38066,267.11914,313.03783,332.62599,312.86396,205.71617,286.90597,275.51113,267.12462,261.1508,307.3131,282.6004,332.83794,298.43259,272.27143,285.56287,281.05244,293.67704,263.05283,250.45572,241.54703,258.23103,229.17117,263.97638,206.38935,222.28076,314.23415,302.91903,362.9231,202.9318,292.56877,284.17635,333.41806,225.69471,317.95768,255.70441,278.0962,116.22788,291.38022,210.95799,219.14349,270.44947,270.6008,204.52365,221.20336,163.81323,209.56195,310.85022,218.3768,258.08928,255.86432,280.16283,325.07626,279.07126,321.96923,293.58423,254.78532,279.25805,307.35187,240.20602,316.56741,253.69989,280.36031,224.00445,325.51085,213.97591,253.72408,292.52439,266.53523,206.00905,307.49361,217.16123,246.08609,143.66822,268.15411,255.6981,233.6414,295.32682,296.39549,267.56525,310.62783,249.23077,305.71758,309.99486,247.96955,267.02284,259.35293,274.77678,176.96845,304.34978,293.44631,196.61299,274.68294,306.83548,276.10816,180.10934,311.67703,250.44271,294.8422,298.02537,256.11727,258.06384,219.15546,390.93573,314.4863,313.48376,246.56215,196.28391,207.74889,246.23976,310.65824,309.02708,310.5626,206.56735,330.42979,276.60469,232.48712,254.27592,286.81449,174.7817,258.26443,190.66588,255.70264,249.95776,238.63489,181.13922,187.34221,344.21422,283.52928,333.37237,276.52149,276.70156,187.71859,250.52421,266.53361,184.77973,171.94859,283.50191,270.75512,292.55473,178.7591,222.51376,199.25776,208.18861,259.90472,233.04869,225.14988,259.55017,236.71067,234.24165,301.47501,254.53016,330.60314,249.05995,302.22411,288.46298,252.64796,303.97621,246.61897,196.34381,180.43136,236.95372,224.41979,222.7809,202.72976,228.77804,314.76748,189.67714,274.73052,297.08353,224.92275,265.93113,229.8522,244.22477,321.98999,227.00196,240.86006,178.56857,252.18817,266.70234,197.93955,260.55085,275.49088,278.87771,291.40422,285.01423,269.02833,281.46893,248.64176,302.11353,304.45664,236.10121,246.88516,304.62661,277.17634,310.753,301.0613,244.66816,328.67084,325.57452,234.30215,198.80356,254.30847,233.19692,194.6515,253.69412,206.04836,323.70256,283.9374,178.34069,317.72944,218.99698,95.55308,304.29358,159.69582,216.55654,376.04288,261.23093,292.5466,298.33858,245.54929,213.86721,205.19784,248.34965,274.74346,305.53033,251.0488,260.22403,236.58132,208.62904,167.77341,233.18961,287.79956,270.65115,289.28266,245.23715,248.30835,264.63717,221.21075,231.25238,288.31728,293.73346,304.69195,215.53794,319.2478,290.27106,185.1302,257.01754,290.29324,244.50645,329.89651,219.84704,240.45095,355.29147,249.63059,239.94064,264.65146,237.29472,257.12914,300.23539,181.36782,261.51633,301.94962,243.92876,286.89998,292.57588,264.14389,343.63755,194.38831,374.73188,290.2078,269.28297,274.74078,208.43326,329.98718,262.97605,212.02833,201.2297,279.76148,192.08951,281.3779,97.83037,329.45548,218.8758,256.4569,284.57779,244.16786,262.03537,236.56565,197.34903,356.79666,349.49177,278.40376,230.43503,233.12124,275.21512,264.95654,294.50355,334.43132,285.04138,277.52533,287.31404,236.10713,262.46826,310.75389,282.57642,270.16539,222.85966,226.59581,354.02966,254.73478,226.32993,266.35941,303.87058,287.97573,287.33823,230.88169,255.83002,225.01486,300.50574,281.16169,164.05423,290.5693,298.96732,232.88617,244.93391,312.64914,281.64359,304.24328,254.90159,227.06154,255.66963,286.57283,238.29771,257.39907,208.94218,197.56718,336.9934,201.58822,316.2814,276.23615,271.61466,297.19281,252.0657,249.72503,292.1764,245.92773,305.01594,193.60667,197.77243,208.64704,231.02424,195.92848,257.79474,298.62253,202.66046,201.79867,331.79528,265.71015,324.83117,232.07528,123.72287,329.21307,321.58961,147.60081,286.27758,343.71686,295.76678,284.6522,225.26656,291.35961,303.60929,220.96509,291.55408,286.03936,243.48483,249.92418,225.24404,247.35297,259.19642,268.24682,355.36665,315.44196,232.93168,272.34801,284.27309,285.13899,250.43816,333.9612,173.3443,304.71523,264.31079,230.2607,291.40643,229.94737,283.29862,189.09817,270.40068,266.46938,283.9257,202.85259,286.35732,188.93678,297.5537,300.69447,309.0072,152.90073,228.89768,322.49409,263.20475,307.25071,329.13234,330.42949,309.18881,235.75752,280.14393,304.80468,300.14956,184.1024,318.38884,195.37002,265.06883,218.95324,302.39773,330.68604,295.03937,246.37183,350.6948,256.94675,256.27879,165.58668,303.04024,299.16981,270.80897,305.94261,210.63384,348.70732,348.96405,264.59184,360.80927,286.04096,199.04942,273.32975,207.71419,277.67287,265.68836,238.00196,157.03123,213.58688,178.21727,262.83982,273.52766,253.19516,361.33341,273.31205,197.4602,188.71954,233.49142,278.80155,248.96679,270.28962,332.39548,237.55257,301.59478,212.80182,246.40353,237.55133,183.48334,298.86936,258.13763,201.18234,281.1913,264.87427,292.13172,246.10398,280.53674,244.90374,296.34489,279.45913,236.46712,166.78335,310.25209,276.09061,253.08924,288.0538,353.57674,277.44646,301.78249,274.95773,254.31994,212.75783,251.55273,355.68585,284.87599,222.33807,286.81845,239.60044,165.47236,305.54349,319.53725,221.29096,239.49377,259.48528,256.40774,227.3712,264.80947,292.26602,300.95119,221.27892,246.84712,227.72244,127.89481,355.24319,133.17583,264.10257,207.18378,244.53584,262.3953,234.45959,270.76605,227.65306,310.56919,248.63813,301.94249,278.98949,262.82084,301.26209,267.82808,305.37908,325.03329,233.26791,202.55422,303.27502,301.80756,223.44536,284.99379,191.3498,218.77149,291.07846,262.09753,224.0008,209.98154,298.01728,300.29222,221.90253,298.90347,317.53252,321.62163,260.42746,241.10807,230.9229,192.23823,321.57636,315.32017,281.67528,298.83876,324.81897,296.45925,273.59054,274.67293,222.82469,192.5219,230.26896,299.91338,294.95922,349.27878,274.26806,232.16579,260.10155,330.80266,275.33824,278.07475,291.26287,246.18482,262.66139,214.88092,350.896,314.33902,286.15212,291.25446,259.7187,192.31545,316.79995,247.28965,221.79188,282.39662,313.13504,337.11399,295.42576,268.74398,159.76123,242.70563,335.50475,238.72729,197.42797,255.76387],"Numeracy_score_b":[0,0,1,0,0,1,1,0,0,0,0,1,0,1,0,0,1,1,1,1,0,1,0,0,0,1,1,1,1,0,0,0,0,1,0,1,0,1,0,0,1,0,0,0,0,1,0,1,1,1,0,0,1,0,1,0,1,0,1,1,0,0,1,0,1,0,0,1,0,0,1,1,0,1,0,0,1,0,0,1,0,1,0,1,0,0,1,1,0,1,0,0,0,0,0,0,1,0,0,1,1,1,0,0,0,0,1,0,0,1,0,0,1,1,1,0,1,1,0,1,1,0,0,1,1,0,0,0,1,0,0,0,1,1,1,1,0,1,0,0,1,0,0,0,0,0,1,0,1,0,1,1,1,1,1,1,0,1,1,1,0,1,1,1,0,1,0,1,0,0,1,0,1,0,0,0,0,0,1,1,0,1,0,1,1,0,1,0,0,1,0,1,1,0,0,1,0,0,0,0,1,1,1,0,0,0,0,0,1,1,0,1,0,1,0,0,0,0,0,1,0,0,0,0,0,1,0,1,1,1,1,1,0,0,0,1,0,0,0,0,0,1,0,0,0,0,1,0,0,1,1,1,1,1,0,0,1,0,0,1,0,1,0,1,0,0,0,1,1,0,1,0,0,0,1,1,0,0,1,1,0,0,0,0,1,1,0,0,0,1,1,1,1,1,1,0,0,0,1,0,1,1,1,0,0,0,1,1,0,0,0,0,1,0,1,0,1,0,1,0,0,0,0,0,0,1,0,1,0,1,0,1,0,0,0,1,1,1,1,1,1,1,0,1,1,0,0,0,0,1,1,0,0,0,1,1,0,0,0,0,0,0,0,1,0,0,1,1,1,1,0,1,0,0,1,0,0,0,1,0,0,0,0,1,1,0,1,0,1,0,1,0,1,0,1,0,1,1,0,1,1,1,1,1,0,1,1,0,1,1,0,0,0,0,1,0,1,1,1,0,0,1,0,1,1,1,0,0,1,1,0,0,0,0,0,1,0,0,0,0,0,0,0,0,1,0,1,0,1,0,1,1,0,1,0,0,0,0,0,0,1,0,0,1,0,1,1,0,0,0,0,1,0,0,0,0,0,0,0,0,0,1,0,0,1,1,1,1,0,0,1,0,1,1,1,1,1,1,1,0,0,1,0,0,0,1,0,0,0,0,1,0,1,0,0,1,1,1,1,0,0,1,0,1,1,1,0,0,1,1,1,1,1,0,0,0,0,0,0,0,0,0,1,1,0,1,0,1,1,1,0,1,1,0,1,0,1,0,1,0,0,1,0,1,0,0,1,1,1,0,1,1,0,1,0,0,0,1,0,1,0,0,0,0,1,1,0,1,1,1,1,0,0,0,1,0,0,0,0,1,1,1,1,0,0,0,0,0,0,0,1,0,0,1,1,1,1,1,1,0,0,1,0,0,0,1,1,1,1,0,0,0,0,1,1,1,0,1,0,0,1,0,0,0,0,1,1,0,0,0,0,0,0,0,1,1,0,0,0,1,0,1,1,1,0,1,1,1,0,0,0,1,1,1,1,0,1,0,1,1,0,0,1,1,1,1,0,0,0,0,0,1,0,0,1,1,0,1,1,1,0,0,1,1,1,1,0,1,1,1,0,1,1,0,0,0,1,0,0,1,1,1,1,0,0,0,1,1,0,1,1,1,0,1,1,1,0,0,1,0,1,1,1,1,0,0,0,0,0,0,0,0,1,0,1,1,0,1,0,0,1,0,0,0,0,0,0,1,1,1,0,0,0,0,1,1,0,0,0,0,0,0,1,0,1,1,1,1,0,0,0,0,0,1,1,1,0,0,1,1,0,0,0,0,0,1,1,1,1,1,0,0,1,1,0,0,0,0,0,1,0,1,1,0,0,0,0,1,1,1,1,0,1,0,0,1,0,1,1,1,1,1,1,0,0,0,0,0,1,0,0,0,0,0,0,0,1,0,1,0,1,0,0,1,0,0,0,0,0,1,1,0,1,1,0,0,1,0,1,0,0,0,1,1,0,1,0,1,0,1,1,0,0,0,0,0,1,1,1,0,1,0,1,0,1,1,1,1,1,1,1,0,0,1,0,0,0,0,0,0,0,1,0,1,0,1,0,1,1,0,1,0,0,1,0,0,1,0,0,0,1,0,1,1,1,1,0,0,1,1,1,0,1,1,0,1,1,1,1,1,1,0,0,1,1,1,1,0,0,0,0,0,0,1,1,1,0,1,0,1,1,1,0,1,0,0,1,1,1,1,0,1,1,1,1,1,1,0,0,1,1,0,0,0,0,1,1,0,0,1,0,0,0,1,1,1,1,1,1,0,0,1,1,1,0,1,1,1,0,1,1,0,1,0,0,1,1,0,0,0,0,0,1,0,0,1,1,0,0,0,0,0,1,1,1,0,1,0,0,0,1,1,0,0,0,1,0,1,0,1,0,0,1,0,1,0,1,1,0,0,0,0,0,0,1,1,0,0,1,0,0,0,0,1,0,0,0,1,1,1,1,0,1,0,0,1,0,0,0,0,1,0,0,0,1,1,1,0,0,1,1,1,0,1,1,0,0,0,1,0,1,0,0,1,0,0,1,1,1,0,0,0,0,0,1,1,0,1,0,0,1,1,1,0,0,0,1,1,1,1,1,0,1,0,0,1,0,1,0,0,0,0,1,1,1,1,0,0,0,1,1,1,1,0,1,1,0,0,1,1,0,1,0,0,1,0,1,1,1,1,0,0,1,0,1,1,1,0,0,1,1,1,0,0,1,1,0,0,0,0,0,0,1,0,1,1,0,1,1,1,1,0,1,1,1,0,1,0,0,0,1,1,0,0,0,1,1,1,1,0,1,0,1,1,1,1,1,1,0,0,0,0,0,1,1,1,0,0,0,0,1,1,0,1,0,0,0,1,1,0,0,0,1,0,0,0,1,0,0,0,0,0,0,0,0,0,1,1,1,1,1,1,0,1,0,1,0,0,0,1,1,0,1,0,0,1,0,0,0,1,1,1,1,1,0,0,1,1,1,0,1,1,0,1,1,1,1,1,1,1,0,1,1,0,1,1,0,1,0,0,1,0,0,0,1,0,1,1,0,1,0,0,0,1,1,0,1,1,0,1,0,0,1,0,1,0,0,0,1,1,0,1,1,0,1,1,0,1,1,1,1,0,0,1,0,0,0,1,1,1,1,0,1,0,1,1,0,1,0,0,0,0,1,1,1,0,1,1,0,1,1,0,0,0,0,1,0,1,1,0,0,0,0,1,1,0,0,0,0,0,0,1,1,1,1,1,0,0,0,0,0,1,1,0,0,0,1,0,0,0,0,0,1,1,0,1,0,1,0,1,0,1,1,1,1,0,0,1,0,0,1,0,1,0,0,1,1,0,0,0,0,1,0,0,0,1,0,0,0,0,1,1,0,1,1,0,1,1,0,0,1,0,1,0,1,1,1,1,0,0,1,1,0,0,1,0,0,0,0,1,1,0,0,0,0,1,0,1,0,1,0,0,1,0,0,1,1,1,0,0,0,0,1,1,0,1,1,0,1,0,1,1,1,1,0,1,1,0,0,0,0,1,0,1,0,1,1,0,0,0,0,0,1,0,1,1,0,1,0,0,1,0,1,0,0,0,1,1,1,1,1,0,1,0,0,1,0,1,1,1,1,1,0,1,0,1,1,1,0,0,1,1,0,0,0,0,1,1,0,1,0,0,0,0,1,1,1,0,0,0,0,0,0,1,0,1,1,1,1,0,0,0,1,1,0,1,1,1,1,1,0,1,0,1,1,0,0,1,1,0,0,0,0,1,1,0,1,0,1,1,1,1,0,0,1,1,1,1,1,1,0,0,1,0,0,0,1,0,0,0,1,0,0,1,1,0,1,0,1,1,1,1,1,1,0,0,1,0,0,0,1,0,0,0,0,1,0,0,1,0,0,0,1,1,0,1,0,1,1,1,1,0,0,0,1,0,0,0,1,0,0,0,1,1,0,0,0,0,1,0,0,0,1,0,0,0,1,1,1,1,0,0,0,0,0,1,1,1,0,1,1,1,1,1,0,1,1,1,1,1,0,0,0,1,1,0,1,0,1,1,0,0,1,0,1,1,1,1,1,0,1,0,0,1,0,0,0,0,1,1,0,0,1,1,0,0,0,0,1,0,0,1,0,1,0,0,1,0,0,0,1,1,1,0,1,0,1,0,0,1,0,0,1,1,1,1,0,1,0,1,0,1,1,0,0,1,0,1,0,0,1,0,0,0,1,0,1,1,0,1,0,1,1,0,1,1,1,1,1,1,1,1,1,0,0,0,1,0,0,0,0,1,1,1,0,1,0,1,0,1,0,0,1,0,0,0,1,1,1,1,1,0,0,0,1,0,0,1,0,0,1,1,0,0,0,0,1,0,1,0,0,1,1,1,0,1,0,0,0,1,0,0,1,0,1,1,0,1,1,0,1,0,1,0,1,1,0,1,0,0,0,1,1,1,0,1,0,0,1,1,1,1,1,1,0,1,1,0,0,0,0,0,1,0,1,0,1,1,0,1,0,1,1,0,0,0,0,0,1,1,0,0,1,1,0,0,0,1,0,1,1,0,1,1,1,0,1,1,1,0,1,0,1,1,1,1,1,1,0,1,1,1,1,0,0,0,1,0,0,0,1,0,0,1,1,1,0,1,1,0,0,0,1,0,0,1,0,0,1,1,1,1,0,1,1,0,0,1,1,0,0,0,1,1,1,1,1,1,0,0,1,1,0,1,1,1,0,1,1,1,1,0,1,1,1,0,1,0,0,1,1,0,0,0,1,0,1,1,0,0,0,1,1,0,1,0,0,1,1,1,1,1,0,0,1,1,0,0,0,0,1,0,1,1,1,0,0,1,1,1,0,1,1,1,1,0,1,1,1,0,1,1,0,0,0,0,0,1,1,0,1,0,1,0,0,1,0,0,0,0,0,0,0,1,0,0,0,1,1,1,1,1,0,0,0,1,1,0,1,1,1,1,0,1,0,0,0,1,0,0,0,1,1,0,0,0,0,1,0,0,1,null,1,0,0,1,1,1,1,0,0,1,1,0,0,1,1,1,1,0,0,1,0,1,1,1,1,1,1,0,0,0,1,0,1,1,1,0,0,1,0,1,1,0,1,1,1,0,1,1,0,0,0,0,1,1,0,1,0,1,1,1,1,1,0,1,1,0,1,0,1,1,1,1,1,0,1,0,0,0,0,0,0,0,0,1,0,1,0,1,1,0,0,1,0,1,1,0,1,0,1,1,1,0,0,0,1,1,1,1,0,0,1,1,1,1,0,0,0,1,0,1,1,0,1,0,0,1,0,1,1,1,1,0,1,1,0,1,0,1,0,1,0,0,0,0,1,1,0,1,0,1,1,1,1,1,0,1,1,1,1,1,0,0,1,1,1,1,1,0,0,0,0,1,1,0,0,1,0,0,0,0,0,0,1,1,1,1,1,1,1,1,1,1,1,0,1,0,1,0,0,1,1,1,0,1,1,1,1,1,0,1,0,0,1,0,0,1,1,1,1,1,1,1,1,1,0,0,1,1,0,0,1,0,1,0,1,0,1,1,0,1,1,0,1,0,1,0,1,1,1,1,1,0,0,1,1,1,0,0,1,1,0,1,1,0,1,1,1,0,0,1,0,1,0,0,0,1,0,1,0,1,1,1,0,0,1,1,1,1,0,1,1,1,1,1,1,1,0,1,1,1,0,0,1,0,1,0,1,0,1,0,0,1,0,1,1,0,1,1,1,0,0,1,1,0,1,1,0,0,1,1,1,1,1,1,0,1,0,0,1,0,0,1,0,1,1,1,1,0,1,1,1,1,1,0,1,1,0,0,0,0,1,0,1,0,0,0,1,1,1,0,0,1,1,1,1,1,0,1,1,0,0,1,1,0,0,0,0,0,1,0,0,1,0,0,1,0,1,1,1,0,1,0,1,1,1,1,1,1,0,0,0,0,1,1,1,0,1,1,1,1,0,1,0,1,1,1,1,0,1,0,0,0,1,0,1,1,1,0,1,1,1,0,0,0,0,0,0,1,0,0,0,1,0,0,0,0,0,0,1,0,1,1,0,1,1,0,1,0,1,1,1,1,1,1,0,0,0,0,1,1,0,1,1,0,1,0,0,1,0,0,1,1,0,0,0,1,1,1,0,1,0,1,1,0,1,1,1,1,1,1,1,0,1,0,1,1,1,1,1,0,1,1,1,1,1,1,1,0,1,0,1,0,1,0,1,0,0,1,1,1,1,0,1,0,0,1,1,1,0,1,1,0,1,0,1,0,1,1,1,1,1,0,0,0,0,0,0,1,0,0,1,0,1,0,1,0,1,0,1,0,0,1,1,1,0,1,1,1,1,0,0,1,1,1,1,1,0,1,1,1,0,1,0,0,1,0,0,0,0,0,1,0,1,1,0,1,1,1,1,0,0,0,0,1,1,1,1,1,1,0,0,0,0,1,0,1,0,1,0,0,0,1,1,1,1,1,1,0,0,0,1,0,0,1,0,0,1,0,0,1,0,0,1,1,0,0,0,0,1,1,0,0,1,1,1,0,1,0,0,1,1,0,1,1,0,1,0,1,0,1,0,0,1,1,1,1,0,1,1,1,0,1,0,0,0,1,1,0,0,0,1,0,1,1,0,1,1,0,1,1,0,0,1,0,0,0,1,0,1,1,1,1,0,1,0,1,1,0,0,0,1,1,1,1,0,1,1,1,0,1,0,0,0,1,1,1,0,1,1,1,0,1,1,0,0,1,1,0,0,0,1,0,0,0,1,0,1,0,1,0,1,1,0,0,1,1,1,1,1,0,0,0,0,1,0,1,0,0,0,1,0,1,0,0,0,0,0,0,1,0,1,0,0,1,1,0,1,0,1,0,1,0,1,1,1,0,0,0,1,0,0,1,1,1,0,0,0,0,1,0,0,0,0,1,1,1,1,0,1,1,1,1,0,0,0,0,0,0,0,1,1,1,1,1,0,0,0,0,0,0,1,1,1,1,0,0,0,0,1,0,0,0,1,1,1,1,1,1,1,1,1,1,1,0,0,1,0,0,0,1,0,0,1,0,1,1,1,0,1,0,1,0,0,0,0,0,1,1,1,0,1,1,1,0,0,0,1,0,1,0,0,1,1,1,1,0,0,0,1,1,1,0,1,1,0,1,0,1,1,0,1,0,1,0,0,1,1,0,1,1,1,1,1,1,0,1,0,1,0,0,0,1,0,0,1,0,1,1,1,1,1,1,0,1,1,1,1,0,1,0,0,1,0,0,1,0,1,1,0,1,0,1,0,1,1,1,0,0,0,1,0,1,1,1,0,0,1,0,0,0,0,0,0,0,0,1,0,0,0,1,1,0,0,1,1,1,1,1,0,1,1,1,0,0,1,0,1,0,0,0,0,1,0,1,1,0,1,1,0,1,1,0,1,1,1,0,1,0,1,1,1,0,0,1,1,0,1,0,1,0,0,1,1,0,0,1,0,1,1,0,0,0,1,1,0,1,0,1,0,1,1,1,1,1,1,0,0,0,0,0,0,0,0,0,0,0,1,1,0,1,0,0,0,1,0,1,0,1,0,1,0,1,0,0,0,0,0,1,0,0,1,1,0,1,1,1,0,0,1,0,0,0,1,0,1,1,1,1,1,0,1,1,0,0,1,1,0,0,1,1,0,1,1,0,1,1,1,1,1,0,0,0,1,1,1,0,1,1,0,0,0,1,1,0,1,0,1,1,0,1,1,1,1,1,1,1,1,1,0,1,1,1,1,1,1,0,1,0,1,1,1,0,1,1,1,1,1,0,1,1,0,1,0,1,1,1,1,0,1,1,0,1,0,1,0,0,0,0,0,1,1,1,0,0,1,1,1,0,1,1,0,1,1,0,1,0,0,0,0,1,1,1,0,0,0,0,0,1,1,0,1,1,0,0,0,0,0,0,1,0,1,1,0,0,1,1,1,0,1,0,1,0,1,1,1,0,0,1,1,0,1,0,1,1,1,0,0,0,0,0,0,0,1,0,1,0,1,1,0,1,0,0,1,0,0,1,1,1,1,0,0,1,0,1,0,1,1,1,0,1,0,1,1,0,0,1,0,0,1,1,0,1,1,1,1,1,1,0,1,1,1,1,0,0,0,1,0,1,0,1,0,0,0,1,0,1,0,1,0,0,1,0,1,0,0,0,0,0,1,1,1,0,0,0,1,0,1,0,0,1,1,0,0,1,0,1,1,0,1,1,1,0,1,0,1,0,1,0,1,1,1,1,1,0,0,1,0,0,0,0,0,1,1,0,0,0,0,1,0,1,0,1,0,1,1,0,0,0,1,0,0,1,0,1,1,1,0,1,1,0,1,0,1,1,0,0,1,1,1,1,1,0,1,1,1,0,0,0,1,0,0,0,1,1,0,0,1,1,0,1,0,0,0,0,1,0,1,0,1,1,1,0,0,0,1,1,0,1,0,0,1,1,1,1,0,1,1,0,0,0,0,0,1,0,0,1,1,1,0,1,0,0,0,1,1,1,1,0,0,0,1,0,0,1,0,1,0,1,0,0,0,0,0,1,1,1,1,1,0,0,0,1,1,0,1,1,1,0,1,1,0,1,0,1,1,1,0,0,0,1,1,0,1,0,1,0,0,0,0,0,0,0,0,0,1,0,0,1,1,1,1,1,1,0,0,1,1,0,0,0,0,1,1,0,1,1,1,0,0,0,0,1,0,0,0,1,1,0,1,0,0,0,0,0,0,1,0,1,1,0,1,0,1,0,1,1,1,1,1,0,1,1,0,1,0,1,0,0,1,0,1,0,1,1,1,1,1,1,1,1,0,1,0,1,0,1,0,1,1,0,0,1,1,1,0,1,0,0,0,0,0,0,0,1,1,0,1,0,1,1,1,1,1,1,0,1,1,0,0,1,1,1,0,1,0,1,0,1,1,0,0,1,0,0,1,0,1,1,1,1,0,1,1,1,1,0,0,0,0,0,1,1,1,0,1,1,1,1,0,1,0,1,0,0,0,1,1,0,0,0,1,0,1,0,1,1,1,1,0,1,1,0,0,0,0,0,0,1,1,0,0,1,1,1,1,1,0,0,1,0,1,0,0,1,1,0,0,1,0,1,0,0,0,1,1,0,0,1,0,1,1,1,1,0,1,1,1,1,1,1,0,1,0,1,1,1,1,1,0,0,1,1,1,1,1,1,0,0,0,1,1,1,0,0,1,0,1,0,1,1,1,1,0,0,1,0,0,1,0,1,1,0,0,0,1,0,1,1,1,0,1,1,1,1,1,0,0,1,0,1,0,0,0,1,0,1,0,1,0,0,0,1,0,0,0,1,1,1,0,0,0,1,0,0,1,0,0,0,0,1,1,1,1,0,0,1,0,0,0,0,1,0,0,1,0,0,1,0,1,1,1,1,0,0,1,0,0,1,1,1,0,0,0,0,0,1,1,1,1,0,1,1,0,1,1,1,1,0,1,0,0,1,0,1,1,1,0,0,0,1,1,1,0,0,0,1,0,0,0,0,1,1,0,0,1,0,0,0,1,1,1,0,0,0,0,0,0,1,1,1,1,0,1,0,0,0,1,0,1,0,1,1,0,1,1,1,1,1,0,0,1,1,1,1,0,0,0,0,1,1,1,1,1,0,1,0,1,1,0,1,1,1,0,0,1,0,0,1,1,1,0,1,1,0,1,1,1,0,1,1,1,1,0,1,1,0,1,0,0,0,1,0,1,1,1,1,1,1,0,0,0,1,1,1,1,0,0,1,1,0,1,0,0,0,1,0,1,1,1,0,0,1,1,1,1,0,1,1,1,1,1,1,0,1,0,1,1,1,0,1,1,1,0,0,0,1,0,1,1,0,1,1,0,0,1,0,1,0,1,0,1,1,1,1,0,1,1,1,1,1,0,1,1,0,1,0,1,1,1,0,1,0,1,1,0,1,0,0,1,1,0,1,0,0,1,1,0,1,0,1,0,1,1,0,0,1,0,1,0,1,1,0,0,1,1,0,0,1,0,0,1,0,1,0,1,0,1,0,1,1,1,1,0,1,1,1,0,1,1,1,0,1,0,1,0,0,1,0,1,1,0,1,0,0,0,0,0,1,1,0,0,0,1,1,0,0,0,0,1,0,0,0,0,0,1,1,0,1,0,1,0,1,1,1,0,0,0,0,1,0,1,1,1,0,1,0,1,1,1,0,1,1,1,0,1,0,1,1,0,1,0,1,1,0,1,0,0,1,0,1,0,0,0,0,1,0,1,1,0,1,1,1,1,1,1,1,1,1,1,0,1,1,1,1,1,1,0,1,0,0,1,1,0,0,1,0,0,0,0,0,0,1,0,1,1,0,1,0,1,1,1,1,0,0,1,0,1,0,1,1,1,0,1,0,1,1,0,1,1,0,0,1,0,0,1,1,1,1,1,1,0,1,0,1,0,0,1,0,1,0,0,1,0,1,0,1,1,0,1,0,1,0,0,0,0,0,1,1,1,0,0,1,1,1,1,1,1,1,1,0,0,0,1,0,1,1,1,0,1,1,1,1,0,1,0,1,0,0,1,0,1,0,0,0,1,1,0,1,0,0,1,0,0,0,0,1,0,1,0,1,1,1,0,1,1,0,0,1,1,1,1,0,1,1,1,1,1,1,0,0,1,1,1,1,1,1,0,1,1,0,0,0,1,0,1,1,1,1,0,0,1,0,0,1,1,1,0,1,0,1,0,1,1,0,1,0,0,1,0,0,0,1,1,0,1,0,1,0,0,0,1,1,1,1,1,1,0,0,0,0,0,1,1,1,1,0,1,1,1,1,0,1,1,1,0,1,1,0,0,1,1,0,0,0,0,0,0,1,1,1,1,1,1,1,0,1,1,0,1,0,0,1,1,0,0,0,1,1,1,0,1,1,0,1,1,1,0,1,1,0,1,1,1,0,1,0,1,0,1,1,null,1,1,0,1,1,1,0,1,1,1,1,1,1,1,1,1,1,1,1,0,1,1,1,1,0,0,1,1,0,1,0,1,0,1,0,1,0,0,0,1,0,1,1,1,0,1,1,0,0,1,1,0,0,1,1,1,1,1,0,0,0,0,0,1,1,0,0,0,1,0,1,1,1,1,1,1,1,1,1,1,1,1,0,0,1,1,1,0,0,1,0,1,1,1,1,0,0,1,0,1,0,1,1,0,0,1,1,1,0,0,1,1,0,0,1,0,1,1,1,0,1,1,0,0,1,1,1,0,1,1,1,1,0,1,1,1,0,0,1,0,1,1,0,1,1,1,1,1,0,1,1,1,1,0,1,1,1,1,1,1,0,1,1,0,1,1,1,1,0,0,0,1,0,0,1,0,0,0,1,1,0,0,1,1,0,1,1,0,1,0,0,0,0,1,1,1,0,1,0,0,1,0,0,1,1,1,1,1,1,0,1,1,1,1,1,0,1,0,1,1,0,1,1,1,1,0,0,0,1,1,0,0,1,0,0,1,0,0,1,1,0,1,1,1,0,0,1,0,0,1,0,0,0,1,1,1,1,0,1,0,0,0,1,0,0,1,0,1,1,0,1,0,1,1,1,1,0,0,1,1,1,1,0,0,1,0,0,0,1,0,1,0,0,1,1,1,1,1,0,1,1,0,1,1,1,1,1,0,1,0,1,1,1,1,1,1,0,1,0,1,0,0,1,1,1,1,1,1,1,1,1,1,1,1,1,1,0,1,0,0,0,1,0,1,0,1,0,0,1,0,1,1,0,1,0,1,0,1,1,0,1,0,1,0,0,1,1,0,1,0,1,0,0,1,0,1,1,0,1,0,1,0,1,1,0,0,0,1,0,1,0,1,1,1,0,1,1,1,0,1,1,0,1,0,0,0,0,0,1,1,1,1,0,1,0,1,0,0,1,1,0,1,0,1,1,1,1,0,1,1,0,1,1,0,1,0,0,1,1,0,0,0,1,0,1,0,0,1,0,1,1,0,0,0,1,1,1,0,1,1,1,null,1,1,1,1,1,1,1,0,0,1,1,0,1,0,1,1,1,0,1,0,1,1,1,1,1,1,0,0,0,1,0,1,0,0,1,1,0,1,1,0,0,0,0,0,1,1,0,0,1,0,1,1,0,0,1,0,0,0,1,1,1,1,0,1,1,0,0,0,0,1,0,1,1,0,1,1,1,0,0,0,1,1,0,1,1,1,1,1,1,0,0,0,0,0,1,1,0,0,0,0,0,1,1,1,1,0,0,0,0,0,1,1,1,0,1,1,1,1,1,1,0,1,0,0,0,0,1,1,1,0,1,1,0,0,0,0,1,0,1,0,1,0,1,0,1,1,0,0,1,1,0,0,1,0,1,1,1,0,0,1,0,1,0,0,1,0,1,0,0,1,1,0,1,0,1,1,0,0,1,1,1,0,0,1,1,1,0,1,1,0,1,0,1,1,1,0,1,1,0,1,0,1,1,0,0,1,1,1,0,0,0,0,1,0,1,1,1,0,0,1,1,1,0,0,0,0,1,0,0,0,1,0,0,0,1,0,1,1,1,0,0,0,1,1,1,0,0,1,1,0,0,1,1,1,0,1,1,0,0,1,0,1,1,1,0,1,1,1,0,1,0,1,1,0,1,1,0,1,1,1,0,1,1,1,1,0,0,0,0,1,1,0,0,1,1,1,0,0,1,0,1,1,0,1,1,0,1,1,1,1,0,0,1,1,0,0,0,1,0,0,0,1,0,0,1,1,0,0,0,1,0,0,1,1,0,1,0,1,0,1,1,1,1,1,1,1,0,0,0,1,0,0,1,1,1,1,0,0,1,0,0,1,1,1,0,1,0,1,0,0,1,1,1,1,1,1,1,0,0,1,0,0,1,0,1,1,0,0,1,1,0,1,0,1,1,0,0,0,0,0,1,0,1,0,0,1,0,0,0,1,0,1,1,0,0,1,0,1,1,1,1,1,1,0,0,0,0,1,0,0,1,1,1,1,1,1,1,0,0,1,0,1,0,1,0,1,0,1,1,0,1,0,1,1,1,1,1,0,1,1,1,1,1,1,1,0,0,0,1,1,1,0,1,0,0,1,1,0,0,0,1,0,0,0,1,1,1,1,0,0,0,0,1,1,0,1,0,1,1,0,1,1,0,1,1,1,1,1,1,0,1,1,1,1,0,1,1,0,0,1,0,1,0,0,0,1,0,0,0,0,0,0,0,1,1,1,1,1,0,1,1,1,1,1,1,0,0,1,0,1,1,1,1,0,1,1,1,1,0,0,1,0,1,1,0,0,1,1,1,1,1,0,1,0,1,0,1,0,1,1,0,0,0,0,0,1,1,0,1,0,0,1,0,0,0,0,1,0,1,1,1,0,0,0,1,0,1,1,1,0,1,1,0,1,0,0,0,1,1,1,0,0,1,1,0,1,0,1,1,0,1,1,0,0,1,0,1,0,0,0,1,0,1,1,0,0,0,0,0,0,0,1,0,1,0,1,1,1,0,1,0,1,0,1,1,0,1,1,0,0,1,1,1,1,1,1,0,1,1,0,0,1,1,1,0,1,1,1,1,1,0,1,0,0,0,1,0,0,1,1,1,1,0,0,0,1,1,1,0,1,1,1,1,0,0,0,1,0,1,1,0,1,0,1,1,1,0,1,1,1,0,1,1,1,0,0,0,1,0,0,1,1,1,1,0,0,0,1,0,0,0,0,1,1,0,0,1,1,0,0,1,0,0,0,1,1,0,1,1,1,1,1,0,0,0,1,0,0,1,0,0,1,1,1,1,0,1,1,1,0,0,0,1,0,1,1,1,1,0,1,1,1,0,0,0,1,0,0,1,1,1,1,1,1,0,1,0,0,1,0,1,1,1,1,0,1,1,0,0,1,0,1,1,1,1,0,1,0,1,0,1,1,1,0,1,1,1,1,0,0,0,1,1,1,1,0,1,1,0,1,1,0,1,1,0,0,0,0,1,0,0,1,1,0,0,0,0,0,0,0,0,1,1,1,1,1,1,0,1,1,0,1,0,0,1,1,1,1,0,0,0,0,1,0,0,0,0,1,0,0,1,1,1,0,1,1,0,0,0,0,0,0,0,0,1,1,1,1,0,0,1,1,1,1,1,1,1,1,1,0,0,1,0,1,0,0,0,0,0,0,1,1,0,0,1,0,1,0,1,1,0,0,0,0,1,0,0,0,0,1,0,1,1,1,0,1,1,0,1,0,0,1,0,0,0,1,0,1,1,0,1,0,0,1,0,1,0,1,0,1,0,1,1,1,1,1,1,1,0,0,0,0,1,1,1,1,0,0,0,0,1,0,1,1,1,1,1,0,1,1,1,1,1,0,0,0,0,1,1,1,1,0,0,1,0,0,1,0,0,0,0,0,0,1,0,1,1,0,1,1,0,0,0,1,1,0,1,1,1,0,0,0,1,1,0,0,1,0,0,0,0,0,0,0,0,0,0,1,0,1,0,0,1,0,1,1,0,0,1,0,0,0,1,1,1,1,0,0,1,0,0,1,0,0,0,1,0,0,1,0,1,1,1,1,1,1,0,1,1,0,1,0,0,1,0,1,1,1,0,1,1,1,1,0,1,1,0,0,0,1,1,0,1,1,0,0,1,0,0,1,0,0,0,1,1,0,0,1,0,0,1,1,1,1,0,0,1,0,1,0,1,1,0,0,1,1,1,0,0,1,0,1,1,1,1,1,0,1,1,0,1,1,0,1,1,1,1,0,1,1,0,0,0,1,1,1,1,0,0,0,0,0,1,0,0,1,0,0,0,1,1,0,1,0,0,1,1,1,1,1,0,0,0,1,0,0,1,0,1,0,0,0,1,1,0,1,1,0,1,0,0,0,1,0,1,0,1,1,1,1,1,0,1,1,0,1,0,0,0,1,0,1,0,1,1,1,1,0,0,0,0,1,0,1,1,0,1,0,0,0,0,0,1,0,1,0,1,0,1,1,1,0,1,1,1,0,1,0,1,1,1,1,0,1,0,1,1,1,0,1,1,0,0,0,0,0,1,1,1,0,0,0,1,1,1,0,0,1,1,1,0,1,0,1,0,1,1,1,1,0,0,0,1,1,0,0,0,1,0,1,1,1,1,1,1,1,0,0,1,0,0,1,1,0,0,1,1,0,1,1,0,1,0,1,1,0,0,0,0,1,0,1,1,1,1,1,0,0,0,0,0,1,1,0,0,1,0,1,0,1,0,0,1,0,1,0,0,1,1,1,1,1,0,1,1,1,0,1,1,1,1,0,0,0,0,1,0,0,0,1,1,1,0,1,1,1,0,0,0,1,0,1,1,0,1,1,0,0,0,1,1,0,0,0,0,1,1,1,1,0,1,1,0,0,0,0,0,1,0,0,1,0,1,0,1,0,1,0,1,0,0,0,0,1,0,1,0,0,1,1,1,1,1,1,0,0,1,0,1,0,0,1,0,1,0,0,0,0,1,1,1,1,1,1,0,1,1,0,1,0,1,0,1,0,0,0,1,0,1,1,1,0,0,1,0,1,1,0,1,1,1,0,1,1,0,1,1,1,0,1,0,1,1,1,0,1,0,0,1,1,0,1,0,0,0,1,1,0,0,0,0,0,1,1,0,1,0,1,0,1,0,0,1,0,0,1,1,0,1,1,0,1,0,0,1,1,0,1,0,1,0,1,0,1,0,1,0,0,1,0,1,0,0,1,0,1,0,0,0,0,1,0,0,1,1,0,0,1,0,1,0,1,0,1,0,1,1,0,1,1,1,0,1,1,1,0,1,1,0,0,0,1,1,1,0,1,1,0,1,0,1,0,0,1,1,0,0,1,0,0,0,1,0,0,0,0,0,0,1,1,0,1,0,1,0,1,1,1,0,0,0,0,1,1,0,1,0,0,0,0,1,1,1,0,0,1,1,1,0,1,1,1,0,0,0,0,0,1,1,0,0,1,1,1,1,1,0,1,1,0,0,1,1,0,1,1,1,0,0,1,0,0,1,0,0,0,0,1,1,1,0,1,1,0,1,1,1,1,1,1,0,0,0,1,1,0,0,1,0,1,1,0,1,0,1,0,0,1,0,1,1,1,1,0,1,0,1,0,1,0,1,1,0,1,1,1,1,1,1,1,1,1,1,0,1,0,1,1,0,1,1,0,1,0,1,1,0,0,0,0,1,1,1,1,1,1,1,0,1,1,1,0,1,1,1,0,0,1,0,0,1,1,1,1,1,0,1,0,1,0,0,1,0,1,1,1,0,0,0,1,1,1,1,0,0,1,1,1,0,0,1,0,0,1,1,1,0,0,0,0,0,0,1,0,0,0,1,0,1,0,1,0,1,1,0,1,1,0,1,1,0,1,0,1,1,0,1,0,0,1,1,0,0,0,1,1,1,0,1,0,0,1,0,1,1,0,1,0,1,1,0,0,1,0,0,0,0,1,0,0,0,0,1,1,1,0,1,0,1,1,1,0,0,1,1,0,0,0,1,0,1,1,1,1,1,1,0,1,1,1,1,0,0,1,1,0,0,1,1,1,1,1,0,0,0,1,0,0,0,0,1,1,1,1,0,0,1,1,0,1,1,1,1,1,0,0,0,0,1,1,1,1,1,1,1,1,0,0,0,0,0,0,0,0,1,0,1,0,1,1,0,1,0,1,1,0,1,0,1,1,1,1,0,1,1,1,1,0,1,1,1,1,1,0,1,1,1,1,1,0,0,1,1,0,0,1,1,1,1,0,1,1,0,1,0,1,1,1,0,1,0,0,1,0,1,0,1,1,0,1,0,1,0,0,1,1,0,1,0,1,1,0,1,1,1,1,0,1,1,1,1,1,1,1,1,1,1,1,1,1,0,0,0,0,1,0,0,1,1,1,0,1,1,1,0,1,0,1,0,1,0,0,1,1,0,0,0,0,1,0,0,0,1,1,1,1,1,0,1,1,0,1,0,1,0,1,0,0,1,1,0,1,0,0,0,1,0,0,1,1,1,1,0,1,1,0,1,0,1,0,1,1,0,1,1,1,0,1,0,1,1,0,0,0,1,1,1,0,0,0,0,1,1,1,0,1,1,0,0,1,0,0,0,0,0,0,0,0,1,1,1,1,1,0,0,1,0,0,1,1,1,0,0,0,0,1,0,0,0,0,0,1,0,1,0,1,1,0,1,0,0,0,0,0,0,0,0,1,0,1,1,0,1,0,0,1,0,0,0,0,1,0,1,1,1,1,1,1,1,0,1,1,0,0,1,1,1,1,0,1,1,0,0,0,0,0,0,0,1,1,0,1,0,0,1,0,0,1,1,1,1,0,0,0,0,1,1,0,1,0,0,0,0,1,1,1,0,0,1,0,0,1,1,1,0,1,1,0,0,1,0,1,0,0,1,0,0,1,0,0,1,0,1,1,0,1,1,1,1,0,1,1,1,1,0,1,1,0,0,1,0,1,0,1,0,0,1,0,1,0,0,1,1,1,0,0,1,1,1,1,1,1,1,0,1,1,1,1,0,0,1,0,0,1,1,1,1,0,0,0,1,1,0,1,1,0,0,1,1,1,0,0,0,1,0,0,0,0,1,0,1,1,1,1,0,0,1,0,1,0,0,0,0,0,0,1,0,0,1,1,1,0,0,1,1,0,1,1,1,1,0,1,1,0,1,1,0,0,0,0,0,1,1,1,0,1,1,1,0,1,0,1,1,0,1,0,1,0,1,1,1,0,1,0,1,1,1,0,0,1,1,1,1,1,1,0,1,1,1,0,1,0,1,0,1,1,1,0,1,0,0,0,1,1,1,1,0,1,1,1,1,1,0,1,0,1,1,0,0,0,0,1,1,0,1,1,0,0,0,1,0,1,1,0,1,0,0,0,0,1,0,0,1,1,1,0,1,0,1,1,0,0,1,1,0,1,1,1,1,1,0,0,0,1,1,0,1,0,0,1,1,0,0,0,0,0,1,1,1,0,0,0,0,1,0,1,0,0,1,0,1,0,1,0,1,1,1,1,1,1,1,0,0,1,1,0,1,0,0,1,1,0,0,1,1,0,1,1,1,1,0,0,0,1,1,1,1,1,1,1,1,0,0,0,1,1,1,1,0,1,1,1,1,1,0,1,0,1,1,1,1,1,0,1,0,0,1,1,1,1,1,0,0,1,0,0,0]},"params":{"rows":["Gender"],"cols":["Country"]},"locale":"en","subtotals":false},"evals":[],"jsHooks":[]}</script>

<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>

[^1]: En realidad en castellano deber??a llamarlos cuadros, pero ???

[^2]: Evidentemente, en R hay muchos otros paquetes para hacer tablas b??sicas. Algunas de ellas son resumidas en este <a href="https://dabblingwithdata.wordpress.com/2017/12/20/my-favourite-r-package-for-frequency-tables/" target="_blank">post</a>
