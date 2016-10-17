---
layout: page
title: Archive
permalink: /archive/
---

{% for post in site.posts %}
  {% assign currentdate = post.date | date: "%Y" %}
  {% if currentdate != date %}
    {% unless forloop.first %}
</ul>
    {% endunless %}
<h2 id="y{{post.date | date: "%Y"}}">{{ currentdate }}</h2>
<ul>
    {% assign date = currentdate %}
  {% endif %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% if forloop.last %}</ul>{% endif %}
{% endfor %}

- - -

{% for post in site.posts %}
  {% assign currentdate = post.date %}
  {% if currentdate != date %}
    {% unless forloop.first %}
</ul>
    {% endunless %}
<h2 id="y{{post.date | date: "%Y"}}">{{ currentdate  }} <br> {{date}}</h2>
<ul>
    {% assign date = currentdate %}
  {% endif %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% if forloop.last %}
</ul>
  {% endif %}
{% endfor %}
