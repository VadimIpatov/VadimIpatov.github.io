---
layout: page
title: Встречи
comments: true
---

<div>
{% for data in site.data.talks reversed %}
    {% assign meetupid = data[0] %}
    {% assign meetup = data[1] %}
    
    {% if meetup.finished %}
    
    {% capture talklist %}{% for post in site.posts %}{% if post.talk == meetupid %}{% if post.author %}{% assign author = site.data.authors[post.author] %}{% endif %}<li><a href="{{ site.url }}{{ post.url }}">{{ post.title }} [ {% if author %} {{ author.name }}{% if author.company %}, {{ author.company }}{% endif %}{% endif %} ]</a></li>{% endif %}{% endfor %}{% endcapture %}
    
    {% if talklist.size > 0 %}
    <h2>
    {{ meetup.date | date: "%-d" }}
    {% assign m = meetup.date | date: "%-m" %}
    {% case m %}
      {% when '1' %}января
      {% when '2' %}февраля
      {% when '3' %}марта
      {% when '4' %}апреля
      {% when '5' %}мая
      {% when '6' %}июня
      {% when '7' %}июля
      {% when '8' %}августа
      {% when '9' %}сентября
      {% when '10' %}октября
      {% when '11' %}ноября
      {% when '12' %}декабря
    {% endcase %}
    {{ meetup.date | date: "%Y" }}
    </h2>
    {% if meetup.info %}
    <p>{{ meetup.info }}</p>
    {% endif %}
    {{ meetup.foto }}
    <h3>Доклады</h3>
    <ul class="post-list">
        {{ talklist }}
    </ul>
    {% if meetup.photos %}
    <div class="fotorama" data-fit="scaledown" data-width="700" data-maxwidth="100%" data-ratio="3/2">
    {% assign photospath = 'images/reports/' | append: meetupid %}
    {% for image in site.static_files %}
        {% if image.path contains photospath %}<img src="{{image.path}}" />{% endif %}
    {% endfor %}
    </div>
    {% endif %}
    {% endif %}
    
    {% endif %}
{% endfor %}
</div>