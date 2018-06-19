---
layout: markdown
title: Course list
---

{% assign sorted = (site.posts | sort: 'date') %}
{% for post in sorted %}
-----------------------------------
## [{{post.title}}]({{site.baseurl}}{{post.url}})

*{{post.date | date: "%-d %B @ %-I %P"}} - {{post.room}}*

{{post.excerpt}}
{% endfor %}
