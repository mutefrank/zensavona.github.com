---
layout: default
title: Recently...
---
{% include JB/setup %}


{% for post in site.posts limit:3 %}
<center>
	<h2>
	    <a href="{{ post.url }}" rel="bookmark" title="Permanent link to ">{{ post.title }}</a>
	</h2>
</center>
<span>{{ post.date | date: '%B' }} {{ post.date | date: '%e' }}, {{ post.date | date: '%Y' }}</span>
<p>
    {{ post.content }}
</p>
<hr />
<br />
{% endfor %}