---
layout: page
title: Dados
permalink: /Dados/
feature-img: "assets/img/pexels/pexels-photo.png"
tags: [Page]
---

<div class="container">
<!-- cards do post -->
  {% for post in site.posts %}
    <div class="box">
      <span></span>
      <div class="content">
        <h2>{{ post.title }}</h2>
        <p>{{ post.description }}</p>
        <a href="{{ post.url }}">Read More</a>
      </div>
    </div>
  {% endfor %}

  <!-- lista de cards -->
 <div class="toc-list">
  <div class="box-list">
   <ul class="toc">
     {% for post in site.posts %}
       <li class="li-toc">
         <a class="test" href="#{{ post.title | slugify }}">{{ post.title }}</a>
       </li>
     {% endfor %}
   </ul>
  </div>
 </div>
</div>