---
layout: page
title: Assets
---

# Assets

Jekyll allows you to manage and include various types of assets in your site, such as images, CSS, and JavaScript files.

## Including Assets

To include assets in your Jekyll site, you can place them in the `assets` directory. For example, you can create an `assets` directory in the root of your site and add an image file:

```
assets/
  └── images/
      └── example.jpg
```

## Using Assets in Templates

You can reference and use assets in your templates using relative URLs. For example, to include an image in a Markdown file, you can use the following syntax:

```markdown
![Example Image](/assets/images/example.jpg)
```

To include a CSS file in an HTML layout, you can use the following syntax:

```html
<link rel="stylesheet" href="/assets/css/styles.css">
```

## Asset Management Plugins

Jekyll also supports various plugins for managing and optimizing assets. Some popular plugins include:

- `jekyll-assets`: A plugin for managing and optimizing assets, including CSS, JavaScript, and images.
- `jekyll-sass-converter`: A plugin for converting Sass/SCSS files to CSS.

For more information on managing and including assets in your Jekyll site, refer to the official [Jekyll documentation](https://jekyllrb.com/docs/assets/).
