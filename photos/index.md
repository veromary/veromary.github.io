---
layout: default
title: Photos
permalink: photos/
---

<h1>Photos</h1>
<img src="family04.jpg" alt="Old Family Photo" width="375"
height="248">

<p>Posts from the Photos category:</p>


<ul>
{% for post in site.categories.photos %}
<li>{{ post.date | date_to_string }} <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
 <ul>
<li><a href="11.html">2011</a></li>
<li><a href="10.html">2010</a></li>
<li><a href="09.html">2009</a></li>
<li><a href="0801.html">2008</a></li>
<li><a href="0702.html">2007</a></li>
<li><a href="bernard.html">Bernard's Birth and Baptism</a></li>
<li><a href="0506.html">Three Boys</a> June 2005</li>
<li><a href="anthony.html">Anthony's Birth and Baptism</a></li>
<li><a href="nov04.html">Patrick and Chris</a> - November
2004</li>
<li><a href="mar04.html">A day with Nanna and Granddad</a> -
March 2004</li>
<li><a href="nov03.html">Patrick and Christopher (and Mum and
Dad)</a> - November 2003</li>
<li><a href="aug03.html">Patrick and Christopher</a> - August
2003</li>
<li><a href="chris.html">Christopher's Birth and Baptism</a></li>
<li><a href="patrick.html">Patrick's Birth, Baptism and Baby
photos</a></li>
<li><a href="../garb.html">Brandt Garb Guide</a></li>
<li><a href="../mini.html">Peter's Minis</a></li>
</ul>
<img src="umina.jpg" alt=
"Umina Beach with Mum, Anthony, Patrick and Christopher" width=
"247" height="185">


<p></p>

<br>

   
