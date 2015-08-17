---
layout: default
title: Education
---

#Education

##Recent posts

{% for post in site.posts %}
{% if post.category contains 'Education' %}
* {{ post.date | date_to_string }} [{{ post.title }}]({{ site.url }}{{ post.url }})
{% endif %}
{% endfor %}

##Things we are currently studying
<ul>
<li><a href="http://www.classicalliberalarts.com/family/index.cfm">Classical Liberal Arts Academy</a> for Catechism and Grammar. Our sub expires at the end of June 2015, and we do not plan to move into the new system, so we hope to have a good go at finishing some courses.  Wish us luck!</li>
<li><a href="http://mathsonline.com.au/login">Maths Online</a> - A nice, clear, uncluttered Australian Maths program.</li>
<li><a href="http://learnenglish.britishcouncil.org/en/">British Council's Learn English</a> - aimed at adults learning English as a second language, but very interesting.  Also has a Kids and Teen section.</li>
<li><a href="http://codecademy.com">codecademy</a> - for learning some programming.  Also <a href="http://scratch.mit.edu">Scratch</a>.</li>
<li><a href="http://typingweb.com/tutor">Typing Web</a> a free online typing tutor.</li>
<li><a href="http://quizlet.com/class/140924/">Catholic's Latin Instructor</a> at Quizlet for Latin Vocabulary.</li>
<li><a href="https://docs.google.com/forms/d/1bc0TiOzx3HZTYdQvPN0I7wLW7u4b2sodTjkgIR0D8Z4/viewform?usp=send_form">Book log</a></li>
</ul>


##Ideas for homeschooling and general teaching/learning stuff

[The Catholic's Latin Instructor]({{ site.url }}/latin/) - a project to turn Fr Edward Caswall's book into an online course.

Here are two old pages:
[Home Education]({{ site.url }}/homeschool.html) and [Teaching]({{ site.url }}/teaching.html) resources, ideas, recommended reading and things like that. Lots of book reviews.


