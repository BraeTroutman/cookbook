---
layout: page
title: Recipes by Region
permalink: /regions/
---

{% assign regions = site.recipes | map: "region" | join: "," | split: "," | uniq %}
{% for region in regions %}
## {{ region }}

{% for recipe in site.recipes %}
{% if recipe.region contains region %}
### [{{ recipe.title }}]({{ recipe.url | prepend: site.baseurl }})
{% endif %}
{% endfor %}

{% endfor %}
