---
title: Sessions
description: "shiatsu, massatges a gracia"
menu: true
permalink: sessions/
sibling: sessions
---

{% assign sessions = site.pages | where:"lang", page.lang | where:"parent", 'sessions' | sort: 'id' %}
{% assign preus-link = site.pages | where:"sibling", "preus" | where:"lang", page.lang %}
{% assign espai-link = site.pages | where:"sibling", "espai" | where:"lang", page.lang %}

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
  <div class="col-md-12">

    <a class="btn btn-primary btn-block" href="{{ preus-link[0].url | prepend: site.baseurl | prepend: site.url }}">
      {{ preus-link[0].title }}
    </a>

    <a class="btn btn-primary btn-block" href="{{ espai-link[0].url | prepend: site.baseurl | prepend: site.url }}">
     {{ espai-link[0].title }}
    </a>

  </div>
</div>
