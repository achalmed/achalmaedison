---
title: Definicion de ciencia de datos
author: Edison Achalma Mendoza
date: '2023-03-03'
slug: definicion-de-ciencia-de-datos
categories:
  - Data Science
tags:
  - Python
subtitle: ''
excerpt: 'En nuestra vida cotidiana, estamos constantemente rodeados de datos. El texto que estás leyendo ahora son datos. La lista de números de teléfono de sus amigos en su teléfono inteligente son datos, así como la hora actual que se muestra en su reloj. Como seres humanos, operamos naturalmente con datos contando el dinero que tenemos o escribiendo cartas a nuestros amigos.'
draft: yes
series: ~
layout: single
links:
  - icon: door-open
    icon_pack: fas
    name: website
    url: /
---

## ¿Qué son los datos?

En nuestra vida cotidiana, estamos constantemente rodeados de datos. El texto que estás leyendo ahora son datos. La lista de números de teléfono de sus amigos en su teléfono inteligente son datos, así como la hora actual que se muestra en su reloj. Como seres humanos, operamos naturalmente con datos contando el dinero que tenemos o escribiendo cartas a nuestros amigos.

Sin embargo, los datos se volvieron mucho más críticos con la creación de computadoras. La función principal de las computadoras es realizar cálculos, pero necesitan datos para operar. Por lo tanto, necesitamos entender cómo las computadoras almacenan y procesan los datos.

Con la aparición de Internet, el papel de las computadoras como dispositivos de manejo de datos aumentó. Si lo piensas, ahora usamos computadoras cada vez más para el procesamiento de datos y la comunicación, en lugar de cálculos reales. Cuando escribimos un correo electrónico a un amigo o buscamos alguna información en Internet, esencialmente estamos creando, almacenando, transmitiendo y manipulando datos.

> ¿Puedes recordar la última vez que usaste computadoras para calcular algo?

## ¿Qué es la ciencia de datos?

