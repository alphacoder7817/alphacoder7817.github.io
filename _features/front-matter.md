---
layout: page
title: Front Matter
---

# Front Matter

Front matter is a key feature in Jekyll that allows you to define metadata for your pages and posts. This metadata can be used to control the layout, title, and other properties of your content.

## Basic Usage

Front matter is defined at the top of your Markdown or HTML files, enclosed within triple-dashed lines. Here's an example of basic front matter:

```yaml
---
layout: post
title: "My First Post"
date: 2023-01-01
---
```

## Common Front Matter Variables

Here are some common front matter variables you can use in your Jekyll site:

- `layout`: Specifies the layout to use for the page or post.
- `title`: Sets the title of the page or post.
- `date`: Sets the date of the post (for blog posts).
- `categories`: Specifies the categories for the post.
- `tags`: Specifies the tags for the post.

## Custom Front Matter Variables

You can also define custom front matter variables to store additional metadata for your content. For example:

```yaml
---
layout: post
title: "My First Post"
author: "John Doe"
---
```

In this example, the `author` variable is a custom front matter variable that can be used to store the author's name.

## Accessing Front Matter Variables

You can access front matter variables in your templates using Liquid syntax. For example, to display the title of a post, you can use the following code:

```liquid
<h1>{{ page.title }}</h1>
```

For more information on front matter and how to use it in Jekyll, refer to the official [Jekyll documentation](https://jekyllrb.com/docs/front-matter/).
