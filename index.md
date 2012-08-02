---
layout: page
title: Hello Zen!
tagline: Supporting tagline
---
{% include JB/setup %}

{% for post in site.posts.newest %}
{% include JB/post_content %}
{% endfor %}