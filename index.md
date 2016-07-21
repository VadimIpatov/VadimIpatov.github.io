---
layout: page
title: 30 июля 2016 — АйТишники на каникулах
excerpt: 
comments: true
---

Лето, солнце, пляж… митап. Да-да-да, мы решили не расслабляться и не терять темпа.
Очередной митап будет по расписанию. Однако, в этот раз, сделав поправку на летнее настроение,
формат митапа немного изменится.


Доклады
-------

<ul class="post-list">
{% for post in site.categories.talks %}
  {% if post.author %}
    {% capture authorslist %}
      {% for a in post.author %}
        {% assign author = site.data.authors[a] %}
        {% if author %} {{ author.name }}{% if author.company %}, {{ author.company }}{% endif %}{% endif %}{% unless forloop.last %};{% endunless %}
      {% endfor %}
    {% endcapture %}
  {% endif %}
  {% if post.announce %}
  <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }} [ {{ authorslist }} ]</a></li>
  {% endif %}
{% endfor %}
</ul>

Когда
-----

Пятая встреча пройдёт в **субботу**, 30 июля 2016 в 15:00.
На мероприятие отведено приблизительно 2 часа.
А после докладов состоится after-party, где, по традиции, можно будет пообщаться на свободные темы — не расходитесь :)

Регистрация
-----------

Обратите внимание, что в этот раз количество мест ограничено 20-ю участниками. Пожалуйста, [зарегистрируйтесь][register].

<p><a class="fa fa-calendar" href="webcal://kosbackend.ru/register/kosbackend.ics"> Создать напоминание в календаре</a></p>

Где
---

Встреча пройдёт в студии ["FOTORAMA"][fotorama]{:target="_blank"} по адресу: г. Кострома, ул. Ерохова, д.3а, 2 этаж.<br>
Это большое здание из белого кирпича, рядом с ТЭЦ-1.
После того, как зайдете в ворота идите налево. Заходите в единственную дверь и поднимайтесь
на второй этаж. Далее направо, до конца по коридору, последняя дверь налево, соседний офис с Теле2.
Пожалуйста, не паркуйтесь близко к Ж/Д путям — они действующие. А поезд умеет очень громко гудеть :)

*Как добраться на общественном транспорте?*<br>
Остановка ТЭЦ-1.<br>
Автобусы и маршрутки: 2, 50, 57, 66.<br>
Троллейбус: 3 и 4.<br>

![Карта проезда](http://fotorama.su/images/map-site.jpg)

*Контакты:* +7 920 640-2860 <a href="mailto:euphoria.vi@gmail.com">Вадим</a>, +7 910 660-2044 <a href="mailto:n.druzhinin@it-kostroma.ru ">Николай</a>

<!--
<ul class="post-list">
{% for post in site.posts limit:10 %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></article></li>
{% endfor %}
</ul>
-->

[register]: /register/
[tensor]: http://tensor.ru/
[hotel-ring]: http://www.kostroma-goldenring.ru/contacts/
[fotorama]: http://fotorama.su/contacts
[speakers]: /speakers/
[vote-oleg]: /blog/generators-or-gpu/
[vote-pavel]: /blog/derby-or-loadspeed/
