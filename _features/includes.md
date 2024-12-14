---
layout: page
title: Includes
---

# Includes

Includes in Jekyll are reusable snippets of code that can be included in your layouts and pages. This allows you to modularize your code and keep it DRY (Don't Repeat Yourself).

## Basic Usage

To create an include, add a new HTML or Markdown file to the `_includes` directory in your Jekyll site. For example, you can create a `header.html` include:

```html
<header>
  <h1>{{ site.title }}</h1>
</header>
```

## Using an Include

To use an include, use the `include` tag in your layouts or pages. For example:

```liquid
{% include header.html %}
```

In this example, the contents of the `header.html` include will be inserted at the location of the `include` tag.

## Passing Variables to Includes

You can also pass variables to includes, allowing you to create more dynamic and customizable snippets. For example:

```html
<header>
  <h1>{{ include.title }}</h1>
</header>
```

To pass a variable to the include, use the following syntax:

```liquid
{% include header.html title="My Custom Title" %}
```

In this example, the `title` variable will be passed to the `header.html` include and used to set the header title.

## Common Includes

Here are some common includes you might use in your Jekyll site:

- `header.html`: A reusable header for your site.
- `footer.html`: A reusable footer for your site.
- `navigation.html`: A reusable navigation menu for your site.

For more information on includes and how to use them in Jekyll, refer to the official [Jekyll documentation](https://jekyllrb.com/docs/includes/).
