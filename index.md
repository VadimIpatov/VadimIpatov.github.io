---
layout: page
title: 26 марта 2016
excerpt: 
comments: true
---

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

Следующая встреча (четвёртая по счёту) пройдёт в **субботу**, 28 мая 2016 в 15:00.
На все доклады отведено приблизительно 3 часа.
Между докладами запланирован 10-15 минутный кофе-брейк, чтобы вы могли перекусить.
А после докладов состоится after-party, где можно будет пообщаться на свободные темы — не расходитесь :)

Чтобы мы могли оценить количество участников, пожалуйста, [зарегистрируйтесь][register].

<p><a class="fa fa-calendar" href="webcal://kosbackend.ru/register/kosbackend.ics"> Создать напоминание в календаре</a></p>

Где
---

Встречи проходят в конференц-зале отеля ["Golden Ring"][hotel-ring]{:target="_blank"} по адресу: г. Кострома, ул. Нижняя Дебря, д.104а.
До отеля можно добраться на маршрутке №4. Маршрут от остановки общественного транспорта указан на карте.

Контакты: +7 920 640-2860 <a href="mailto:euphoria.vi@gmail.com">Вадим</a>, +7 910 660-2044 <a href="mailto:n.druzhinin@it-kostroma.ru ">Николай</a>

<script type="text/javascript" charset="utf-8" src="//api-maps.yandex.ru/services/constructor/1.0/js/?sid=D_FAZaSMO4OggLeG6imnrClLom5cO5Ww&height=450"></script>

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
[speakers]: /speakers/
[vote-oleg]: /blog/generators-or-gpu/
[vote-pavel]: /blog/derby-or-loadspeed/