En [Wikipedia](https://en.wikipedia.org/wiki/Data_science), **la ciencia de datos** se define como *un campo científico que utiliza métodos científicos para extraer conocimientos y perspectivas de datos estructurados y no estructurados, y aplicar conocimientos y conocimientos procesables a partir de datos en una amplia gama de dominios de aplicación*. 

Esta definición destaca los siguientes aspectos importantes de la ciencia de datos:

* El objetivo principal de la ciencia de datos es **extraer conocimiento** de los datos, en otras palabras, **comprender** los datos, encontrar algunas relaciones ocultas y construir un **modelo**.
* La ciencia de datos utiliza **métodos científicos**, como probabilidad y estadística. De hecho, cuando se introdujo por primera vez el término *ciencia de datos*, algunas personas argumentaron que la ciencia de datos era solo un nuevo nombre elegante para las estadísticas. Hoy en día se ha hecho evidente que el campo es mucho más amplio.   
* El conocimiento obtenido debe aplicarse para producir algunos **conocimientos útiles**, es decir, conocimientos prácticos que puede aplicar a situaciones comerciales reales. * Deberíamos poder operar con datos tanto **estructurados** como **no estructurados**. Volveremos a discutir los diferentes tipos de datos más adelante en el curso. 
* **El dominio de la aplicación** es un concepto importante, y los científicos de datos a menudo necesitan al menos cierto grado de experiencia en el dominio del problema, por ejemplo: finanzas, medicina, marketing, etc.

> Otro aspecto importante de la ciencia de datos es que estudia cómo se pueden recopilar, almacenar y operar los datos usando computadoras. Si bien las estadísticas nos brindan fundamentos matemáticos, la ciencia de datos aplica conceptos matemáticos para extraer información de los datos.

Una de las formas (atribuida a [Jim Gray](https://en.wikipedia.org/wiki/Jim_Gray_(computer_scientist))) de observar la ciencia de datos es considerarla como un paradigma separado de la ciencia:
* **Empirico**, en el que nos basamos principalmente en observaciones y resultados de experimentos
* **Teórico**, donde surgen nuevos conceptos a partir del conocimiento científico existente
* **Computacional**, donde descubrimos nuevos principios basados ​​en algunos experimentos computacionales
* **Data-Driven**, basado en el descubrimiento de relaciones y patrones en los datos

## Otros campos relacionados

Dado que los datos son omnipresentes, la ciencia de datos en sí también es un campo amplio que toca muchas otras disciplinas.

<dl>
<dt>Bases de datos</dt>
<dd>
Una consideración crítica es **cómo almacenar** los datos, es decir, cómo estructurarlos de manera que permitan un procesamiento más rápido. Hay diferentes tipos de bases de datos que almacenan datos estructurados y no estructurados, que <a href="https://github.com/achalmed/Data-Science-For-Beginners/blob/main/2-Working-With-Data/README.md">consideraremos en nuestro curso</a>.
</dd>
<dt>Big Data</dt>
<dd>
A menudo necesitamos almacenar y procesar grandes cantidades de datos con una estructura relativamente simple. Existen enfoques y herramientas especiales para almacenar esos datos de manera distribuida en un clúster de computadoras y procesarlos de manera eficiente.
</dd>
<dt>Aprendizaje automático</dt>
<dd>
Una forma de comprender los datos es **construir un modelo** que pueda predecir el resultado deseado. El desarrollo de modelos a partir de datos se denomina **aprendizaje automático**. 
</dd>
<dt>Inteligencia Artificial</dt>
<dd>
Un área de aprendizaje automático conocida como inteligencia artificial (IA) también se basa en datos e implica la construcción de modelos de alta complejidad que imitan los procesos de pensamiento humano. Los métodos de IA a menudo nos permiten convertir datos no estructurados (por ejemplo, lenguaje natural) en información estructurada.
</dd>
<dt>Visualización</dt>
<dd>
Grandes cantidades de datos son incomprensibles para un ser humano, pero una vez que creamos visualizaciones útiles usando esos datos, podemos darles más sentido y sacar algunas conclusiones. Por lo tanto, es importante conocer muchas formas de visualizar información, algo que cubriremos en la <a href="../../3-Data-Visualization/README.md">Sección 3</a> de nuestro curso. . Los campos relacionados también incluyen **Infografía** e **Interacción humano-computadora** en general.
</dd>
</dl>

## Tipos de datos

Como ya hemos mencionado, los datos están en todas partes. ¡Solo tenemos que capturarlo de la manera correcta! Es útil distinguir entre datos **estructurados** y **no estructurados**. El primero generalmente se representa en una forma bien estructurada, a menudo como una tabla o un número de tablas, mientras que el segundo es solo una colección de archivos. A veces también podemos hablar de datos **semiestructurados**, que tienen algún tipo de estructura que puede variar mucho.

| Structured                                                                   | Semi-structured                                                                                | Unstructured                            |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | --------------------------------------- |
| List of people with their phone numbers                                      | Wikipedia pages with links                                                                     | Text of Encyclopedia Britannica        |
| Temperature in all rooms of a building at every minute for the last 20 years | Collection of scientific papers in JSON format with authors, data of publication, and abstract | File share with corporate documents     |
| Data for age and gender of all people entering the building                  | Internet pages                                                                                 | Raw video feed from surveillance camera |

## Dónde obtener datos

Hay muchas fuentes posibles de datos, ¡y será imposible enumerarlas todas! Sin embargo, mencionemos algunos de los lugares típicos donde puede obtener datos:

* **Estructurado**: 
  - **Internet de las cosas** (IoT), que incluye datos de diferentes sensores, como sensores de temperatura o presión, proporciona una gran cantidad de datos útiles. Por ejemplo, si un edificio de oficinas está equipado con sensores IoT, podemos controlar automáticamente la calefacción y la iluminación para minimizar los costos.  
  - **Encuestas** que solicitamos a los usuarios que completen después de una compra o después de visitar un sitio web. - 
  - **El análisis de comportamiento** puede, por ejemplo, ayudarnos a comprender qué tan profundo ingresa un usuario a un sitio y cuál es la razón típica para abandonar el sitio. 
* **No estructurado**: 
  - Los **textos** pueden ser una rica fuente de información, como una **puntuación de opinión** general o la extracción de palabras clave y significado semántico. 
  - **Imágenes** o **Video**. Se puede usar un video de una cámara de vigilancia para estimar el tráfico en la carretera e informar a las personas sobre posibles atascos de tráfico. 
  - Los **Registros** del servidor web se pueden usar para comprender qué páginas de nuestro sitio se visitan con más frecuencia y durante cuánto tiempo. 
* Semiestructurado: 
  - Los gráficos de **redes sociales** pueden ser excelentes fuentes de datos sobre las personalidades de los usuarios y la eficacia potencial en la difusión de información. 
  - Cuando tenemos un montón de fotografías de una fiesta, podemos intentar extraer datos de **Dinámica de grupo** construyendo un gráfico de personas tomándose fotos entre sí. 

Al conocer diferentes fuentes posibles de datos, puede intentar pensar en diferentes escenarios donde se pueden aplicar técnicas de ciencia de datos para conocer mejor la situación y mejorar los procesos comerciales.

## Qué puede hacer con los datos

En Data Science, nos centramos en los siguientes pasos del viaje de datos:

<dl>
<dt>1) Adquisición de datos</dt>
<dd>
El primer paso es recopilar los datos. Si bien en muchos casos puede ser un proceso sencillo, como los datos que llegan a una base de datos desde una aplicación web, a veces necesitamos usar técnicas especiales. Por ejemplo, los datos de los sensores de IoT pueden ser abrumadores, y es una buena práctica utilizar puntos finales de almacenamiento en búfer como IoT Hub para recopilar todos los datos antes de su posterior procesamiento.
</dd>
<dt>2) Almacenamiento de datos</dt>
<dd>
Almacenar datos puede ser un desafío, especialmente si estamos hablando de big data. Al decidir cómo almacenar datos, tiene sentido anticipar la forma en que consultaría los datos en el futuro. Hay varias formas en que se pueden almacenar los datos:
<ul>
<li>Una base de datos relacional almacena una colección de tablas y utiliza un lenguaje especial llamado SQL para consultarlas. Normalmente, las tablas se organizan en diferentes grupos llamados esquemas. En muchos casos, necesitamos convertir los datos del formulario original para que se ajusten al esquema.
</li>
<li> Una base de datos <a href="https://en.wikipedia.org/wiki/NoSQL">NoSQL</a>, como <a href="https://azure.microsoft.com/services/cosmos-db/?WT.mc_id=academic-31812-dmitryso">CosmosDB</a>, no aplica esquemas en los datos y permite almacenar datos más complejos, por ejemplo, documentos o gráficos JSON jerárquicos. Sin embargo, las bases de datos NoSQL no tienen las capacidades de consulta enriquecidas de SQL y no pueden imponer la integridad referencial, es decir, las reglas sobre cómo se estructuran los datos en tablas y gobiernan las relaciones entre tablas.</li>
<li><a href="https://en.wikipedia.org/wiki/Data_lake">El almacenamiento de Data Lake</a> se utiliza para grandes colecciones de datos en forma cruda y no estructurada. Los lagos de datos se utilizan a menudo con big data, donde todos los datos no pueden caber en una máquina, y tienen que ser almacenados y procesados por un clúster de servidores <a href="https://en.wikipedia.org/wiki/Apache_Parquet">Parquet</a> es el formato de datos que a menudo se usa junto con big data.
</li> 
</ul>
</dd>
<dt>3) Tratamiento de datos</dt>
<dd>
Esta es la parte más emocionante del viaje de datos, que implica convertir los datos de su forma original en una forma que se puede usar para la visualización / entrenamiento de modelos. Cuando se trata de datos no estructurados, como texto o imágenes, es posible que necesitemos utilizar algunas técnicas de IA para extraer **características** de los datos, convirtiéndolos así en forma estructurada.
</dd>
<dt>4) Visualización / Human Insights</dt>
<dd>
A menudo, para entender los datos, necesitamos visualizarlos. Al tener muchas técnicas de visualización diferentes en nuestra caja de herramientas, podemos encontrar la vista correcta para hacer una idea. A menudo, un científico de datos necesita "jugar con los datos", visualizándolos muchas veces y buscando algunas relaciones. Además, podemos utilizar técnicas estadísticas para probar una hipótesis o probar una correlación entre diferentes datos.   
</dd>
<dt>5) Entrenamiento de un modelo predictivo</dt>
<dd>
Debido a que el objetivo final de la ciencia de datos es poder tomar decisiones basadas en datos, es posible que deseemos utilizar las técnicas de <a href="http://github.com/microsoft/ml-for-beginners">Machine Learning</a> para construir un modelo predictivo. Luego podemos usar esto para hacer predicciones utilizando nuevos conjuntos de datos con estructuras similares.
</dd>
</dl>

