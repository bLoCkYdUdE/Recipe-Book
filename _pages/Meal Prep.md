---
layout: default
title: Meal Prep
permalink: /meal-prep/
---


<h1>Meal Prep</h1>

<ul>
  {% assign meal-prep_recipes = site.recipes | where: "categories", "Meal Prep" %}
  {% for recipe in meal-prep_recipes %}
    <li><a href="{{ recipe.url }}">{{ recipe.title }}</a></li>
  {% endfor %}
</ul>