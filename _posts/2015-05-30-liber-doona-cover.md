---
layout: post
title: Liber Doona Cover
category: Music
image:
   feature: liberdoonacover.jpg
   teaser: liberdoona400x250.jpg
comments: true
---

A crazy idea while doing the washing up:

A photomosaic doona cover of a Latin Mass scene using pages from the Liber Usualis!

I've installed [metapixel](https://github.com/schani/metapixel).

To turn [liberusualis.pdf](http://www.musicasacra.com/music/) into a folder full of jpgs:

    mkdir liberusrc
    for i in {0001..2333}; do convert -density 300 ~/Documents/Library/liberusualis.pdf[$i] -resize 500 -gravity center -crop 440x730+0+0 +repage liberusrc/liberu$i.jpg; echo $i; done

That last line takes a Long Time to run for my Core 2 vPro HP Compaq computer.  The upside of slow computers is that the compile time facilitates other activities such as documentation, food preparation and domestic maintenance.

Metapixel also requires a destination directory:

    mkdir liberudst

Then the next step should be something like:

    metapixel-prepare -r liberusrc liberudst --width=440 --height=730

Drumroll please...

    metapixel --metapixel suitablephoto.jpg awesomemosaic.png -l liberudst -s 10

Now, the thing I should have checked in the beginning:

Duvet Covers (125 DPI):

 * 8570x11250 pixels for the twin duvet (including bleeding)
 * 11000x11000 pixels for the queen duvet (including bleeding)
 * 13500×11462 pixels for the king duvet (including bleeding)

So if I'm working with multiples of 440x730, then for my image to be big enough for the biggest duvet cover, then I'm looking at a mosaic about 30x15 pages.  That's not so big after all!

I guess the next question is, where to find a suitable photo!

**UPDATE:** the finished product is [available here](http://www.redbubble.com/people/veronicabrandt/works/15071278)