Por supuesto, dependiendo de los datos reales, es posible que falten algunos pasos (por ejemplo, cuando ya tenemos los datos en la base de datos o cuando no necesitamos capacitación en modelos), o algunos pasos pueden repetirse varias veces (como el procesamiento de datos).

## Digitalización y Transformación Digital

En la última década, muchas empresas comenzaron a comprender la importancia de los datos al tomar decisiones comerciales. Para aplicar los principios de la ciencia de datos a la gestión de un negocio, primero se necesitan recopilar algunos datos, es decir, traducir los procesos de negocio a forma digital. Esto se conoce como **digitalización**.  ALa aplicación de técnicas de ciencia de datos a estos datos para guiar las decisiones puede conducir a aumentos significativos en la productividad (o incluso al pivote empresarial), llamado **transformación digital**.

Consideremos un ejemplo. Supongamos que tenemos un curso de ciencia de datos (como este) que impartimos en línea a los estudiantes, y queremos usar la ciencia de datos para mejorarlo. ¿Cómo podemos hacerlo?

Podemos empezar preguntándonos "¿Qué se puede digitalizar?" La forma más sencilla sería medir el tiempo que tarda cada alumno en completar cada módulo, y medir los conocimientos obtenidos dando una prueba de opción múltiple al final de cada módulo. Al promediar el tiempo de finalización en todos los estudiantes, podemos averiguar qué módulos causan las mayores dificultades para los estudiantes y trabajar para simplificarlos.

