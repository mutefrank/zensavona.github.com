---
layout: default
title: Recently...
tagline: Supporting tagline
---
{% include JB/setup %}

<h2>Latest entries</h2>
{% for post in site.posts limit:4 %}
<h3>
    <a href="/" rel="bookmark" title="Permanent link to ">{{ post.title }}</a>
</h3>
<span>{{ post.date | date: '%B' }} {{ post.date | date: '%e' }}, {{ post.date | date: '%Y' }}</span>
<p>
    {{ post.content | replace:'more start -->','' | replace:'<!-- more end','' }}
</p>
{% endfor %}