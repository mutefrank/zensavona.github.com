---
layout: default
title: Zen Savona - Ruby, CodeIgniter, Startups, Psychedelics
---
{% include JB/setup %}


{% for post in site.posts limit:3 %}
<center>
	<h2>
	    <a href="{{ post.url }}" rel="bookmark" title="Permanent link to ">{{ post.title }}</a>
	</h2>
	<span>{{ post.date | date_to_long_string }}</span>
</center>
<p>
    {{ post.content }}
</p>
<hr />
<br />
{% endfor %}