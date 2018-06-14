---
layout: markdown
title: Course list
---

{% assign sorted = (site.posts | sort: 'date') %}
{% for post in sorted %}
## [{{post.title}}]({{post.url}})

{{post.excerpt}}

{% endfor %}
