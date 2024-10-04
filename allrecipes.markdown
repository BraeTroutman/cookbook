---
layout: page
title: All Recipes
permalink: /recipes/
---

{% for recipe in site.recipes %}
## [{{ recipe.title }}]({{ recipe.url | prepend: site.baseurl }})
{% endfor %}
