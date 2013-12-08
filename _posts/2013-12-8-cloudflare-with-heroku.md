---
layout: default
title: Using Cloudflare with Heroku
---

#Using Cloudflare with Heroku

So you've got your shiny new domain, and have pushed your site up to Heroku, but how exactly do you get them to play nicely? Well, it's easy and here is how.

First you need to change your current DNS to use Cloudflare's DNS and wait until that propagates across the internet. While you're waiting you can configure your Cloudflare settings by making a CNAME record for ``*`` and ``www`` which is an alias of yourapp.herokuapp.com.

After this, you need to modify Cloudflare's page rules to have ``yourdomain.com/`` forward to ``www.yourdomain.com/`` and ``yourdomain.com/*`` forward to ``www.yourdomain.com/$1``.

That should be all you need to use Cloudflare to speed up your site while using Heroku to host it!