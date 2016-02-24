---
layout: default
title: Computers
permalink: computers/
---

# Computers

<ul>
{% for post in site.categories.Computers %}
<li>{{ post.date | date_to_string }} <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
 
