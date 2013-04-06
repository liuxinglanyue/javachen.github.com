---
layout: index
title : Categories
---


Categories
--------
{% for category in site.categories %}

<a id="{{category[0]}}"></a>

### {{category[0]}} ({{category[1] | size}}) ###

{% for post in category[1] %}

- [{{post.title}}]({{post.url}})

{% endfor %}

{% endfor %}
