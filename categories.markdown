---
layout: page
title: Recipes by Category
permalink: /categories/
---

{% assign categories = site.recipes | map: "categories" | join: "," | split: "," | uniq %}
{% for cat in categories %}
## {{ cat | capitalize }}

{% for recipe in site.recipes %}
{% if recipe.categories contains cat %}
### [{{ recipe.title }}]({{ recipe.url | prepend: site.baseurl }})
{% endif %}
{% endfor %}

{% endfor %}
