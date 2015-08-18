---
layout: default
title: Food
permalink: food/
---

#Food

<ul>
{% for post in site.categories.food %}
<li>{{ post.date | date_to_string }} <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
 
