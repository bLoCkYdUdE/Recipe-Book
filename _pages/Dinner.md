---
layout: default
title: Dinner
permalink: /dinner/
---


<h1>Dinner</h1>

<ul>
  {% assign Dinner_recipes = site.recipes | where: "categories", "dinner" %}
  {% for recipe in Dinner_recipes %}
    <li><a href="{{ site.baseurl }}{{ recipe.url }}">{{ recipe.title }}</a></li>
  {% endfor %}
</ul>