> Puede argumentar que este enfoque no es ideal, porque los módulos pueden ser de diferentes longitudes. Probablemente sea más justo dividir el tiempo por la longitud del módulo (en número de caracteres) y comparar esos valores en su lugar.

Cuando comenzamos a analizar los resultados de las pruebas de opción múltiple, podemos tratar de determinar qué conceptos tienen dificultades para entender los estudiantes, y usar esa información para mejorar el contenido. Para hacer eso, necesitamos diseñar pruebas de tal manera que cada pregunta se asigne a un determinado concepto o trozo de conocimiento.

Si queremos complicarnos aún más, podemos trazar el tiempo empleado para cada módulo en función de la categoría de edad de los estudiantes. Podríamos descubrir que para algunas categorías de edad se necesita un tiempo inapropiadamente largo para completar el módulo, o que los estudiantes abandonan antes de completarlo. Esto puede ayudarnos a proporcionar recomendaciones de edad para el módulo y minimizar la insatisfacción de las personas por las expectativas erróneas.

## 🚀 Challenge

En este desafío, trataremos de encontrar conceptos relevantes para el campo de la Ciencia de Datos mirando textos. Tomaremos un artículo de Wikipedia sobre Ciencia de Datos, descargaremos y procesaremos el texto, y luego construiremos una nube de palabras como esta:

Visite [`notebook.ipynb`](https://github.com/achalmed/Data-Science-For-Beginners/blob/main/1-Introduction/01-defining-data-science/notebook.ipynb) para leer el código. También puede ejecutar el código y ver cómo realiza todas las transformaciones de datos en tiempo real.

> Si no sabe cómo ejecutar código en un Jupyter Notebook, eche un vistazo a [este artículo](https://soshnikov.com/education/how-to-execute-notebooks-from-github/).


## Assignments

* **Tarea 1**: Modificar el código anterior para descubrir conceptos relacionados con los campos de **Big Data** y **Machine Learning**
* **Tarea 2**: [Pensar en escenarios de ciencia de datos](assignment.md)

## Credits

Esta lección ha sido escrita con ♥️ por [Dmitry Soshnikov](http://soshnikov.com) y [E Edison Achalma Mendoza] (https://github.com/achalmed)
