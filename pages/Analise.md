---
layout: page
title: Analise
subtitle: "Analise sobre os dados do município de São Paulo" 
permalink: /analise/
feature-img: "assets/img/pexels/pexels-photo.png"
tags: [Page]
position: 3
---

<!-- lista de cards -->
<div class="dados">

 <div class="toc-list">
   <div class="box-list">
    <ul class="toc">
      {% for post in site.analise %}
        <li class="li-toc">
          <a class="test" href="#{{ post.title | slugify }}">{{ post.tema }}</a>
        </li>
      {% endfor %}
    </ul>
   </div>
 </div>
 <!-- cards do post -->
 <div class="contain">
   {% for post in site.analise %}
     <div class="box-analis">
        <span></span>
        <div class="contente">
          <div class="linha"></div>
          <h2>{{ post.tema }}</h2>
          <p>{{ post.description }}</p>
          <a class="btn" href="{{ post.permalink | relative_url }}">Leia Mais</a>
        </div>
      </div>
   {% endfor %}
  </div>
</div>