---
layout: page
title: 21 ноября 2015
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
  <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }} {{ authorslist }}</a></li>
  {% endif %}
{% endfor %}
</ul>

Когда
-----

Нулевая встреча пройдет в **субботу**, 21 ноября 2015 в 21:00.

Чтобы мы могли оценить количество участников, пожалуйста, [зарегистрируйтесь][register].

Где
---

Встречи проходят в новом офисе компании [Тензор][tensor] по адресу: г. Ярославль, ул. Угличская, д. 36.
Центральный вход, угол здания на пересечении улиц Чехова и Угличской.
Маршрут от остановки общественного транспорта указан на карте.

Места для парковки автомобилей указаны на карте зеленым цветом. Припарковаться можно либо на пустыре за зданием, 
либо вдоль здания под "навесом". Пожалуйста, не паркуйтесь на тротуаре. 

Контактные телефоны: +7 920 640-2860 Вадим, +7 910 660-2044 Николай

<script type="text/javascript" charset="utf-8" src="//api-maps.yandex.ru/services/constructor/1.0/js/?sid=OaSCkjqQ9MoOIwGeLlFWJiM9GD6Ae8KK&height=450"></script>

<!--
<ul class="post-list">
{% for post in site.posts limit:10 %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></article></li>
{% endfor %}
</ul>
-->

[register]: /register/
[tensor]: http://tensor.ru/
[speakers]: /speakers/
[vote-oleg]: /blog/generators-or-gpu/
[vote-pavel]: /blog/derby-or-loadspeed/
