---
layout: default
title: Meetings
---

{% for post in site.posts %}
{{ DIVIDER }}
*{{ post.date | date_to_long_string}}*
## [{{ post.title }}]({{ site.url }}{{ post.url }})

{{ post.excerpt}}

[read more]({{ site.url }}{{ post.url }})

{% assign DIVIDER = "---" %}
{% endfor %}
