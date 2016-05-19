---
layout: post
title: Print Etsy Inventory
category: Computers
comments: true
image:
   teaser: printetsy400x250.jpg
---

[Working Online Demo](http://www.brandt.id.au/print-etsy-inventory)

![screenshot](https://veromarybrrr.files.wordpress.com/2016/05/printetsy.png?w=750)

Etsy is a pretty and useful platform for selling handmade stuff.  It isn't always the most powerful platform for getting things done, but there are lots of commercial third party programs to help out.

But just to print out product thumbnails and titles of current listings for a quick stocktake shouldn't be that hard.

So, yesterday I did it the long way - taking the csv download and using vim regular expressions to search and replace strings to make a passable html file to print the 200+ active listings for [my husband's Etsy shop](http://avalonprand.etsy.com).  Along the way it occurred to me that this should be easy to make into a web app.

So, today I tried out a few different approaches and finally settled on [JQuery-csv](https://github.com/evanplaice/jquery-csv) and now I can proudly present to the world: [Print Etsy Inventory](http://www.brandt.id.au/print-etsy-inventory)

Now we still have a lot of stocktaking to go to stock the new online shop [www.peterbrandt.com.au](http://www.peterbrandt.com.au).  At least this is a step in the right direction.
