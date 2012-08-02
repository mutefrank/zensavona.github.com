---
layout: page
title:  Speed, Weed & Rubies.
tagline: Supporting tagline
---
{% include JB/setup %}

<ul class="no-decoration">
    {% for post in site.posts limit 4 %}
    <li class="no-decoration"><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
        {{ post.content | strip_html | truncatewords:75}}<br>
            <a href="{{ post.url }}">Read more...</a><br><br>
    {% endfor %}
</ul>
