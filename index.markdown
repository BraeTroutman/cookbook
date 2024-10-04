---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

## Recipes

{% for recipe in site.recipes %}
### [{{ recipe.title }}]({{ recipe.url | prepend: site.baseurl }})
{% endfor %}

## Notes

If any recipes are missing here that you'd like added, or you think one of the recipes is wrong, please let me know by [opening a new issue](https://github.com/BraeTroutman/cookbook/issues/new)
on my github, and I'll acknowledge/make a fix as soon as I can!

