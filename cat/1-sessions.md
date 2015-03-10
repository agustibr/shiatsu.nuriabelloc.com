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
    <div class="col-xs-6">
      <a class="btn" href="{{ session.url | prepend: site.baseurl | prepend: site.url }}">{{ session.title }}</a>
      <!-- <p>{{ session.cover }}</p> --><br>
    </div>
  {% endfor %}
  <div class="col-xs-6">
    <div class="row">
      <div class="col-xs-6">
        <a href="{{ preus-link[0].url | prepend: site.baseurl | prepend: site.url }}">
          {{ preus-link[0].title }}
        </a>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-6">
        <a href="{{ espai-link[0].url | prepend: site.baseurl | prepend: site.url }}">
         {{ espai-link[0].title }}
        </a>
      </div>
    </div>
  </div>
</div>
