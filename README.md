# Brae's Cookbook

A collection of recipes defined using [Cooklang](https://cooklang.org/) and automatically grouped and 
converted to a static site hosted on GitHub pages using Jekyll. 

## Defining new recipes

new recipes can be defined for the website by adding a `.cook` file to the `_recipes/` directory.

copy the [recipe template](templates/example.cook) to the `_recipes` directory with a name corresponding to your recipe,
and fill in yaml frontmatter with the proper details. Then you can write the recipe itself, following the [cooklang file format](https://cooklang.org/docs/spec/)

While the category and region fields of the frontmatter are not strictly necessary, they are really helpful for automatically
grouping recipes on the statically generated site.
