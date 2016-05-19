---
title: Raspberry Pi chat server in the home
layout: post
category: Computers
image:
   teaser: raspi400.jpg
comments: true
---

![Raspberry Pi](/images/raspi800.png)

This morning's diversion was setting up a chat server on the Raspberry Pi.

The Raspberry Pi is a gadget that seems so full of possibilities, but hard to settle on one idea to run with.

I installed prosody on the Pi:

```
sudo apt-get install prosody
```

Then I edited the config file thus:

```
sudo nano /etc/prosody/prosody.cfg.lua
```

The things to change are :

* VirtualHost - I set it to `raspberrypi` to match the default hostname on Raspbian.
* admin - adding in parents as admins so only parents start multi user chatrooms
* enabling multi user chat (MUC) plus restricting room creation like this:

```
Component "conference.raspberrypi" "muc"
    restrict_room_creation = true
```

I think everything else was left as default.

Then restart prosody for these changes to take effect:

```
sudo /etc/init.d/prosody restart
```

Then I made some users:

```
sudo prosodycrl adduser *name*@raspberrypi
```

Then installed [pidgin](http://www.pidgin.im) on the other computers and logged in using the Facebook(xmpp) setting and raspberrypi as the server.

###Windows XP

One of our laptops runs Windows XP and this could not see the server at raspberrypi.  Linux uses this avahi thing and Windows needs [the Apple Bonjour Printer Driver](https://support.apple.com/kb/DL999).  

Once this was installed it still wouldn't work so I edited the Windows Hosts file `C:\Windows\System32\Drivers\etc\hosts`

Logging into the modem I was able to find and fix the raspberrypi ip address to 10.1.1.20.

Back to `C:\Windows\System32\Drivers\etc\hosts` I added the line:

```
10.1.1.20    raspberrypi
```

and then finally the Windows XP machine was able to find the raspberrypi and everything was fine.

It can be handy to have a live chat thing when juggling several different students at different levels tackling different problems.

