---
layout: page
title: Pagination
---

# Pagination

Pagination is a feature in Jekyll that allows you to split your content into multiple pages. This is particularly useful for blogs and other content-heavy sites.

## Basic Usage

To enable pagination in your Jekyll site, you need to add the following configuration to your `_config.yml` file:

```yaml
paginate: 5
paginate_path: "/page:num/"
```

In this example, the `paginate` setting specifies the number of posts per page, and the `paginate_path` setting defines the URL structure for the paginated pages.

## Pagination in Templates

To display paginated content in your templates, you can use the `paginator` object provided by Jekyll. Here's an example of how to use it in a template:

```liquid
{% for post in paginator.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
{% endfor %}

<div class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}">Previous</a>
  {% endif %}
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}">Next</a>
  {% endif %}
</div>
```

In this example, the `paginator.posts` array contains the posts for the current page, and the `paginator.previous_page` and `paginator.next_page` variables are used to create navigation links for the paginated pages.

## Customizing Pagination

Jekyll allows you to customize the pagination behavior by using plugins or custom code. For example, you can create a custom pagination plugin to implement advanced pagination features like infinite scrolling or AJAX-based pagination.

For more information on pagination and how to use it in Jekyll, refer to the official [Jekyll documentation](https://jekyllrb.com/docs/pagination/).
