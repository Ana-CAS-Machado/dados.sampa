---
layout: page
title: Dados
permalink: /Dados/
feature-img: "assets/img/pexels/pexels-photo.png"
tags: [Page]
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
       <div class="content">
         <h2>{{ post.tema }}</h2>
         <p>{{ post.description }}</p>
         <a href="{{ post.url }}">Read More</a>
       </div>
     </div>
   {% endfor %}
 </div>
</div>