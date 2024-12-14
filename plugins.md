---
layout: page
title: Plugins
---

# Jekyll Plugins

Jekyll allows you to extend its functionality using plugins. Plugins can be used to add custom features, generate content, and more.

## Installing Plugins

To install a Jekyll plugin, you need to add it to your `Gemfile` and run `bundle install`. For example, to install the `jekyll-feed` plugin, add the following line to your `Gemfile`:

```ruby
gem "jekyll-feed"
```

Then run the following command to install the plugin:

```sh
bundle install
```

## Using Plugins

Once a plugin is installed, you can configure it in your `_config.yml` file. For example, to use the `jekyll-feed` plugin, add the following line to your `_config.yml` file:

```yaml
plugins:
  - jekyll-feed
```

## Popular Plugins

Here are some popular Jekyll plugins:

- `jekyll-feed`: Generates an Atom feed for your site.
- `jekyll-seo-tag`: Adds SEO tags to your site's head.
- `jekyll-sitemap`: Generates a sitemap for your site.
- `jekyll-paginate`: Adds pagination support to your site.

For more information on Jekyll plugins, refer to the official [Jekyll documentation](https://jekyllrb.com/docs/plugins/).
