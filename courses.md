---
layout: markdown
title: Course list
---

{% for post in site.posts %}
## [{{post.title}}]({{post.url}})

{{post.excerpt}}

{% endfor %}
