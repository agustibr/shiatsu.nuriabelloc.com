---
title: Sessions
description: "shiatsu, massatges a gracia"
menu: true
permalink: sessions/
sibling: sessions
espaiCarousel: ['espai-nuriabelloc-01.jpg','espai-nuriabelloc-02.jpg','espai-nuriabelloc-03.jpg','espai-nuriabelloc-04.jpg','espai-nuriabelloc-05.jpg','espai-nuriabelloc-06.jpg','espai-nuriabelloc-07.jpg','espai-nuriabelloc-08.jpg','espai-nuriabelloc-09.jpg','espai-nuriabelloc-10.jpg','espai-nuriabelloc-11.jpg']
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
  <section class="banner row">
    <div id="marquee" class="row">
      {% for img in page.espaiCarousel %}
        <img src="{{site.baseurl | prepend: site.url}}/image/{{img}}" alt="page.title" />
      {% endfor %}
    </div>
  </section>
</div>
