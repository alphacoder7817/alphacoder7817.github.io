---
layout: page
title: Collections
---

# Collections

Collections in Jekyll are custom content types that allow you to group related content together. This is useful for organizing things like portfolios, case studies, or documentation.

## Creating a Collection

To create a collection, add a new directory to your Jekyll site and configure it in your `_config.yml` file. For example, to create a collection called `portfolio`, you would add the following to your `_config.yml`:

```yaml
collections:
  portfolio:
    output: true
```

Then, create a `_portfolio` directory in your Jekyll site to store your collection items.

## Using Collections

You can access and display collection items in your templates using Liquid syntax. For example, to display a list of portfolio items, you can use the following code:

```liquid
<ul>
  {% for item in site.portfolio %}
    <li><a href="{{ item.url }}">{{ item.title }}</a></li>
  {% endfor %}
</ul>
```

## Front Matter for Collection Items

Collection items can have front matter just like regular pages and posts. This allows you to define metadata for your collection items. For example:

```yaml
---
title: "My Portfolio Item"
date: 2023-01-01
---
```

In this example, the `title` and `date` variables are defined in the front matter of a portfolio item.

For more information on collections and how to use them in Jekyll, refer to the official [Jekyll documentation](https://jekyllrb.com/docs/collections/).
