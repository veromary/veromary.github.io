---
layout: default
title: House and Garden
---

# House and Garden.

This category was coined to contain the post about moving to Wagga, which never eventuated to anything, but maybe one of our kids will take it up and we can become resident grandparents - the mind boggles.

But it might just be the category to help get the house painted and generally finished up.  If we include Gardening as well then we might document the vegie patch adventures too.

## Recent posts

<ul>
{% for post in site.categories.House %}
<li>{{ post.date | date_to_string }} <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>{% endfor %}
</ul>


