---
title: e11ty
subtitle: ely + 11ty
layout: layouts/base.njk
---

## blog

<ul class="listing">
{%- for page in collections.post -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>

## links

<ul class="listing">
{%- for item in hawksworx.entries.slice(0,5) -%}
  <li>
    <a href="{{ item.link }}">{{ item.title }}</a>
  </li>
{%- endfor -%}
</ul>

[![Netlify Status](https://api.netlify.com/api/v1/badges/57d7936f-985c-4196-b61a-4dcde75b4666/deploy-status)](https://app.netlify.com/sites/eleventy-57-blue/deploys)





