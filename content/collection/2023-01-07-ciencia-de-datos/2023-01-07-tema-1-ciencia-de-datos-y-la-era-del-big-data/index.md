---
title: 'Tema 1: Ciencia de datos y la era del Big Data'
author: Edison Achalma Mendoza
date: '2023-01-07'
slug: tema-1-ciencia-de-datos-y-la-era-del-big-data
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

El objetivo principal achi del curso es aprender un poco, todo lo que podamos, sobre una nueva disciplina: Ciencia de datos o Data Science. En concreto, nos centraremos en aprender a manejar y analizar datos utilizando una herramienta profesional como R. En el tema 2 hablaremos y utilizaremos intensivamente R, de momento nos sobra con señalar que R es un programa informático, más bien un entorno, con el que hacer análisis de datos (o ciencia de datos), pero R también es un lenguaje de programación. Lo veremos!!

Antes de empezar el cuerpo principal del curso voy a tratar de explicar, en este tema introductorio, qué significan términos que todos habéis oído como: Big Data, Inteligencia Artificial (IA), Machine Learning (ML), algoritmos, redes neuronales, etc… etc… Puff!!! Muchas cosas, pero … paso a paso.

## 1. ¿Qué es esto de la era del Big Data?

Pues no os voy a engañar, la principal razón de la presencia del término “Big Data” en el título del curso es que me parecía que como el título comienza con “Programación y manejo de datos …”, es posible que nadie se apuntase al curso, así que había que añadir al título un término de moda y un poco misterioso. ¿Estrategia de marketing? Un poco sí, pero en realidad todos los cursos de Ciencia de Datos que están apareciendo en el mundo, seguramente no habrían aparecido si no estuviésemos en la “era del Big Data”. En el curso no usaremos técnicas de Big Data pero sí hablaremos algo de ellas, principalmente en el tema 4.

