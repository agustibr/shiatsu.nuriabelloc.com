---
title: Sessions de Shiatsu
description: "shiatsu, massatges a gracia"
menu: true
permalink: sessions/
sibling: sessions
shiatsuCarousel: ['sessio-shiatsu-nuriabelloc-01.jpg','sessio-shiatsu-nuriabelloc-02.jpg','sessio-shiatsu-nuriabelloc-03.jpg','sessio-shiatsu-nuriabelloc-04.jpg','sessio-shiatsu-nuriabelloc-05.jpg','sessio-shiatsu-nuriabelloc-06.jpg','sessio-shiatsu-nuriabelloc-07.jpg','sessio-shiatsu-nuriabelloc-08.jpg','sessio-shiatsu-nuriabelloc-09.jpg','sessio-shiatsu-nuriabelloc-10.jpg']
espaiCarousel: ['espai-nuriabelloc-01.jpg','espai-nuriabelloc-02.jpg','espai-nuriabelloc-03.jpg','espai-nuriabelloc-04.jpg','espai-nuriabelloc-05.jpg','espai-nuriabelloc-06.jpg','espai-nuriabelloc-07.jpg']
---

<section class="row banner">
  <div id="" class="marquee">
    {% for img in page.shiatsuCarousel %}
      <img src="{{site.baseurl | prepend: site.url}}/image/{{img}}" alt="{{page.title}}, {{site.description_short}}" />
    {% endfor %}
  </div>
</section>

El Shiatsu és una teràpia manual que es fonamenta en l'antiga filosofia i medicina tradicional xinesa i japonesa. Es basa en l'aplicació de pressió sobre els meridians i punts, així com també, mitjançant estiraments i mobilitzacions.

> Fomenta la circulació del Ki i estimula diversos sistemes de l'organisme, promovent la vitalitat i potenciant la capacitat d'autocuració.

Combino l'essència del shiatsu amb el treball corporal, l’estudi del moviment del cos, coneixements d’anatomia i fisiologia d’occident. Amb aquesta base, genero eines per a treballar el símptoma, la causa i la dinàmica creada.

Son sessions personalitzades i úniques, en les que treballarem conjuntament, l’aprenentatge i el feedback són elements imprescindibles. La comprensió sensitiva del motiu del treball corporal ajuda a que el sistema nerviós reorganitzi inclús els hàbits més arrelats. El shiatsu proporciona un ventall d’eines corporals que permeten un ritme respectuós i a la mesura de cadascú.

> _la durada de les sessions és entre 50 i 60 minuts cal portar roba còmode_

<div>
  <h2>l'Espai</h2>
  <section class="row banner">
    <div id="" class="marquee">
      {% for img in page.espaiCarousel %}
        <img src="{{site.baseurl | prepend: site.url}}/image/{{img}}" alt="{{page.title}}, {{site.description_short}}" />
      {% endfor %}
    </div>
  </section>
</div>
