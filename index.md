---
layout: default
title: Recently...
---
{% include JB/setup %}


{% for post in site.posts limit:3 %}
<h3>
    <a href="/" rel="bookmark" title="Permanent link to ">{{ post.title }}</a>
</h3>
<span>{{ post.date | date: '%B' }} {{ post.date | date: '%e' }}, {{ post.date | date: '%Y' }}</span>
<p>
    {{ post.content }}
</p>
{% endfor %}