Los tiempos están cambiando ([The Times They Are A Changin’](https://www.youtube.com/watch?v=-e7b09L4jY8)) decía Bob Dylan en el 64. Quizás los tiempos siempre han estado cambiando y siempre cambiarán, pero ahora mismo la mayoría de nosotros tenemos la sensación de que todo va muy deprisa. En mi opinión lo que está detrás de este cambio acelerado del mundo en muchos aspectos tiene que ver con la tecnología, fundamentalmente con los ordenadores y las redes que transmiten cantidades ingentes de datos.

Puede que nada ilustre más estos cambios que lo qué he hecho yo para continuar este razonamiento: en lugar de buscar un libro he buscado en Google “la era del Big Data”. En estos últimos años he leído bastante sobre el tema, pero para empezar a pensar me he ido a Google y he buscado el término. El tercer resultado me ha llevado a la Wikipedia (otro de los milagros disruptivos que hemos vivido en las dos últimas décadas). Igual que he hecho yo para informarme/documentarme, todos los días utilizamos software, aplicaciones para gestionar la agenda, escuchar radio, comprar, comunicarnos etc … La tecnología está presente en todos los aspectos de nuestra vida porque llevamos un ordenador, el teléfono móvil, en el bolsillo, y con él podemos comunicarnos y recibir y transmitir información a través de la redes. Esto es lo que ha cambiado el mundo y seguirá cambiándolo y afectará a todas las esferas de nuestra vida, espero que para bien (seguro!!). Pero claro, en el curso no vamos a hablar de todo esto, solo de trasfondo, sino que nos centraremos en los datos, en como tratar, manejar y obtener información de las grandes cantidades de datos que consumimos y generamos constantemente; así que, dejemos las posibles implicaciones sociales, políticas, filosóficas para otros cursos y bajemos a cosas más concretas.

### ¿Qué significa, qué es Big Data?

Pues es un término polisémico, tiene distintos significados. Luego seré más preciso y riguroso, pero de momento podemos pensar que Big Data significa que tenemos muuuuuuchos datos, muchos. Esta disponibilidad de datos es uno de los principales factores que explican porqué el desarrollo técnico se ha acelerado en los últimos tiempos.

Lo que ha pasado es que, el hecho de que los científicos dispongan ahora de muchos datos ha dado un fuerte impulso a un campo de la Inteligencia Artificial (concretamente el campo del Machine Learning/Deep Learning) que ha hecho que las máquinas, los ordenadores, los robots, puedan hacer cosas que antes eran inimaginables, como por ejemplo que Alexa nos entienda, que haya coches autónomos que conduzcan mejor que los humanos, que un ordenador gane al campeón mundial de ajedrez (esto paso ya hace mucho tiempo, en 1996, antes de la era del Big data [^1]).

En los medios, en la tele, se habla, aparece el término “la era del Big data” significando más o menos lo que os he contado, que la “abundancia de datos” está impulsando fuertemente el desarrollo tecnológico, de forma que ahora tenemos acceso a aplicaciones que hasta hace bien poco parecían ciencia ficción.

Este acelerado cambio técnico y sus aplicaciones, va a tener y está teniendo innumerables efectos en todos los ámbitos de nuestra vida y también en el de las empresas e industrias. Muchas industrias, como la del transporte van a ver como el escenario cambia y, muy posiblemente, las que no sepan entender y aprovechar los nuevos retos tecnológicos posiblemente acaben despareciendo; evidentemente esto genera, ya sea real o no, una urgencia en las empresas por intentar no quedarse fuera de este cambio acelerado y esto, en principio, genera mayor demanda de profesionales que sepan de tecnología y de datos. Bien, creo que ya tenemos un poco más claro que significa esto de “la era del Big Data”.

El término Big Data es relativamente nuevo, y en castellano se suele traducir como “Datos masivos”, aunque ahora mismo en la wikipedia pone “Macrodatos” y [aquí](https://www.fundeu.es/recomendacion/macrodatosalternativa-abig-data-1582/) recomiendan el uso del término Macrodatos. A mi personalmente no me acaba de gustar este término, pero quizás sea por el hecho de que tengo formación de economista, y el término macrodatos me recuerda a los datos macroeconómicos. En cualquier caso, el término usado habitualmente es el inglés: Big Data.

El término tiene matices, y variantes, pero para mi, la característica definitoria de datos Big es el hecho de que estos datos tengan tal volumen (o complejidad) que no “quepan”, que no puedan “manejarse” en un ordenador, en realidad que no puedan tratarse con las aplicaciones informáticas habituales. Tal y como figura en la Wikipedia: “es un término que hace referencia al concepto relativo a conjuntos de datos tan grandes y complejos como para que hagan falta aplicaciones informáticas no tradicionales de procesamiento de datos para tratarlos adecuadamente”

Luego hay “definiciones” más elaboradas como una famosa, de 2001 en la que se destacaban tres aspectos en el Big Data, **las tres “v’s”** del Big Data: **volumen, velocidad y variedad**: después se han añadido 2 uves más y se habla de 5 uves o 5 aspectos relacionados con el Big Data: **v**olumen de datos, **v**elocidad con la que se obtienen y transfieren, **v**ariedad de tipos de datos (texto, imágenes etc…), **v**eracidad de las fuentes, y un quinto aspecto a considerar es el **v**alor que aportan los datos. En [este texto](https://www.bbva.com/es/las-cinco-uves-del-big-data/) cortito lo explican bien.

Se pueden mirar más aspectos del Big data, pero lo fundamental es que son datos, que ya sea por su volumen, por su variedad, o por su velocidad no son fáciles de almacenar/tratar/manejar con las técnicas y ordenadores habituales. Este hecho da lugar a que el mercado, las empresas, necesiten personas que sean capaces de gestionar la infraestructura de hardware y software para manejar datos masivos, estas personas generalmente son ingenieros de software, o informáticos. Además de almacenar y distribuir los datos las empresas también necesitan personas que sean capaces de analizar y obtener información y valor de esos datos, el perfil de estas personas es menos uniforme, puede que sean ingenieros, matemáticos, estadísticos, economistas (why not?), biólogos, sí en Biología con el estudio del genoma y los genes es uno de los campos donde más se está haciendo Ciencia de Datos.

En cualquier caso, como es un área o campo de estudio relativamente nueva y además en constante evolución, los términos y conceptos aún están definiéndose y evolucionando; por ejemplo, ya se empieza a hablar del [“smart data”](https://retina.elpais.com/retina/2018/01/12/tendencias/1515763421_780579.html). En este artículo señalan que:

> “El término big data … hace referencia a conjuntos de datos que, debido a su gran volumen, necesitan sistemas especializados de almacenado y procesado para poder trabajar con ellos de manera eficiente …. La información es importante, sí, pero demasiada puede llegar a ser confusa y hasta contraproducente …. Aquí es donde el big data da un paso hacia adelante, el smart data, que se encarga de detectar señales y patrones relevantes a través de algoritmos inteligentes”.

Esto a mí me suena al objetivo fundamental de la Ciencia de Datos, extraer información a partir de los datos de forma que se genere conocimiento y/o valor.

Muchas veces si leéis un articulo relacionado con “el Big Data” aparecen palabras extrañas: Keras, TensorFlow, Apache, ApacheSpark, Mongo, MongoDB, Maria, Cassandra, …. y muchísimas más. Yo conozco algunas un poco, otras me suenan y otras me suenan a chino. ¿Qué son? Pues en general son nombres de aplicaciones informáticas, o repositorios de datos, o empresas, o paquetes, frameworks, …, que se utilizan para almacenar/tratar/manejar/estimar modelos con grandes volúmenes de datos. Por ejemplo [Apache](https://es.wikipedia.org/wiki/Apache_Software_Foundation) es una fundación de software libre, que se ocupa de hacer proyectos que en la práctica posibilitan hacer Big data, implementar los nuevas técnicas, con software y plataformas open source. Como la fundación Apache tiene muchos proyectos y “productos”, por eso hay ApacheSpark, Cassandra, Geronimo etc…

Esta infraestructura, tanto física (ordenadores, repositorios), como de software/programas que se utilizan en Big Data cambian muy deprisa. Constantemente están surgiendo nuevas empresas, nuevos métodos, un nuevo algoritmo, una nueva implementación de algo ya existente, etc…

Nos acaba de parecer otra palabra importante en este campo de conocimiento, los **algoritmos**, ya hablaremos de ellos y su importancia en “la era del Big Data”.

Quiero llamaros la atención sobre varias ideas que, como muchísimas otras no trataremos en el curso [^2], algunas de ellas provienen de [este artículo](https://www.infobae.com/opinion/2018/08/22/la-ciencia-de-los-datos-y-su-impacto-en-la-economia-la-politica-y-la-sociedad/):

- Los datos hoy son omnipresentes y a menudo abrumadores. Producimos, organizamos y consumimos datos de manera casi constante. Estamos rodeados de información que no para de aumentar. Una de las principales fuentes de datos son nuestras acciones en la red (clicks, likes, rating, shares, etc… ), pero también hay muchos datos provenientes de sensores en máquinas y procesos, piensa por ejemplo en la información que genera un coche de Formula 1, o un sonda espacial, o el VAR que hay en el fútbol. A modo de ejemplo, [Data Never Sleeps 8.0 de Domo](https://www.domo.com/learn/infographic/data-never-sleeps-8) informó que en cada minuto de 2020 hubo, usando datos solamente de la la plataforma Zoom, un promedio de 208.333 personas conectadas en una reunión virtual y se crearon 347.222 historias en Instagram.

- De la misma forma que Internet cambió radicalmente el mundo al añadir comunicación, los datos masivos modificaran aspectos fundamentales de nuestra vida otorgándole una dimensión cuantitativa que nunca había tenido antes, piensa por ejemplo en aplicaciones médicas o de monitorización de la actividad física. Ante tal volumen de datos, el desafío es construir conocimiento usando los datos más relevantes y diversos, no solo para nosotros, sino para nuestra sociedad en su conjunto.

- Hasta hace algunas décadas la recopilación de la información estaba mayormente a cargo de los Estados nacionales, pero, ahora mismo, gran parte de los datos están en manos de empresas privadas (Google, Facebook, Amazon, … ). Esto tiene y puede tener fuertes implicaciones y consecuencias.

- El poseer datos puede dar poder/beneficio/ventajas competitivas a quien los posea. Por ejemplo, según los expertos, el mejor traductor online no es Google Translator sino [DeepL](https://www.deepl.com/es/translator). Los dos servicios utilizan algoritmos de inteligencia artificial, pero parece ser que DeepL tiene mejores datos. DeepL utiliza los datos del proyecto Linguee que ha permitido construir una base de datos enorme. Lo explican [aquí](https://www.xataka.com/servicios/deepl-vs-google-translate-quien-gana-batalla-traductores-online)

- El ejemplo anterior ilustra que lo que hay detrás de los avances no son los algoritmos o la IA/ML/DL, sino los datos: el gran volumen de datos es lo que ha hecho posible esta época de avances tecnológicos acelerados; en este sentido se suele decir que [los datos son el nuevo petroleo](https://www.europeandataportal.eu/en/highlights/ode-open-data-benefits-open-data-compared-oil), pero a diferencia de este, cuyas reservas podemos considerar fijas, el volumen de datos no hace sino crecer, son más fáciles de transportar y generan más valor para la sociedad cuanta más gente los usa.

- Obviamente, la gran disponibilidad de datos tiene también aspectos más oscuros o con potenciales peligros, como por ejemplo aspectos legales en la seguridad y [privacidad](https://www.youtube.com/watch?v=pT19VwBAqKA&feature=youtu.be), o sesgos en los datos. Ya no sólo que los gobiernos corten internet o espíen a los ciudadanos, como por ejemplo el caso Snowden o el plan de crédito social chino, sino que está emergiendo un [mercado de espionaje digital](https://www.vice.com/en_us/article/ne879z/i-tracked-someone-with-license-plate-readers-drn).

En [este post](https://www.forbes.com/sites/neilmalhotra/2019/07/01/making-sure-ai-is-socially-responsible/#6a96f16c660c) hablan de cómo favorecer que las aplicaciones surgidas de la IA sean socialmente responsables o que los algoritmos no acaben reproduciendo los sesgos presentes en los datos. En [esta guía para el diseño responsable de sistemas de IA](https://www.turing.ac.uk/sites/default/files/2019-06/understanding_artificial_intelligence_ethics_and_safety.pdf) del Alan Turing Institute desarrollan estás ideas.

- Cuando se dispone de datos sensibles, por ejemplo datos médicos, aparece el dilema entre privacidad e información que puede ser beneficiosa para la sociedad. Siempre se puede tratar de anonimizar los datos, pero parece ser que a los expertos les resulta no demasiado complicado recuperar la información original; es decir, a veces es posible la [reidentificación](https://www.datanalytics.com/2019/08/27/mas-sobre-la-anonimidad-y-reidentificacion-en-ficheros-de-microdatos/) de ficheros anonimizados. Más sobre esto [aquí](https://www.youtube.com/watch?v=pT19VwBAqKA) y [aquí](https://hipertextual.com/2019/09/privacidad-diferencial-datos?utm_medium=feed&utm_source=feedpress.me&utm_campaign=Feed%3A+hipertextual).

- Como en otras facetas de la vida, la información y transparencia es clave a la hora de reducir los posibles riesgos de las aplicaciones de IA. Es importante que el código fuente de las aplicaciones y algoritmos sea de acceso libre. Como ejemplo [este artículo](https://www.publico.es/sociedad/transparencia-gobierno-no-quiere-publicar-funcionan-aplicaciones-algoritmos-debera-explicar.html) de Público o este [paper](https://www.tandfonline.com/doi/full/10.1080/1369118X.2018.1477967).

<br>

## 2. IA, ML y DL

Inteligencia Artificial (IA), Machine Learning (ML) y Deep Learning (DL) [^3] son tres palabras/conceptos que aparecen constantemente en la era del Big Data. [Aquí](https://blogthinkbig.com/artificial-intelligence-machine-learning-y-deep-learning-conoces-las-diferencias) tienes un post sencillo y claro sobre estos tres términos.

La primera idea a retener está resumida en la infografía que veis más abajo y que proviene de este [post](https://hackernoon.com/are-you-using-the-term-ai-incorrectly-911ac23ab4f5)

Como se aprecia en la infografía, DL es un subconjunto del ML y ML es un campo de la IA. Vamos que tanto DL como ML son aplicaciones específicas de IA. La IA surgió en los 50 y el ML puede verse como un enfoque de la IA que empezó a coger fuerza en los 80 y que supuso un cambio de paradigma en como se afrontaba la IA.

Primero veamos qué es la IA. Para ello voy a recurrir de nuevo a la [Wikipedia](https://es.wikipedia.org/wiki/Inteligencia_artificial) y a lo que ya sé sobre IA para redactar unos párrafos que os den cierta idea de qué es la IA.

La Wikipedia empieza diciendo: “IA es la inteligencia llevada a cabo por máquinas”. Esta primera frase no aclara mucho, pero es que a veces la cosas cuestan. Lo intento yo: IA es un campo de conocimiento, compartido por varias ciencias, cuyo objetivo podemos pensar qué es que la maquinas sean inteligentes. Las maquinas no son humanos, nunca van a poder ser inteligentes en un sentido amplio o humano, sólo en la ciencia-ficción, pero sí pueden tener comportamientos “inteligentes”; es decir que hagan cosas que simulen la inteligencia humana como por ejemplo resolver problemas o dicho de forma más técnica, en función de unas variables de entorno tomar una decisión (esto es lo que hace por ejemplo un ordenador que juega al ajedrez, en función de las posiciones de las piezas en el tablero toma una decisión sobre que pieza mover). Una definición concisa del campo sería: el esfuerzo por automatizar las tareas intelectuales normalmente realizadas por los seres humanos.

La idea fundamental en que se basa la Inteligencia Artificial es conseguir que una computadora resuelva un problema complejo como lo haría un humano. Es decir, según Andreas Kaplan y Michael Haenlein definen la inteligencia artificial es “la capacidad de un sistema para interpretar correctamente datos externos, para aprender de dichos datos y emplear esos conocimientos para lograr tareas y metas concretas a través de la adaptación flexible”. Por ejemplo, conducir un coche.

¿Desde cuando existe la inteligencia artificial? Pues desde hace bastante ….. no habíais nacido, ni yo tampoco.

La inteligencia artificial nació en la década de 1950, cuando un puñado de pioneros del campo de la informática comenzó a preguntarse si las computadoras podían “pensar”, una pregunta cuyas ramificaciones se están explorando todavía hoy. La idea principal que subyace al campo de la IA es conseguir que una computadora resuelva un problema o tarea compleja como lo haría un humano.

Durante las primeras etapas, mediados de los 60, se pensaba que la IA podría lograrse elaborando un conjunto suficientemente grande de reglas explícitas para manipular conocimiento o datos. En esta fase, se desarrollaron aplicaciones conocidas como **sistemas expertos**, en los que se creía que un potente ordenador y un conjunto de reglas de razonamiento podrían emular el razonamiento humano. Este enfoque se conoce como IA simbólica, y fue el paradigma dominante en IA hasta finales de los 80.

La IA simbólica demostró ser adecuada para resolver problemas lógicos bien definidos, como jugar al ajedrez, pero resultó difícil encontrar reglas explícitas para resolver otro tipo de problemas complejos y difusos, como la clasificación de imágenes, el reconocimiento de voz o la traducción de textos; de forma que hoy en día se utiliza otro enfoque: el Machine Learning o Aprendizaje Maquina.

Como señalan [aquí](https://empresas.blogthinkbig.com/atrevete-con-el-deep-learning/), no fue hasta los años 80, casi 30 años después del los inicios de la IA, que empezó a cobrar importancia el aprendizaje automático o Machine Learning. Se trata de una forma de IA que ya no necesita un programador que codifique reglas, sino que es capaz de establecer sus propias reglas y aprender por sí misma.

La idea básica detrás del ML consiste en que, en lugar de darle al ordenador un conjunto de reglas para procesar los datos, es el propio ordenador el que aprende esas reglas mirando/analizando los datos. ¿Cómo? Ya lo veremos, pero lo que está claro es que el enfoque/paradigma ha cambiado: en lugar de programar y dar al ordenador unas reglas o programa para procesar los datos y devolvernos respuestas/acciones, el enfoque del ML provee a la maquina con los datos y las respuestas esperadas con esos datos y nos devuelve las “reglas”. Estas reglas pueden aplicarse a nuevos datos para producir las respuestas en esos nuevos datos. Un sistema que usa ML no es explícitamente programado, sino que se le provee de suficientes datos (relevantes para la tarea que se espera que haga) y encuentra las reglas (o estructura estadística) en esos datos o ejemplos y, si todo funciona bien, el sistema aprende y encuentra las reglas/patrones para poder automatizar la tarea y que sea llevada a cabo por la máquina. Un sistema/programa de ML es entrenado más que explícitamente programado.

Un ejemplo puede ayudar a entenderlo: ¿Cómo se enseña a un niño qué es un gato y qué es un perro? No se le provee de reglas, no se le dice, mira un gato tiene dos orejas puntiagudas, bigotes, cola y cuatro patas; generalmente se le enseña al niño con ejemplos, se le enseñan fotos de gatos y perros y es el propio niño quien aprende las reglas de forma que sin que nadie le diga nada, cuando ve un gato por la calle lo identifica, quizás al principio se equivoca pero conforme se le dan más ejemplos acaba aprendiendo a reconocer/etiquetar a los gatos. Conforme el niño practica, cada vez lo hace mejor; es decir, aprende. Lo que es destacable es que no es necesario enseñar ninguna regla al niño; es decir, parece que los humanos tenemos “de serie” mecanismos de clasificación, podemos inferir reglas de clasificación, reglas que usamos pero que nos es difícil describir.

Este es el enfoque que utiliza el ML, no se programan las reglas (o características) del problema o cuestión a analizar (identificar gatos), sino que se le provee de datos (fotos de gatos y de perros) correctamente etiquetadas y mediante técnicas estadísticas/algoritmos él sólo encuentra las reglas para diferenciar entre perros y gatos. Una vez el programa/ordenador ha encontrado las reglas, se le pueden pasar nuevas fotos de perros y gatos (está vez sin etiquetar) y él las etiquetará. En cierta forma el ordenador ha aprendido de los datos y sabe diferenciar gatos de perros. Esta capacidad de generalizar, de aplicar los conocimientos adquiridos a través de la formación a ejemplos y situaciones nuevos, es una característica clave tanto del aprendizaje humano como del aprendizaje automático. Por supuesto, el aprendizaje humano es mucho más sofisticado que los algoritmos más avanzados de aprendizaje automático, pero las computadoras tienen la ventaja de tener mayor capacidad para el procesado de datos.

Los científicos que trabajan el campo del ML/DL utilizan técnicas de ML para elaborar aplicaciones o programas que funcionen para resolver/hacer una tarea concreta, como por ejemplo detectar spam, sugerir una ruta de tráfico, clasificar una imagen, traducir un texto, reconocer el lenguaje hablado, etc… [Aquí](https://www.youtube.com/watch?v=kopoLzvh5jY) puedes ver a dos inteligencias artificiales aprendiendo a jugar al escondite. Después de unas cuantos millones de partidas han aprendido bastante bien, incluso a colaborar para esconderse mejor En [este artículo](https://www.technologyreview.com/s/614325/open-ai-algorithms-learned-tool-use-and-cooperation-after-hide-and-seek-games/) lo explican un poco.

En el campo del ML/DL se utilizan técnicas estadísticas/algoritmos de aprendizaje. Hay muchos tipos de ellos. La elección del más adecuado, dependerá del tipo de tarea que se quiera resolver en cada caso. Por ejemplo, podemos hablar de algoritmos de clasificación como los árboles de decisión, o Naïve Bayes, algoritmos de regresión, de clustering, de análisis de componentes principales, redes neuronales, …

Con ML no nos encontraremos con ordenadores que piensan en el sentido humano, solamente estaremos utilizando el poder de computo de los ordenadores para obtener información a partir de un conjunto de datos; en realidad estamos usando ML para dar sentido a los datos[^4]. Las técnicas de ML se pueden aplicar a muchos campos, desde la política hasta las neurociencias. Es una herramienta que se puede aplicar a muchos problemas. Cualquier campo que necesite interpretar y actuar sobre los datos puede beneficiarse de las técnicas de aprendizaje automático. De hecho, estas técnicas, principalmente las de aprendizaje profundo, se están convirtiendo en el motor que impulsa la economía moderna basada en datos y para que ese motor funcione se necesita “energía”, y la energía la proporcionan los datos. En ese sentido se dice que los datos son el nuevo petroleo. Lo importante no son tanto las técnicas, sino los datos que alimentan a los algoritmos.

Las técnicas de ML/DL esencialmente sirven para hacer **predicciones**, en general, no permiten obtener la causa de algo. Los datos masivos tratan del qué, no del porqué. No se obtienen relaciones de **causalidad** sino correlaciones o asociaciones. Bueno … a todos nos gusta conocer las causas, sobre todo a los investigadores, pero, quizás, muchas veces esto no sea absolutamente necesario y aunque esto choque con las prácticas establecidas hace siglos y con nuestra comprensión más elemental sobre como tomar decisiones y aprehender la realidad. Siendo un poco abogado del diablo, no siempre necesitamos saber la causa; además, el método científico tradicional se limitaba a contrastar un limitado número de hipótesis mientras que con las técnicas de ML/DL el enfoque consiste, en cierta forma, en dejar que los datos hablen por si mismos.

Respecto al **Deep Learning**, simplemente volver a decir que es un subconjunto del ML. Son técnicas más complejas en términos computacionales y por lo tanto necesitan para aprender un mayor volumen de datos, pero su filosofía es la misma: proveer de datos para que el ordenador aprenda a resolver y automatizar una tarea concreta. Utilizan algoritmos más complejos o con más elementos o capas. Prácticamente todas las aplicaciones exitosas utilizan técnicas de DL, y generalmente algoritmos basados en redes neuronales.

Os dejo algunas ideas frases sobre DL provenientes de [este fantástico artículo](https://empresas.blogthinkbig.com/atrevete-con-el-deep-learning/):

- El Deep Learning es una de las áreas de investigación más populares dentro del campo de la Inteligencia Artificial en los últimos años porque, gracias a estas técnicas, cosas como la visión artificial o el procesamiento del lenguaje natural han saltado del ámbito de la ciencia ficción a la realidad.

- El Deep Learning es tan importante porque está permitiendo resolver de forma más fácil y eficiente un gran número de problemas. Por una parte, realiza de forma automática una de las tareas más complejas del proceso de trabajo de Machine Learning: la ingeniería de atributos[^5]. Las redes neuronales seleccionan de forma automática qué atributos son los relevantes y cuáles se pueden desechar.

- Otra de las grandes ventajas de trabajar con redes neuronales es que permiten trabajar con cualquier tipo de input. Cualquiera: números, imágenes, sonidos, textos, series temporales. Teniendo en cuenta que los datos no estructurados, aquellos que no encajan en la estructura tradicional filas/columnas de las bases de datos relacionales, suponen más de un 90% de todos los datos generados, es fácil comprender la importancia de poder manejarlos de forma eficiente. Estamos hablando de datos como mensajes de correo, vídeos, ficheros de audio, páginas web, mensajes en redes sociales etc.

- Una red neuronal entrenada con datos etiquetados, también se puede aplicar a datos no estructurados, lo cual les da a los algoritmos de Deep Learning una gran ventaja respecto a otros algoritmos al poner a su disposición un volumen de datos de entrenamiento mucho mayor. Algoritmos no muy buenos entrenados con enormes conjuntos de datos pueden dar mejores resultados que buenos algoritmos entrenemos con conjuntos de datos reducidos. De hecho, mientras en el caso de los algoritmos tradicionales usados en Machine Learning llega un momento en el un mayor volumen de datos no implica un mejor rendimiento, en el caso del Deep Learning no ocurre así. El rendimiento no deja de crecer, según lo hacen el volumen de datos y el número de capas del modelo.

Como ya sabéis, aunque el curso tiene un tema sobre ML, el tercero, en el que se hará una introducción a la terminología y principales métodos del ML, en realidad el curso no está orientado al ML, ni mucho menos al DL, sino que está más orientado a ser una introducción a la ciencia de datos (DS).

¿Que qué es la Ciencia de datos? Pues voy a tratar de explicarlo en el siguiente apartado.

## 3. Ciencia de Datos

Como se dijo en el prefacio, DS es una nueva disciplina[^6] que se incorpora poco a poco, pero con mucha fuerza, a la mayoría de planes de estudio, incluida la Economía. Por ejemplo, [este Máster de la LSE](http://www.lse.ac.uk/study-at-lse/Graduate/Degree-programmes-2019/MSc-Data-Science).

¿De qué se ocupa la ciencia de datos? Pues puede tener varias respuestas, pero en definitiva el objetivo último de la ciencia de datos es transformar los datos en información con sentido. Algunos dirán, pero sí ese es el objetivo de la Estadística. Sí, es cierto, transformar datos en información es, y ha sido siempre, el objetivo último de la estadística, PERO lo que habitualmente conocemos por Estadística se fue conformando con el paso de los años en un contexto en el que conseguir datos era difícil, así que se desarrollaron métodos y técnicas apropiadas para extraer el máximo de información con muestras de reducido tamaño. El contexto ha cambiado, vivimos rodeados de datos, de mayor volumen y variedad, lo que provoca nuevos retos a los analistas, y tenemos mayor capacidad de computo, por lo que a veces ya no hay que utilizar aproximaciones asintóticas[^7]. La American Statistical Asociation (ASA) destaca la importancia de la Estadística en DS, pero reconoce en [este statement](https://magazine.amstat.org/blog/2015/10/01/asa-statement-on-the-role-of-statistics-in-data-science/) la diferencia entre DS y estadística.

No es estrictamente cierto, pero podemos pensar que la estadística tradicional se concentra principalmente en las técnicas o métodos estadísticos, además dado el contexto de escasez de datos, en un tipo determinado de técnicas; sin embargo la óptica de la ciencia de datos es más amplia. En Ciencia de datos se usan y necesitan técnicas estadísticas, pero el enfoque es más global: se hace énfasis en que el proceso de análisis de datos comienza desde que se recopilan los datos hasta que se presentan los resultados[^8]. El siguiente diagrama ilustra este proceso:

En la Ciencia de datos, etapas como el procesado y limpieza de datos o el análisis gráfico, que ocupaban un lugar secundario cuando no marginal en los libros tradicionales de estadística se han convertido en partes fundamentales del trabajo de un científico de datos.

No solo se considera el análisis de datos como un proceso más global compuesto de varias etapas, sino que dada la complejidad, volumen y variedad de los datos actuales se necesita un fuerte componente tecnológico generalmente apoyado en los ordenadores y la programación. No se puede, o es extremadamente complicado, hacer ciencia de datos sin saber programar. Además en la ciencia de datos se da una gran importancia al contexto en el que se hace Data Science, en cierta forma se reconoce que hace falta saber Economía para hacer ciencia de datos en el campo de la economía.

La siguiente infografía puede ilustrar esta idea, mostrando que, idealmente, para hacer DS se requieren, al menos, tres tipos de competencias o conocimientos: 1) matemáticas y estadística, 2) tecnología y programación y 3) conocimientos del campo de aplicación. En [este post](http://drewconway.com/zia/2013/3/26/the-data-science-venn-diagram) explican el diagrama en detalle, por ejemplo, qué es la “Danger Zone”.

En [este post](https://medium.com/@ODSC/data-science-in-manufacturing-an-overview-e6d648bf9c08) desarrollan estas ideas en el contexto concreto de la industria manufacturera y hacen un listado de potenciales usos de la DS en el campo de las manufacturas. En [este otro post](http://varianceexplained.org/r/ds-ml-ai/) puedes encontrar una visión de la DS un poco distinta, ya que incide en la diferencias entre DS, ML e IA. Como resumen del post: “Data science produces insights, Machine learning produces predictions, Artificial intelligence produces actions”. En este [otro post](https://blog.rstudio.com/2020/05/27/role-of-the-data-scientist/) argumentan que los científicos de datos son más necesarios que nunca y que su labor no puede, al menos de momento, ser reemplazada por procesos automatizados usando técnicas de ML.

Dos definiciones sencillas de DS:

- `@YBuhl`: This phrase by `@juliesquid` is worth retweeting it all over again:
  “Data Science is not just about \#AI or machine learning. It is the discipline of turning raw data into understanding.”

- `@TiffanyTimbers`: Thinking a lot about the definition of \#DataScience. The best that I have read so far comes from `@rafalab`: “the processes used to extract value from data”. I think we should extend this and say “the reproducible & transparent processes used to extract value from data”

Por último, 3 “definiciones” de DS medio en broma:

- Un científico de datos es un estadístico con pajarita

- Un estadístico que trabaja en San Francisco

- Científico de datos (n): Persona que sabe más de estadística que cualquier programador y que a la vez sabe más de programación que cualquier estadístico

<br>

#### ¿Es fácil ser científico de datos?

Pues, como todo, depende, pero si que hay que tener en cuenta que es un campo en continúa evolución. Estos post, [1](https://towardsdatascience.com/how-it-feels-to-learn-data-science-in-2019-6ee688498029), [2](https://muestrear-no-es-pecado.netlify.com/2019/02/18/la-modernidad/) y [3](https://github.com/oliviergimenez/Things-a-scientist-is-suppposed-to-know), inciden en lo estresante que puede ser la vida de un científico de datos que intente estar al día de las continuos cambios y evoluciones en este campo.

Parecido a lo que sugiere este tweet:

<blockquote class="twitter-tweet">
<p lang="en" dir="ltr">
Why Data Science is Hard™<br><br>(slide via <a href="https://twitter.com/bradurani?ref_src=twsrc%5Etfw">(**bradurani?**)</a> at <a href="https://twitter.com/hashtag/LeadDevAustin?src=hash&amp;ref_src=twsrc%5Etfw">\#LeadDevAustin</a>) <a href="https://t.co/8QcPlRMazw">pic.twitter.com/8QcPlRMazw</a>
</p>
— Caitlin Hudon👩🏼
💻 ((**beeonaposy?**)) <a href="https://twitter.com/beeonaposy/status/1070787394289446912?ref_src=twsrc%5Etfw">December 6, 2018</a>
</blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<br>

Aunque también está bien desmitificar un poco y tomarse las cosas menos en serio:

<blockquote class="twitter-tweet">
<p lang="en" dir="ltr">
Love data science <a href="https://t.co/RZ18jaOJRQ">pic.twitter.com/RZ18jaOJRQ</a>
</p>
— Tim Hopper ((**tdhopper?**)) <a href="https://twitter.com/tdhopper/status/730425632862044161?ref_src=twsrc%5Etfw">May 11, 2016</a>
</blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<br>

Como sugiere este otro tweet, no se puede saber todo, ni pasar por la vida sin cometer errores:

<blockquote class="twitter-tweet">
<p lang="en" dir="ltr">
Vulnerable but important tweets for data scientists & programmers:<br><br>🤷IDK: I don't know<br>🧠TIL: today I learned<br>😬 Mistakes I've made<br><br>Normalizing the fact that no one knows it all (not even you!), everyone makes mistakes, and learning is a lifelong process has profound impacts.
</p>
— Jesse Mostipak ((**kierisi?**)) <a href="https://twitter.com/kierisi/status/1068496229439598592?ref_src=twsrc%5Etfw">November 30, 2018</a>
</blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<br>

Para finalizar, un hilo de Tweeter con muuuuuuchos errores:

<blockquote class="twitter-tweet">
<p lang="en" dir="ltr">
A small sample of data science mistakes I've made so far 👇 <a href="https://t.co/EeiVmmAnuJ">pic.twitter.com/EeiVmmAnuJ</a>
</p>
— Caitlin Hudon👩🏼
💻 ((**beeonaposy?**)) <a href="https://twitter.com/beeonaposy/status/1122964504910938121?ref_src=twsrc%5Etfw">April 29, 2019</a>
</blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<br>

## 4. Ciencia de datos en Economía

Evidentemente todo este cambio tecnológico acelerado al que asistimos en la era del Big Data, y que muchas veces está asociado al ML/DL, ha provocado y provocará grandes cambios tanto en la economía real como en la ciencia económica. Una panorámica de trabajos que analizan las implicaciones de estos cambios en la ciencia económica puede verse en [Análisis económico de la revolución digital](https://blog.funcas.es/wp-content/uploads/2018/11/Economic-Analysis-of-the-Digital-Revolution.pdf).

Uno de los efectos más evidentes consiste en que las innovaciones tecnológicas asociadas al ML seguramente cambiarán radicalmente, si es que no lo han hecho ya, muchos sectores económicos; por ejemplo el transporte o la banca, pero también muchos otros como los seguros, servicios audiovisuales, la venta al por menor, la sanidad, etc…

Otro de los cambios más evidentes consiste en que actualmente las principales corporaciones transnacionales, que antes pertenecían principalmente a los sectores energético y financiero, ahora tienen un fuerte componente tecnológico, las **GAFA**, un acrónimo para hacer referencia a las cuatro grandes compañías tecnológicas: Google, Amazon, Facebook y Apple.

Otra de los cambios significativos que han sido propiciados por las nuevas tecnologías es la llamada **economía colaborativa** al que están asociadas empresas como BlaBlaCar, Airbnb, …

Otro cambio evidente consiste en que ahora mismo hay una economía de los datos. Los datos se han convertido en materia prima, capaz de crear valor, fuente de innovación y servicios nuevos. Para una panorámica de está economía de los datos puede verse la publicación [Economía de los Datos. Riqueza 4.0](https://www.fundacioncarolina.es/wp-content/uploads/2018/11/Libro-Economia-de-los-Datos-Ontiveros.pdf).

Se habla incluso de que estamos inmersos en una **cuarta revolución industrial**. El concepto de cuarta revolución industrial fue acuñado por Klaus Schwab fundador del Foro Económico Mundial en el contexto de la edición del Foro Económico Mundial 2016 y una de sus características es la utilización de la IA/ML/DL para la automatización de tareas que antes sólo estaban al alcance de los humanos. Una de las consecuencias más directas de la automatización será el **desplazamiento de empleos**, no sólo manuales, por las maquinas/algoritmos.

Desde el punto de vista de la ciencia, la actual abundancia de datos, va a tener implicaciones directas:

- “De la misma forma que el telescopio y el microscopio permitieron ver el espacio y las células, las nuevas técnicas de recopilación y análisis de datos ayudarán a ver el sentido de nuestro mundo de una forma que apenas intuimos”.

- “el cambio cuantitativo no es lo único importante, es el cualitativo: una película es diferente de una pintura, también cuando trabajas con muchos datos se pueden hacer otras cosas; es decir, al cambiar la cantidad cambiamos la esencia”.

Ha surgido, incluso, una nuevo término: el [dataísmo](https://es.wikipedia.org/wiki/Data%C3%ADsmo). Para un “dataista”, en un mundo con cada vez mayor complejidad, confiar en los datos puede reducir los sesgos cognitivos y descubrir patrones de comportamiento. Según el filósofo y ensayista surcoreano Byung-Chul Han, “el big data” debe liberar el conocimiento de la subjetividad. El término dataismo fue popularizado en el libro Homo Deus de Harari. El “dataismo” está en cierto modo relacionado con la idea, quizá un poco exagerada, de que está surgiendo un cuarto paradigma científico basado en el uso intensivo de datos. Está idea se atribuye a Jim Gray, ganador del premio Turing. Gray afirma que “todo lo relacionado con la ciencia está cambiando debido al impacto de la tecnología de la información y el diluvio de datos” y que se está conformando un cuarto paradigma científico tras los tres primeros (empírico, teórico, computacional). Esta ideas se desarrollan en [The Fourth Paradigm: Data-intensive Scientific Discovery](https://books.google.es/books?id=oGs_AQAAIAAJ&redir_esc=y). Una traducción al castellano puede encontrarse [aquí](http://www.uam.mx/casadelibrosabiertos/libroselectronicos/4toparadigma/4toparadigma.pdf).

Sin embargo, hay que recordar, como se hace en [este post](https://simplystatistics.org/2016/06/03/defining-success/) de Jeff leek, que un resultado exitoso de un análisis de datos puede ser que los datos no permiten resolver la pregunta. Esta misma idea subyace en este tweet:

<blockquote class="twitter-tweet" align="center" data-width="400" data-lang="en" data-dnt="true" data-theme="light"><p lang="en" dir="ltr">This comment from Tukey (1986, <a href="https://t.co/El7wxTsemV">https://t.co/El7wxTsemV</a>) should be read out in the first 10 minutes of every statistics class, and at 20-minute intervals thereafter. <a href="https://t.co/gfpUPBqV28">pic.twitter.com/gfpUPBqV28</a></p>&mdash; Nïck Brown🌻 (@sTeamTraen) <a href="https://twitter.com/sTeamTraen/status/1361067408660783115?ref_src=twsrc%5Etfw">February 14, 2021</a></blockquote>

<br>

#### ¿Afectará todo esto a la Economía/Econometría?

Todos vosotros sabéis que la Economía es una de las ciencias sociales en la que más se utiliza la Estadística; de hecho la Econometría es precisamente eso, una rama de la Economía que utiliza métodos estadísticos en el estudio de los fenómenos económicos.

La respuesta a la pregunta anterior es que sí, no sé cuando ni como, pero es evidente que la disponibilidad de nuevos datos, y el auge de los métodos estadísticos asociados al ML/DL, tendrán que ir incorporándose poco a poco a nuestra ciencia. Abajo algunas referencias sobre ello:

- [The Economics of Artificial Intelligence: An Agenda](https://www.nber.org/books/agra-1)

- [IA y Economía](https://www.funcas.es/articulos/aplicacion-del-aprendizaje-automatico-al-analisis-economico-y-la-formulacion-de-politicas/)

- [IA y mercados financieros](https://www.funcas.es/articulos/aplicaciones-de-la-inteligencia-artificial-a-los-mercados-financieros-la-gestion-de-la-informacion-en-banca-de-las-finanzas-del-comportamiento-a-la-inteligencia-artificial-2019-n-162/)

- [Big Data in economics](https://wol.iza.org/articles/big-data-in-economics/long)

- [Machine Learning: An Applied Econometric Approach](https://www.aeaweb.org/articles?id=10.1257/jep.31.2.87)

- [The Impact of Machine Learning on Economics](https://www.nber.org/chapters/c14009.pdf)

- [Big Data: New Tricks for Econometrics](https://www.aeaweb.org/articles?id=10.1257/jep.28.2.3)

------------------------------------------------------------------------

<br>

## 5. Investigación reproducible y software libre

Cada vez más se oye hablar de la Investigación Reproducible (IR) o Reproducible Research (RR) en inglés. Creo y espero que en poco tiempo se convierta en el estándar.

Según la Wikipedia española,

> La reproducibilidad es la capacidad de una prueba o experimento de ser reproducido o replicado por otros, en particular, por la comunidad científica. La reproducibilidad es uno de los pilares del método científico, siendo la falsabilidad el otro. …

> … en muchas disciplinas, sobre todo en aquellas que implican el uso de estadística y procesos computacionales, se entiende que un estudio es reproducible si es posible recrear exactamente todos los resultados a partir de los datos originales y el **código informático** empleado para los análisis.

En este [libro](https://www.practicereproducibleresearch.org/) señalan que la reproducibildad está ligada íntimamente al método científico como ilustra el hecho de que el lema de la [Royal Society](https://es.wikipedia.org/wiki/Royal_Society) una de las sociedades científicas más antiguas del mundo es *“Nullius in verba”* que quiere decir más o menos “no creas en la palabra de nadie”. En el contexto científico quiere decir que las afirmaciones o descubrimientos científicos deben ser probados mediante el método científico.

A menudo se habla de la existencia de una [crisis de reproducibilidad](https://es.wikipedia.org/wiki/Crisis_de_replicaci%C3%B3n) refiriéndose con ello a la idea de que los resultados de muchos de los experimentos científicos son difíciles o imposibles a replicar en investigaciones posteriores. Uno de los casos más sonados, asociados a esta idea, es el de [Reinhart y Rogoff](https://www.weforum.org/agenda/2013/04/the-reinhart-and-rogoff-debacle/).

La idea de que puede existir una crisis de reproducibilidad, junto al hecho de que las nuevas tecnologías hacen cada vez más sencillo que los artículos e investigaciones científicas sean reproducibles, ha provocado cambios importantes en la política de asociaciones y revistas científicas, como la de la [American Economic Association](https://www.aeaweb.org/journals/policies/data-code/) según la cual, sólo se publicarán artículos en los que:

> “the data and code used in the analysis are clearly and precisely documented, and access to the data and code is clearly and precisely documented and is non-exclusive to the authors”.

[Aquí](https://www.gleech.org/psych) puedes encontrar un listado de resultados de papers científicos en Psicología que han tenido que ser revisitados tras estudios posteriores.

<br>

Para que un análisis con datos sea reproducible, no sólo es necesario que los datos utilizados han de ser accesibles, sino que cómo mínimo debería:

- proporcionar los datos originales (obviamente documentar las fuentes)

- efectuar todo el proceso a través de código (scripts)

- documentar el proceso de trabajo (por ejemplo el orden en que se ejecutaron los scripts)

<br>

Como veis, uno de los requisitos para hacer investigación reproducible es efectuar todo el proceso mediante scripts; es decir, hay que saber programar. Mira lo que dice Frank Harrell:

> Can one be a good data analyst without being a half-good programmer? The short answer to that is, ‘No.’ The long answer to that is, ‘No.’ —Frank Harrell https://homerhanumat.github.io/r-notes/frames.html

<br>

Hacer una investigación completamente reproducible es COSTOSO; de hecho, hay cursos completos sobre el tema, por ejemplo [este](http://kbroman.org/Tools4RR/), y muchos proyectos que tratan de promoverla; por ejemplo [este](https://ropensci.org/) que pretende favorecer el uso de datos abiertos a través de R. Afortunadamente, cada vez hay más herramientas que facilitan hacer IR: Make, Git, Docker, Pandoc, Knitr, markdown …

Hacer una investigación (completamente) reproducible no siempre es posible; OK, PERO al menos acercarse … un poco. Nosotros, en el curso, haremos análisis con datos e intentaremos que estos sean reproducibles. En el entorno **R** cada vez es más fácil acercarse al ideal de la IR. Para ello en el curso haremos siempre nuestros análisis con scripts de R. Concretamente utilizaremos **RStudio** para hacer análisis de datos, gestionando nuestros análisis a través de **Rprojects** y generaremos los informes y resultados del análisis con documentos **Rmarkdown**[^9]. Estos documentos Rmarkdown o **`.Rmd`** son reproducibles. En breve veremos que significa esto y sus utilidades tanto para la investigación como para la docencia. En [estas transparencias](https://mrslaviniag.github.io/xaringan_presentations/rladies_presentation_22_May_2019.html) nos cuentan como R y su ecosistema facilitan el hacer investigación o análisis reproducibles.

La razón para hacer los análisis reproducibles no sólo es cumplir con los estándares científicos, que también, sino también hay un interés personal para el analista. Para entenderlo puedes ver el siguiente [video de 1’44’’](https://www.youtube.com/watch?v=s3JldKoA0zw&feature=youtu.be) que muestra una de las principales ventajas de la IR, y sino ya lo experimentareis cuando hagamos hecho el primer análisis y os diga que me he equivocado con los datos, que os había dado la versión antigua de los datos. Os vais a reír si no habéis hecho vuestro análisis reproducible.

En palabras de `@TiffanyTimbers`:

> Nothing like doing something manually 60+ times and making mistakes to reinforce the idea “automate all the things”.

<br>

### Software libre

El software libre es de vital importancia en el desarrollo de la investigación reproducible. Piensa que por mucho que un investigador haga accesibles sus datos y su código, si utiliza un software privativo, en realidad su análisis no es reproducible, sólo lo será para aquellos que puedan pagar la licencia[^10].

De hecho, actualmente, al menos en el campo de la ciencia de datos, el software libre, o es ya mayoritario, o va camino de serlo. Es verdad que muchas empresas aún basan sus análisis de datos en programas como Excel, SPSS, Stata o SAS, pero la tendencia está cambiando y es de esperar que se acelere en un futuro próximo. Como ejemplo de esta idea puedes ver está publicación: [Big Data y open source](https://hipertextual.com/presentado-por/bbva/big-data-y-open-source).

Para aquellos que creen que el software comercial da más garantías, pueden leerse [este post](https://notstatschat.rbind.io/2019/02/18/absolutely-no-warranty/).

Seguramente entre las empresas pequeñas y medianas Excel continúa siendo el software de referencia para sus análisis cuantitativos. Sí, Excel es un fantástico software, lo sé, pero no sirve para todo. Un ejemplo de esto [aquí](https://www.sciencemag.org/news/2016/08/one-five-genetics-papers-contains-errors-thanks-microsoft-excel), o [aquí](https://www.johndcook.com/blog/2019/09/07/excel-r-bom/). [Este post](https://appsilon.com/excel-is-obsolete-here-are-the-top-2-alternatives-from-r-and-python/?utm_campaign=News&utm_medium=Community&utm_source=DataCamp.com) explica porque **Excel está obsoleto**. En los comentarios al post le atizan un poco. Un [hilo de Twitter](https://twitter.com/alexandreafonso/status/1313187531782082562) con errores graves provocados por el mal uso[^11]. En un tono más positivo, [este post](https://outsiderdata.netlify.com/post/why-i-migrated-from-excel-to-r/) explica porque abandonar Excel y migrar a R.

En palabras de Hadley en [esta entrevista](https://www.r-bloggers.com/advice-to-young-and-old-programmers-a-conversation-with-hadley-wickham/amp/)

> I think the tradeoff between Stata and R is: do you want a point-and-click interface, or do you want a programming interface? Point-and-click interfaces are great, because they lay out all of your options in front of you, and you don’t have to remember anything. You can navigate through the set of pre-supplied options. And that’s also it’s greatest weakness, because first of all, you are constrained into what the developer thought you should be able to do. And secondly, because your primary interaction is with a mouse, it’s very difficult to record what you did. And I think that’s a problem for science, because ideally you want to say how you actually got these results. And then simply do that reliably and have other people critique you on that. But it’s also really hard when you are learning, because when you have a problem, how do you communicate that problem to someone else? You basically have to say, “I clicked here, then I clicked here, then I clicked here, and I did this.” Or you make a screen cast, and it’s just clunky)

Este tweet incide también en alguno de los problemas de Excel. Tienes que ver la respuesta un poquito irónica de Dale Maschette, muy buena!! Para ello pincha en el tweet:

<blockquote class="twitter-tweet" align="center" data-width="400" data-lang="en" data-dnt="true" data-theme="light"><p lang="es" dir="ltr">Si vas a pasar el tiempo tratando de humillarme, haciendo que la clase sea innecesariamente dura, entonces mejor me voy, pero si de verdad quieres hacer el esfuerzo de ser un buen maestro entonces yo también estoy dispuesto a intentarlo.</p>&mdash; Edison Achalma (@achalmaedison) <a href="https://twitter.com/achalmaedison/status/1597228787431002113?ref_src=twsrc%5Etfw">November 28, 2022</a></blockquote>

<br>

Aquí tenemos un problema concreto que ha generado Excel al ser usado en al análisis de datos: han tenido que renombrar los genes para evitar que Excel interprete sus nombres como fechas.

<blockquote class="twitter-tweet" align="center" data-width="400" data-lang="en" data-dnt="true" data-theme="light"><p lang="es" dir="ltr">Si vas a pasar el tiempo tratando de humillarme, haciendo que la clase sea innecesariamente dura, entonces mejor me voy, pero si de verdad quieres hacer el esfuerzo de ser un buen maestro entonces yo también estoy dispuesto a intentarlo.</p>&mdash; Edison Achalma (@achalmaedison) <a href="https://twitter.com/achalmaedison/status/1597228787431002113?ref_src=twsrc%5Etfw">November 28, 2022</a></blockquote>

<br>

En este [post](https://www.brodrigues.co/blog/2020-11-21-guis_mistake/), Bruno Rodrigues argumenta porqué no se puede usar Excel para hacer Ciencia de Datos. Por supuesto que actualmente hay muchas **alternativas para hacer análisis de datos o visualizaciones** sin usar un lenguaje de programación, por ejemplo [aquí](https://appsilon.com/top-3-bi-tools/) o [aquí](https://www.storytellingwithdata.com/blog/2019/1/24/new-year-new-tools). Yo no digo nada, pero …

<br>

Please, **don’t look** [this other one](http://crashworks.org/if_programming_languages_were_vehicles/) `remo::ji("smile")` !!!

<br>

------------------------------------------------------------------------

## 6. ¿Por qué R?

En el curso usaremos R y RStudio. En la actualidad, en el campo de la ciencia de datos, hay sólo 2 alternativas, Phyton o R. De hecho hay un intenso debate sobre cual es más adecuado. Hay muchas opiniones al respecto, pero yo he seleccionado [esta](https://mchow.com/posts/data-science-cbk/) y [esta](https://blog.shotwell.ca/posts/why_i_use_r/), aunque la verdad, tampoco es necesario elegir un sólo lenguaje, [R y Phyton pueden colaborar](https://blog.rstudio.com/2019/12/17/r-vs-python-what-s-the-best-for-language-for-data-science/).

Evidentemente mi opinión es que para ciencia de datos R está varios pasos por delante de Phyton; si bien es verdad, que para hacer ML, y principalmente DL, Phyton puede ser más adecuado. En palabras de Hadley en [esta entrevista](https://www.r-bloggers.com/advice-to-young-and-old-programmers-a-conversation-with-hadley-wickham/amp/)

> For R and Python, Python is first and foremost a programming language. And that has a lot of good features, but it tends to mean, that if you are going to do data science in Python, you have to first learn how to program in Python. Whereas I think you are going to get up and running faster with R, than with Python because there’s just a bunch more stuff built in and you don’t have to learn as many programming concepts. You can focus on being a great political scientist or whatever you do and learning enough R that you don’t have to become an expert programmer as well to get stuff done.

Este tweet[^12] ejemplifica un poco la rivalidad (con buen rollo) entre R y Phyton:

<blockquote class="twitter-tweet" align="center" data-width="400" data-lang="en" data-dnt="true" data-theme="light"><p lang="en" dir="ltr">R or Python for statistics? It&#39;s basically the same. <br><br>Example: fit a linear model<br><br>R:<br>m1 &lt;- lm(y ~ x1 + x2)<br><br>Python:<br>import numpy as np<br>import statsmodels.api as sm<br>m1 = sm.OLS(y, sm.add_constant(np.array([x1, x2]).T))</p>&mdash; Richard Dinga 🧠📈👶👦👨👴 (@dinga92) <a href="https://twitter.com/dinga92/status/1273685480958242823?ref_src=twsrc%5Etfw">June 18, 2020</a></blockquote>

Aunque después de lo que dijo Elmo, yo creo que el debate está zanjado:

<blockquote class="twitter-tweet" align="center" data-width="300" data-lang="en" data-dnt="true" data-theme="dark"><p lang="en" dir="ltr">Finally an end to the <a href="https://twitter.com/hashtag/rstats?src=hash&amp;ref_src=twsrc%5Etfw">#rstats</a> vs. 🐍 debate! <a href="https://t.co/IDjmE0XIRG">pic.twitter.com/IDjmE0XIRG</a></p>&mdash; Mine Çetinkaya-Rundel (@minebocek) <a href="https://twitter.com/minebocek/status/1174382623499661312?ref_src=twsrc%5Etfw">September 18, 2019</a></blockquote>

R se está convirtiendo en el software estadístico de referencia en la mayoría de los centros de investigación y universidades, y su uso se está extendiendo también dentro de la empresa privada. R es software libre, gratuito y está incorporando más rápidamente que otros programas las técnicas avanzadas de análisis de datos que se están desarrollando en los últimos años. Otro aspecto importante que convierte a R en una herramienta muy potente es que incorpora un lenguaje de programación sencillo y muy flexible, que permite tener un control total sobre el análisis que se está desarrollando

Creo que en la actualidad R es el mejor programa para iniciarse y hacer análisis de datos. Si no me acabas de creer, o quieres leer algo sobre la importancia y capacidades de R puedes hacerlo [aquí](http://nadaesgratis.es/fernandez-villaverde/r) o [aquí](https://www.r-bloggers.com/why-r-is-the-best-data-science-language-to-learn-today/), o [aquí](https://shirinsplayground.netlify.com/2017/09/ode_to_r/) o más recientemente [aquí](https://www.eoda.de/en/wissen/blog/r-python-julia-data-science-2019).

<br>

R es cada vez más usado, no sólo en la universidad y la docencia, sino también en el mundo de la empresa, puedes verlo [aquí](https://www.r-bloggers.com/six-reasons-to-learn-r-for-business/) o [aquí](http://blog.sellorm.com/2016/11/26/talk-r-is-production-safe/). Una de las conferencias más importantes sobre el uso comercial de R es [The Enterprise Applications of the R Language Conference (EARL)](https://earlconf.com/#info).

Entre las empresas que usan R están: Google, Facebook, Twitter, Microsoft, IBM, Uber, Ford, Airbnb, American Express, Barclays Bank, [Bank of America](https://www.r-bloggers.com/bank-of-america-uses-r-for-reporting/) y muchas otras. [Aquí](https://github.com/ThinkR-open/companies-using-r) o [aquí](https://www.listendata.com/2016/12/companies-using-r.html) puedes encontrar un listado más completo.

Una de las mayores ventajas de usar R es que puedes usar Rmarkdown y Shiny. Lo veremos, pero [aquí](https://rfortherestofus.com/2019/03/r-killer-feature-rmarkdown/) tienes un post que explica sus ventajas. Un ejemplo de utilización es [está aplicación de seguiminento del covid](https://calcat.covid19.ca.gov/cacovidmodels/) que ha implementado el departamento of Public Health de California.

Si te gustan los rankings de lenguajes de programación, [aquí](https://redmonk.com/sogrady/2020/02/28/language-rankings-1-20/) tienes uno, de enero de 2020, en el Phyton está en segundo lugar mientras que R está en el puesto 13. Esto es lo que que se dice de R:

> In our first run of these rankings, R placed 17th. All these years later it jumps two spots from the last quarter’s edition up to \#13. In the interim, it has ranked as high as 12th but mostly commonly is found in the 13-15 range. Given the language’s specialized focus, this is likely its effective ceiling, but it’s also an illustration of the remarkable popularity of a language whose usage is restricted for all intents and purposes to a single domain – those who work with and operate on data. R’s success is an example of the power of an academia-supported community to elevate a language beyond its expected threshold, and it is notable that the aforementioned growth of Python and its expansion into data analytics has not observably come at the expense of traction in R.

Mientras reescribo estas notas, julio de 2020, R ha subido al puesto 8, mientras que Phyton está en el tercero. El ranking más actual puedes verlo [aquí](https://www.tiobe.com/tiobe-index/).

### ¿Es complicado aprender R?

¿Aprender R es complicado? No, bueno … ya responderé a esto en clase. No mires el siguiente tweet:

<blockquote class="twitter-tweet" align="center" data-width="400" data-lang="en" data-dnt="true" data-theme="light"><p lang="en" dir="ltr">Learning curve of R versus other tools (h/t <a href="https://twitter.com/timothycbates?ref_src=twsrc%5Etfw">@timothycbates</a>) <a href="https://twitter.com/hashtag/rstats?src=hash&amp;ref_src=twsrc%5Etfw">#rstats</a> <a href="https://t.co/UItBGTZ1s4">pic.twitter.com/UItBGTZ1s4</a></p>&mdash; rogier kievit (@rogierK) <a href="https://twitter.com/rogierK/status/730863729420701697?ref_src=twsrc%5Etfw">May 12, 2016</a></blockquote>

<br>

Aunque la verdad, esta dificultad/rareza de R es cosa de otros tiempos. Con el tidyverse todo es más fácil y brillante. Como muestra el tweet de Chris Albon, un miembro destacado de la comunidad Phyton. Merece la pena echarle un ojo a algunas de las respuestas al tweet.

<blockquote class="twitter-tweet">
<p lang="en" dir="ltr">
I used R for many years but whenever I hear about it now it feels like I watched R season one and now it is on a spin-off based on the characters of season 13.
</p>
— Chris Albon (@chrisalbon) <a href="https://twitter.com/chrisalbon/status/1225592440230481920?ref_src=twsrc%5Etfw">February 7, 2020</a>
</blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<br>

### Algunos sitios a visitar

- [Rweekly](https://rweekly.org/). Cada semana envían un archivo con los mejores análisis hechos con R esa semana. Tienes que apuntarte [aquí](https://feedburner.google.com/fb/a/mailverify?uri=rweekly&loc=en_US)

- [Rbloggers](https://www.r-bloggers.com/). Un agregador de blogs relacionados con R.

- [R Views](https://rviews.rstudio.com/). Es un blog asociado a RStudio. Cada mes saca un post donde eligen los mejores 40 paquetes de ese mes; por ejemplo, [aquí](https://rviews.rstudio.com/2019/08/29/july-2019-top-40-r-packages/) tienes el de julio de 2019.

- [swirl](https://swirlstats.com/). swirl teaches you R programming and data science interactively, at your own pace, and right in the R console!

<br>

<br>

[^1]: Realmente [Deep Blue](https://es.wikipedia.org/wiki/Deep_Blue_(computadora)), el ordenador que gano a Kasparov, no hacia uso de datos sino que usaba el calculo de probabilidades

[^2]: En realidad con aprender a programar un poco, todo lo que podamos, con R para poder ser más eficientes trabajando con datos ya tenemos bastante tarea en el curso

[^3]: Los dos últimos términos en castellano serían: Aprendizaje Máquina y Aprendizaje Profundo

[^4]: La palabra learning o aprendizaje induce a error porque no significa que se enseñe a los ordenadores a pensar como un ser humano, sino que básicamente consiste en aplicar algoritmos a datos masivos para inferir probabilidades.

[^5]: en ML/DL cuando hablan de atributos se refieren, más o menos, al termino regresores en Econometría

[^6]: Aunque el término Ciencia de datos se remonta, según la Wikipedia al menos a principios de los 70

[^7]: Una versión más amplia y fundamentada de estas ideas puede encontrarse [aquí](https://mdsr-book.github.io/mdsr2e/ch-prologue.html)

[^8]: Tal como argumenta [este post](https://www.brodrigues.co/blog/2020-11-05-retire_data_science/), la aparente dicotomía entre estadística y ciencia de datos se reducirá con el tiempo.

[^9]: En seguida explicaremos que son todas estas palabras que empiezan por r: R, RStudio, Rproject y Rmarkdown

[^10]: El software libre o código abierto también es una garantia de transparencia, libertades y derechos, como puede verse en el siguiente [hilo de Twitter](https://twitter.com/dcabo/status/1304418827279773697)

[^11]: Aunque seguramente, estos errores por mal uso de Excel se vieron favorecidos, cuando no provocados, por el mal diseño de Excel como herramienta para manejar datos

[^12]: Algunas de las respuestas al tweet son muy buenas
