---
title: Sessions
description: "shiatsu, massatges a gracia"
menu: true
permalink: sessions/
sibling: sessions
espaiCarousel: ['espai-nuriabelloc-01.jpg','espai-nuriabelloc-02.jpg']
---

{% assign sessions = site.pages | where:"lang", page.lang | where:"parent", 'sessions' | sort: 'id' %}
{% assign preus-link = site.pages | where:"sibling", "preus" | where:"lang", page.lang %}

<div class="row">
  {% for session in sessions %}
    <div class="col-sm-6 col-md-4">
      <a class="thumbnail" href="{{ session.url | prepend: site.baseurl | prepend: site.url }}">
        <img src="{{site.baseurl | prepend: site.url}}/image/{{session.cover}}" alt="{{ session.title }}">
        <div class="caption">
          <h3>{{ session.title }}</h3>
        </div>
      </a>
    </div>
  {% endfor %}
</div>
<div>
  <h2>l'Espai</h2>
  <div id="carousel-espai" class="carousel slide" data-ride="carousel">
    <!-- Indicators -->
    <ol class="carousel-indicators">
      {% for img in page.espaiCarousel %}
        <li data-target="#carousel-espai" data-slide-to="{{ forloop.index0 }}" {% if forloop.first%}class="active"{% endif%}></li>
      {% endfor %}
    </ol>

    <!-- Wrapper for slides -->
    <div class="carousel-inner" role="listbox">
      {% for img in page.espaiCarousel %}
        <div class="item {% if forloop.first %} active {% endif %}">
          <img src="{{site.baseurl | prepend: site.url}}/image/{{img}}" alt="page.title" />
        </div>
      {% endfor %}
    </div>
  </div> <!-- /.carousel -->
</div>
