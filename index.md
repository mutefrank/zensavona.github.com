---
layout: page
title:  Speed, Weed & Rubies.
tagline: Supporting tagline
---
{% include JB/setup %}

{% assign post = site.posts.first %}
{% assign content = post.content %}

<h2 class="entry-title">
{% if post.title %}
    <a href="{{ root_url }}{{ post.url }}">{{ post.title }}</a>
{% endif %}
</h1>
<div class="entry-content">{{ content }}</div>