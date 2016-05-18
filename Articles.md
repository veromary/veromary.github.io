---
layout: archive
permalink: articles/
title: Articles
date: 2016-05-18T09:25:10+10:00
excerpt: Latest posts
ads: false
share: false
---


<ul style="list-style-type: none; padding-left: 0">
<li style="display: inline; padding-right: 20px"><strong>Categories:</strong></li>
{% for category in site.categories %}<li style="display: inline; padding-right: 20px"> <a href="{{ site.url }}/{{ category | first | slugify }}">{{ category | first }}</a></li>{% endfor %}
</ul>

<div style="clear: both"></div>

<div class="tiles">
{% for post in site.posts %}
	{% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->


<div style="clear: both"></div>
