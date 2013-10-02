---
layout: default
title: Puppet for Desktop Management
---

#Puppet for Desktop Management

I have begun using puppet not for server management, the common use case, but to manage my desktop locally. 

##Why would I do this?
This began because I had my laptop operating systems become corrupted, don’t know how, and don’t care to know as it would take more time than it’s worth to determine that. It became so corrupt, not even Linux’s recovery mode would work properly.  I then had to go through the pain of reinstalling and slowly getting my computer back to the state it was. This is unacceptable in this day and age, so I decided to learn puppet by managing my own computer.

##The advantages?
I now have a completely reproducible system, and can go from a fresh install to back to my lovely environment with all my must have application in just a few minutes. The biggest pain point is simply installing puppet and the site.pp dependencies, and for that I’ve decided even that can be solved with a straightforward python script, as python is available by default in most linux distributions.

This ability alone allows me to rethink my relationship to my computer. With the help of offsite backup and a little scripting, my computer becomes completely replaceable in such a way that causes minimal pain. 