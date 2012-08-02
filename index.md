---
layout: page
title: Hello Zen!
tagline: Supporting tagline
---
{% include JB/setup %}

{% for post in site.posts.newest limit 1 %}
{% include JB/post_content %}
{% endfor %}