---
layout: page
title: Sass/SCSS
---

# Sass/SCSS

Jekyll supports Sass and SCSS, allowing you to write your stylesheets using these powerful CSS preprocessors.

## Using Sass/SCSS in Jekyll

To use Sass or SCSS in your Jekyll site, create a `_sass` directory in the root of your site. Inside this directory, you can add your Sass or SCSS files. For example, you can create a `styles.scss` file:

```scss
// styles.scss
$primary-color: #333;

body {
  color: $primary-color;
}
```

## Including Sass/SCSS in Your Site

To include your Sass or SCSS files in your site, create a main stylesheet file in your site's `_assets` directory. For example, you can create a `main.scss` file:

```scss
// main.scss
@import "styles";
```

In this example, the `styles.scss` file is imported into the `main.scss` file.

## Configuring Sass/SCSS

You can configure Sass and SCSS options in your `_config.yml` file. For example, you can set the output style and source map options:

```yaml
sass:
  style: compressed
  source_map: true
```

For more information on using Sass and SCSS in Jekyll, refer to the official [Jekyll documentation](https://jekyllrb.com/docs/assets/).
