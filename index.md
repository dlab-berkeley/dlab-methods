---
layout: default
title: Meetings
---
{% include site_vars %}

{% for post in site.posts %}
{{ DIVIDER }}
*{{ post.date | date_to_long_string}}*
## [{{ post.title }}]({{ BASE_PATH }}{{ post.url }})

{{ post.excerpt}}

[read more]({{ BASE_PATH }}{{ post.url }})

{% assign DIVIDER = "---" %}
{% endfor %}
