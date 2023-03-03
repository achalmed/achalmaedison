---
title: Blog
description: "This is a fully featured blog that supports categories, \ntags, series,and pagination.\n"
author: Edison Achalma
show_post_thumbnail: true
thumbnail_left: false
show_author_byline: true
show_post_date: true
show_button_links: false
# for listing page layout
layout: list-sidebar # list, list-sidebar, list-grid

# for list-sidebar layout
sidebar:
  title: Blog
  description: " ¡Bienvenidos a mi sección de blog en mi página web personal! Aquí encontrarás una variedad de temas y reflexiones que he querido compartir con ustedes, desde mis pensamientos sobre la vida y el mundo que nos rodea, hasta mi experiencia en diferentes áreas de mi vida profesional y personal. Espero que disfrutes leyendo mis publicaciones tanto como yo disfruto escribirlas. ¡Gracias por visitar mi sitio web y por ser parte de esta comunidad! Este blog es mi [digital garden](https://nesslabs.com/digital-garden-set-up), entre un bloc de notas y un blog."
  author: Edison Achalma
  text_link_label: Subscribe via RSS
  text_link_url: /index.xml
  show_sidebar_adunit: true

# set up common front matter for all pages inside blog/  
cascade:
  author: Edison Achalma
  show_author_byline: true
  show_comments: true # see site config to choose Disqus or Utterances
  show_post_date: true
  # for single-sidebar layout
  sidebar:
    show_sidebar_adunit: false # show ad container
    text_link_label: View recent posts
    text_link_url: /blog/


---

** No content below YAML for the blog _index. This file provides front matter for the listing page layout and sidebar content. It is also a branch bundle, and all settings under `cascade` provide front matter for all pages inside blog/. You may still override any of these by changing them in a page's front matter.**
