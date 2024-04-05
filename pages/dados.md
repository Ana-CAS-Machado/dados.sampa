---
layout: page
title: Dados
subtitle: "Dados do município de São Paulo" 
permalink: /dados/
feature-img: "assets/img/pexels/pexels-photo.png"
tags: [Dados]
---

<!-- lista de cards -->
<div class="dados">

 <div class="toc-list">
   <div class="box-list">
    <ul class="toc">
      {% for post in site.posts %}
        <li class="li-toc">
          <a class="test" href="#{{ post.title | slugify }}">{{ post.tema }}</a>
        </li>
      {% endfor %}
    </ul>
   </div>
 </div>
 <!-- cards do post -->
 <div class="container">
   {% for post in site.posts %}
     <div class="box">
       <span></span>
       <div class="cont">
          <div class="linha"></div>
         <h2>{{ post.tema }}</h2>
         <p>{{ post.description }}</p>
         <a class="btn" href="{{ post.permalink }}">Leia Mais</a>
       </div>
     </div>
   {% endfor %}
 </div>
</div>