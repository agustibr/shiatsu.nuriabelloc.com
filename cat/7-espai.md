---
title: Espai
description: "espai on gaudiras"
menu: false
permalink: espai/
sibling: espai
---

<img class="img-responsive" src="{{site.baseurl | prepend: site.url}}/image/espai-nuriabelloc-01.jpg" alt="espai shiatsu" />
<img class="img-responsive" src="{{site.baseurl | prepend: site.url}}/image/espai-nuriabelloc-02.jpg" alt="espai shiatsu" />

---
{% assign sessions-link = site.pages | where:"sibling", "sessions" | where:"lang", page.lang %}

<p><a href="{{ sessions-link[0].url | prepend: site.baseurl | prepend: site.url }}">
{{ sessions-link[0].title }}
</a></p>

