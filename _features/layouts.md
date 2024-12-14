---
layout: page
title: Layouts
---

# Layouts

Layouts in Jekyll allow you to define the structure of your pages and posts. They help you maintain a consistent look and feel across your site.

## Creating a Layout

To create a layout, add a new HTML file to the `_layouts` directory in your Jekyll site. For example, you can create a `default.html` layout:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>{{ page.title }}</title>
  </head>
  <body>
    {{ content }}
  </body>
</html>
```

## Using a Layout

To use a layout, specify the layout name in the front matter of your Markdown or HTML files. For example:

```yaml
---
layout: default
title: "My Page"
---
```

In this example, the `default` layout will be used for the page, and the title will be set to "My Page".

## Nested Layouts

Jekyll also supports nested layouts, allowing you to create more complex page structures. To use a nested layout, specify the parent layout in the front matter of your layout file. For example:

```html
---
layout: parent
---

<!DOCTYPE html>
<html>
  <head>
    <title>{{ page.title }}</title>
  </head>
  <body>
    {{ content }}
  </body>
</html>
```

In this example, the `parent` layout will be used as the base layout for the current layout.

## Common Layouts

Here are some common layouts you might use in your Jekyll site:

- `default`: A basic layout for your pages and posts.
- `post`: A layout specifically for blog posts.
- `page`: A layout for standalone pages.

For more information on layouts and how to use them in Jekyll, refer to the official [Jekyll documentation](https://jekyllrb.com/docs/layouts/).
