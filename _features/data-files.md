---
layout: page
title: Data Files
---

# Data Files

Jekyll allows you to use data files (in formats like YAML, JSON, and CSV) to store structured data that can be accessed and used in your templates.

## Using Data Files

To use data files in your Jekyll site, create a `_data` directory in the root of your site. Inside this directory, you can add your data files. For example, you can create a `data.yml` file:

```yaml
- name: John Doe
  email: john.doe@example.com
- name: Jane Smith
  email: jane.smith@example.com
```

## Accessing Data Files

You can access the data in your data files using Liquid syntax. For example, to display the names and emails from the `data.yml` file, you can use the following code:

```liquid
<ul>
  {% for person in site.data.data %}
    <li>{{ person.name }} - {{ person.email }}</li>
  {% endfor %}
</ul>
```

## Supported Data Formats

Jekyll supports the following data formats:

- YAML
- JSON
- CSV

For more information on using data files in Jekyll, refer to the official [Jekyll documentation](https://jekyllrb.com/docs/datafiles/).
