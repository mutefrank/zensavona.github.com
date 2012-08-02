{% assign post = site.posts.first %}
{% assign content = post.content %}
---
layout: page
title:  post.title
tagline: Supporting tagline
---
{% include JB/setup %}

<h1 class="entry-title">
{% if post.title %}
    <a href="{{ root_url }}{{ post.url }}">{{ post.title }}</a>
{% endif %}
</h1>
<div class="entry-content">{{ content }}</div>