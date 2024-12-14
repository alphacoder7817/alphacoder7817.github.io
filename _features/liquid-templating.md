---
layout: page
title: Liquid Templating
---

# Liquid Templating

Liquid is a powerful templating language used in Jekyll to create dynamic and customizable templates. It allows you to embed logic and variables within your templates, making it easy to generate content dynamically.

## Basic Syntax

Liquid uses a combination of tags, filters, and objects to create dynamic content. Here are some basic examples:

### Outputting Variables

To output a variable, use double curly braces:

```liquid
{{ site.title }}
```

### Using Filters

Filters allow you to modify the output of a variable. For example, to convert a string to uppercase:

```liquid
{{ "hello" | upcase }}
```

### Control Flow

Liquid supports control flow statements like `if`, `else`, and `unless`:

```liquid
{% if page.title %}
  <h1>{{ page.title }}</h1>
{% else %}
  <h1>Untitled</h1>
{% endif %}
```

### Loops

You can use loops to iterate over collections of items:

```liquid
{% for post in site.posts %}
  <h2>{{ post.title }}</h2>
{% endfor %}
```

## Common Use Cases

Here are some common use cases for Liquid templating in Jekyll:

### Displaying Site Data

You can access site-wide data using the `site` object:

```liquid
<p>Site Title: {{ site.title }}</p>
<p>Site Description: {{ site.description }}</p>
```

### Including Partials

You can include partial templates using the `include` tag:

```liquid
{% include header.html %}
```

### Accessing Page Variables

You can access variables defined in the front matter of a page using the `page` object:

```liquid
<h1>{{ page.title }}</h1>
<p>{{ page.content }}</p>
```

For more information on Liquid templating and how to use it in Jekyll, refer to the official [Liquid documentation](https://shopify.github.io/liquid/).
