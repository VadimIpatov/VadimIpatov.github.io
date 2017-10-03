---
layout: page
title: Люди
comments: true
---

<ul class="author-list">
{% for data in site.data.authors %}
  {% assign author = data[1] %}
  {% assign authorId = data[0] %}
  <li>
    <div class="bio-block">
      {% if author.avatar contains 'http' %}
      <img src="{{ author.avatar }}" class="bio-photo" alt="{{ author.name }} bio photo"></a>
      {% else %}
      <img src="{{ site.url }}/images/{{ author.avatar }}" class="bio-photo" alt="{{ author.name }} bio photo">
      {% endif %}
      {% if author.twitter %}
      <span class="social-share-twitter">
        <a target="_blank"  href="https://twitter.com/{{ author.twitter }}"><i class="fa fa-twitter-square"></i> {{ author.twitter }}</a>
      </span>
      {% endif %}
      {% if author.vk %}
      <span class="social-share-vk">
        <a target="_blank" href="https://vk.com/{{ author.vk }}"><i class="fa fa-vk"></i> {{ author.vk }}</a>
      </span>
      {% endif %}      
      {% if author.github %}
      <span>
        <a href="http://github.com/{{ author.github }}" title="{{ author.github }} on Github" target="_blank"><i class="fa fa-github-square"></i> {{ author.github }}</a>
      </span>
      {% endif %}
    </div>
    <h2 data-company="{{ author.company }}">{{ author.name }}</h2>
    <p>{{ author.bio }}</p>
    <ul class="post-list">
    {% for post in site.categories.talks %}
      {% if post.author contains authorId %}
      <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}.</a></li> 
      {% endif %}  
    {% endfor %}
    </ul>
  </li>
{% endfor %}
</ul>