---
layout: page
title: Permalinks
---

# Permalinks

Permalinks in Jekyll allow you to define the URL structure for your pages and posts. This helps you create clean and user-friendly URLs for your content.

## Basic Usage

To set a permalink for a page or post, use the `permalink` front matter variable. For example:

```yaml
---
layout: post
title: "My First Post"
permalink: /my-first-post/
---
```

In this example, the URL for the post will be `/my-first-post/`.

## Permalink Styles

Jekyll supports several built-in permalink styles, including:

- `date`: Includes the date in the URL (e.g., `/2023/01/01/my-first-post/`).
- `pretty`: Creates clean URLs without file extensions (e.g., `/my-first-post/`).
- `ordinal`: Includes the post number in the URL (e.g., `/1-my-first-post/`).
- `none`: Uses the default URL structure (e.g., `/my-first-post.html`).

You can set the default permalink style for your site in the `_config.yml` file. For example:

```yaml
permalink: pretty
```

## Custom Permalinks

You can also create custom permalink structures using placeholders. Here are some common placeholders:

- `:year`: The year of the post (e.g., `2023`).
- `:month`: The month of the post (e.g., `01`).
- `:day`: The day of the post (e.g., `01`).
- `:title`: The title of the post (e.g., `my-first-post`).

For example, to create a custom permalink structure that includes the date and title, you can use the following syntax:

```yaml
permalink: /:year/:month/:day/:title/
```

In this example, the URL for the post will be `/2023/01/01/my-first-post/`.

For more information on permalinks and how to use them in Jekyll, refer to the official [Jekyll documentation](https://jekyllrb.com/docs/permalinks/).
