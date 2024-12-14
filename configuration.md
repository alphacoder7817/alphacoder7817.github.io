---
layout: page
title: Configuration
---

# Jekyll Configuration

Jekyll provides a wide range of configuration options to customize your site. These options can be set in the `_config.yml` file, which is located in the root directory of your Jekyll site.

## Basic Configuration

Here are some basic configuration options you can set in the `_config.yml` file:

- `title`: The title of your site.
- `description`: A short description of your site.
- `url`: The base URL of your site.
- `baseurl`: The subdirectory of your site (if any).

## Permalinks

You can configure the permalink structure for your site using the `permalink` option in the `_config.yml` file. Here are some common permalink structures:

- `/:categories/:year/:month/:day/:title.html`
- `/:year/:month/:day/:title.html`
- `/:year/:month/:title.html`

## Markdown

Jekyll supports different Markdown processors. You can specify the Markdown processor to use in the `_config.yml` file:

- `markdown: kramdown`
- `markdown: redcarpet`

## Plugins

Jekyll allows you to extend its functionality using plugins. You can specify the plugins to use in the `_config.yml` file:

```yaml
plugins:
  - jekyll-feed
  - jekyll-seo-tag
```

## Deployment

You can configure deployment settings for your Jekyll site in the `_config.yml` file. Here are some common deployment options:

- `destination`: The directory where the generated site will be placed.
- `exclude`: A list of files and directories to exclude from the generated site.
- `include`: A list of files and directories to include in the generated site.

For more information on Jekyll configuration options, refer to the official [Jekyll documentation](https://jekyllrb.com/docs/configuration/).
