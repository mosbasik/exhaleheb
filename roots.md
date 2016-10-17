---
layout: page
title: Roots
permalink: /roots/
gallery:
  - href: "/img/roots/PN20081230 122.jpg"
    title:
  - href: "/img/roots/PN20090201 026.jpg"
    title:
  - href: "/img/roots/PN20090201 034.jpg"
    title:
  - href: "/img/roots/PN20090201 062.jpg"
    title:
  - href: "/img/roots/PN20070401 003.jpg"
    title:
  - href: "/img/roots/PN20090830 097.jpg"
    title:
  - href: "/img/roots/PN20090201 068.jpg"
    title:
  - href: "/img/roots/PN20090830 103.jpg"
    title:
  - href: "/img/roots/PN20100610 072.jpg"
    title:
  - href: "/img/roots/PN20090201 063.jpg"
    title:
  - href: "/img/roots/PN20091222 027.jpg"
    title:
  - href: "/img/roots/PN20081230 037.jpg"
    title:
  - href: "/img/roots/PN20090201 065.jpg"
    title:
  - href: "/img/roots/PN20070401 077.jpg"
    title:
  - href: "/img/roots/PN20100929 014.jpg"
    title:
---

Here are some pics of various home groups overseen by Henrys in the Congo - our living CV, if you like:

<ul class="photo-gallery">
  {% for image in page.gallery %}
    <li>
      <a href="{{ image.href }}">
        <img src="{{ image.href }}" alt="{{ image.title }}" title="{{ image.title }}">
      </a>
    </li>
  {% endfor %}
</ul>