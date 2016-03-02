---
layout: default
title: About Brandt Lab
permalink: about/
---

# About Brandt Lab

This somewhat aimless website seemed like a good idea way back when "id.au" domains were new.

For the last decade it has seen many new facelifts, each time accumulating more odds and ends.  One attempt to keep track of these articles is [siteindex]({{ site.url }}/siteindex.html)

Now and then I group posts by Categories, like these:

<ul>
{% for category in site.categories %}<li style="text-transform: capitalize"> <a href="{{ site.url }}/{{ category | first | slugify }}">{{ category | first }}</a></li>{% endfor %}
</ul>


