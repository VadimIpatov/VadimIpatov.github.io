---
layout: page
title: 21 октября 2017
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

Седьмая встреча пройдёт в **субботу**, 21 октября 2017 в 15:00.
На мероприятие отведено приблизительно 3-4 часа.
Между докладами запланирован 10-15 минутный кофе-брейк, чтобы вы могли перекусить.
А после докладов состоится after-party, где можно будет пообщаться на свободные темы — не расходитесь :)

Чтобы мы могли оценить количество участников, пожалуйста, [зарегистрируйтесь][register].

<p><a class="fa fa-calendar" href="webcal://kosbackend.ru/register/kosbackend.ics"> Создать напоминание в календаре</a></p>

Где
---

Встреча пройдёт в конференц-зале компании ["Тензор"][tensor]{:target="_blank"} по адресу: г. Кострома, ул. Лесная, 11.
Маршрут от остановки общественного транспорта указан на карте.

Контакты: +7-920-640-2860 <a href="mailto:euphoria.vi@gmail.com">Вадим</a>, +7-920-645-3357 <a href="mailto:av.bargan@tensor.ru">Алексей</a>

<script type="text/javascript" charset="utf-8" async src="https://api-maps.yandex.ru/services/constructor/1.0/js/?um=constructor%3A12d523befd729e0398d3a802a45ea8371602efd80227538e22f701446abfed20&amp;width=708&amp;height=450&amp;lang=ru_RU&amp;scroll=true"></script>

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
[luxuria]: http://www.conferencelux.ru/location-map/index.aspx
[tensor]: https://tensor.ru
[speakers]: /speakers/
[vote-oleg]: /blog/generators-or-gpu/
[vote-pavel]: /blog/derby-or-loadspeed/
