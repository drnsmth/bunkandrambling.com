---
title: bunk and rambling - on the internet
layout: default
---

# Past posts
{% for post in site.posts %}
* {{ post.date | date: "%Y-%m-%d" }} <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}

