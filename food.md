---
layout: default
title: Food
permalink: food/
---

#Food

<ul>
{% for post in site.posts %}
{% if post.category contains 'Food' %}
<li>{{ post.date | date_to_string }} <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
{% endif %}
{% endfor %}
</ul>
 
