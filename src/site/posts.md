---
title: 11t.ely posts
subtitle: a multipurpose 11ty site for ely to log ongoing projects and processes
layout: layouts/base.njk
---

## Posts

<ul class="listing">
{%- for page in collections.post -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>
