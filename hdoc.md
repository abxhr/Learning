---
title: 100 Days of Code
permalink: /hdoc/
layout: page
excerpt: 100DaysOfCode.
comments: false
---

<p align="center">
Join me on my journey to <a href="https://www.100daysofcode.com/"><b>100 Days Of Code</b></a>!
<br>
I'll be documenting each day of the challenge through my blogs here.
</p>

{% include countdown_hdoc.html %}

{%- for post in site.categories.hdoc -%}
  <article class="post-item">
    <h3 class="post-item-title">
      <a href="{{ post.url }}">{{ post.title | escape }}</a>
    </h3> 
  </article>
{%- endfor -%}
