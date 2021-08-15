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

{%- for post in site.hdoc -%}
  {%- capture current_year -%}{{ post.date | date: "%Y" }}{%- endcapture -%}
  {%- unless current_year == previous_year -%}
    <h2>{{ current_year }}</h2>
    {%- assign previous_year = current_year -%}
  {%- endunless -%}
  <article class="post-item">
    <h3 class="post-item-title">
      <a href="{{ post.url }}">{{ post.title | escape }}</a>
    </h3> 
  </article>
{%- endfor -%}
