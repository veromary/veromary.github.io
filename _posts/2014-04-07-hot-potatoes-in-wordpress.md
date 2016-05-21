---
layout: post
title: Hot Potatoes in Wordpress
date: 2014-04-07 14:50:00 +1100
category: Computers
comments: true
image:
  teaser: hotpot.jpg
---

![Hot Potatoes](/images/hotpot.jpg)

This page started life as an incoherent test post, but turns out to be one of the most popular articles, so here goes making it coherent.

The first thing to do to get your hotpotato up on your Wordpress blog is to upload it.  Now, Wordpress.com doesn't let you upload html files.  You could upload your html file to [Dropbox](http://dropbox.com) and make a link to that file [like this](https://www.dropbox.com/s/9ipscc4si3cy0iv/test.htm?dl=0)

**UPDATE**: Dropbox seems to prevent the javascript from working, so unfortunately this won't work.  You can instruct readers to download the html file from dropbox and open it on their local copy, but this sounds rather complicated.

Wordpress.com is also fussy about what it embeds, so you can't embed it in a page, but people can click on your link to reach the hot potato.  Dropbox mixes up the addresses, so the Masher sets of hotpotato quizzes won't work.  Unless you have a self-hosted Wordpress.org site.

### The Self Hosted Wordpress Way

Self hosted Wordpress *does* let you upload and embed html files.  First upload using the Media Library, then get the link address.

In the page you want to embed your quiz, go to edit the page/post, switch from Visual to Text mode, use this code:

{% highlight html linenos=table %}

<iframe src="http://yourwebsite.com/path-to-your.htm" height="400" width="400"></iframe>

{% endhighlight %}

Which should give something like this:

<iframe src="/assets/docs/test.htm" height="400" width="400"></iframe>

You may need to adjust the width and height according to your quiz.

I hope that helps,

Veronica

### PS: the Github Pages way

There is another way that is free and very satisfying using [Github Pages](https://pages.github.com/).  It is also very useful for collaborative projects and keeping track of changes.  There is a lot to learn in the process, but if you are passionate about education, then that can be a bonus.

This whole website is hosted with github pages now.

### PPS: Quiz Faber

An Italian programmer from Turin has made an awesome program that's even better than Hot Potatoes : [Quiz Faber](http://www.quizfaber.com)

It is a windows program which is really close to working under Linux, but not quite there yet (Next Release, any minute now, for the last few years)

