---
title: "Archiving Digital Journalism"
date: 2019-03-07
---
There are several approaches to saving digital news:

- Passively, rely on Internet archiving sites to crawl your work.
- Actively, tell Internet archiving sites to crawl your work, via something like Ben Welsh's Save My News TKTK link, which is powered by the open-source library TKTK "save page now"

Audience Q: Is there a way to automate archiving, so that people can just archive all the tweeted links? Answer: Not yet, but you could build it! The biggest mistake that people make is to assume that Archive.org scrapes the things you link to. Go out and make sure.

Audience note: I use the Wayback Machine (from the Internet Archive) to link to source webpages.

Audience note: The version of the page that gets saved on the Wayback machine is just a flat version of the page; if it depends on serverside code, it won't work.

Ben Welsh proposes that CMSes automatically publish to the Wayback Machine; audience member notes that there are WordPress plugins TKTK link that do that.

The Internet Archive is just a single site; it's a single point of failure. Welsh's SaveMyNews uses archive.is and perma.link. But imagine a future where there are many archives, all mirroring each other!

Now a quick note about how the LA Times archives Jonathon Gold's food critic work. He died at 57, last year. The LAT Data Desk has been for 5 years the publishers of Gold's 101 best restaurants. Each of the 5 eyars had different takes. They weren't published not to latimes.com but to ballots.latimes.com, because ballots.latimes.com was an Amazon cloud server that dynamically rendered the database in response to reader queries. Dynamic sites allow for great user experience, but are hard to archive, and are likely to crash.

The site was written in Python; the LAT Data Desk used `django-bakery` TKTK link to turn the dynamic site into a flat file. When a dynamic page is requested, the app creates static files that are easily served. And now that the whole app is static, they ran the entire set of generated pages into Save Page Now to back it up. And because all the apps on ballots.latimes.com have been baked statically, the Data Desk has changed ballots.latimes.com to be served from an Amazon S3 bucket.

