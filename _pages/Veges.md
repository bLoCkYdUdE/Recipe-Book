---
layout: default
title: Veges
permalink: /veges/
---


<h1>Veges</h1>

<ul>
  {% assign veges_recipes = site.recipes | where: "categories", "veges" %}
  {% for recipe in veges_recipes %}
    <li><a href="{{ site.baseurl }}{{ recipe.url }}">{{ recipe.title }}</a></li>
  {% endfor %}
</ul>