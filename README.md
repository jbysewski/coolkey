What is this?
=============

This is a fork of CoolKey to support ActivKey SIM with up to 8 slots.

History
=======

CoolKey is a RedHat project that provides support for various smartcards on Linux machine.

It worked well for ActivIDentity ActiveKey SIM token with a patch https://bugs.launchpad.net/ubuntu/+source/coolkey/+bug/786682 to support zero length certificates.

Newer versions of ActivClient client (software for Windows) decided to use a diffent slot for certificate storage. (Information about certificates can be found in "Help -> Troubleshooting"). ActiveKey SIM supports up to 8 certificates.

Unfortunately CoolKey doesn't support multiple slots:

> To accomplish that vision we are focusing on building complete support for CoolKey on exactly one token. As the system is built out, we can add token support.

There is also no option to override ActivClient behaviour or to move certificate to another slot.

So there's no other choice as to add support for more slots.

Installation
============

This repo contains a branch that should fix the problem above. Select it and see its readme file.

You can also install it from a dedicated ppa repository: https://launchpad.net/~markus-tisoft/+archive/coolkey

Notice that I'm not responsible for any damage caused by this software. Use it at your own risk.

Upstreaming
===========

My solution is quite dirty. Someone more experienced should look into it and improve.

Here's a related bug in RedHat's bugzilla:
https://bugzilla.redhat.com/show_bug.cgi?id=826286
