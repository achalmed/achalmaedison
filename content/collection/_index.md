---
title: Cursos
subtitle: A collection, minus the blog.
description: "En la web encontrarás información acerca del desarrollo del curso, así como la mayoría de los materiales que se usarán en él.\n"
author: Edison Achalma
show_post_thumbnail: true
thumbnail_left: false
show_author_byline: true
show_post_date: true
# para el diseño de la página de listado
layout: list-sidebar # list, list-sidebar, list-grid

# para el diseño de la barra lateral de la lista
sidebar: 
  title: Bienvenido a los cursos
  description: "¡Aquí encontrarás una amplia variedad de cursos diseñados para ayudarte a mejorar tus habilidades y conocimientos en diferentes áreas. Nuestros cursos están cuidadosamente diseñados y son impartidos por expertos en cada materia. Desde programación hasta marketing digital, estamos seguros de que encontrarás un curso que se adapte a tus necesidades y objetivos. ¡Explora nuestra selección de cursos y comienza tu camino hacia el éxito hoy mismo!" 
  author: Edison Achalma
  text_link_label: Subscribe via RSS
  text_link_url: /index.xml
  show_sidebar_adunit: true # show ad container

# configurar un frente común para todas las páginas dentro del blog/
cascade:
  author: Edison Achalma
  show_author_byline: true
  show_post_date: true
  show_comments: false # solo activar en blog
  # para diseño de barra lateral única
  layout: single-series
  sidebar:
    author: Edison Achalma
    description: "En la web encontrarás información acerca del desarrollo del curso, así como la mayoría de los materiales que se usarán en él.\n"
    show_author_byline: true
    show_post_date: true
    show_sidebar_adunit: false # mostrar contenedor de anuncios
    text_contents_label: En esta página
    text_link_label: ""
    text_link_url: /blog/
    text_series_label: En esta serie
    title: Create a Collection
---

** No content below YAML for the blog _index. This file provides front matter for the listing page layout and sidebar content. It is also a branch bundle, and all settings under `cascade` provide front matter for all pages inside blog/. You may still override any of these by changing them in a page's front matter.**