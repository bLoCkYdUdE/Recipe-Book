---
layout: default
title: All Recipes
permalink: /all-recipes/
---


<h1>All Recipes</h1>

<ul>
  {% for recipe in site.recipes %}
    <li><a href="{{ recipe.url }}">{{ recipe.title }}</a></li>
  {% endfor %}
</ul>