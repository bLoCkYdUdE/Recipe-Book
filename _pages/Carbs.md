---
layout: default
title: Carbs
permalink: /carbs/
---


<h1>Carbs</h1>

<ul>
  {% assign carbs_recipes = site.recipes | where: "categories", "carb" %}
  {% for recipe in carbs_recipes %}
    <li><a href="{{ site.baseurl }}{{ recipe.url }}">{{ recipe.title }}</a></li>
  {% endfor %}
</ul>