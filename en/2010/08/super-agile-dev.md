---
title: "Super-agile development of Aproxymator with HyperTiny"
date: 2010-08-31T00:00:00
permalink: https://joi.ito.com/weblog/2010/08/31/super-agile-dev.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2010/08/31/super-agile-dev.html
extracted: 2025-12-25
---

[![Bamboo thicket](http://aproxymator1.s3.amazonaws.com/1378841612_7ec4bd62d9.jpg)](http://www.aproxymator.com/photos/joi/1378841612 "Bamboo thicket by Joi, on Aproxymator")  
*[Bamboo thicket on Aproxymator](http://www.aproxymator.com/photos/joi/1378841612)*

I've been talking a lot about agile development and how the speed and cost to a minimum viable product (MVP) has been reduced so much that it is changing the startup scene completely. I've been working with [Pivotal Labs](http://pivotallabs.com/) on my fund and my portfolio companies, having them help get many of my companies up and running with their best practices to take advantage of the latest methods.

Recently, the CTO of Pivotal Labs, Ian McFarland, sent me an excited email about a shop in Ireland called [HyperTiny](http://www.hypertiny.ie/). If Pivotal Labs is the High Council of Jedi Masters, HyperTiny are two young Jedi at some outpost. Ian had recently done a project with Paul (developer) and Brian (designer) at HyperTiny and they knocked out an MVP for him in 2 weeks.

I was fascinated with the idea that one designer and one developer writing fully test driven development (TDD) and [Pivotal Tracker](http://www.pivotaltracker.com/) based code could super-code a Rails 3 product in weeks. It made total sense, but I wanted to see it myself. I engaged [HyperTiny](http://www.hypertiny.ie/) to scratch an itch that has been bugging me ever since I moved to the United Arab Emirates (UAE).

In the UAE, Flickr is unfortunately blocked. People trying to access Flickr get a silly screen from the ISP telling you that it's not safe. I'm working to try to get this unblocked, but in the mean time, none of my friends in the UAE can see my Flickr photos. I've been dreaming of a site that mirrors my Flickr photos and provides a way for me to have most of the functionality of Flickr from an unblocked site.

I talked to Paul and Brian and my [Freesouls.cc](http://freesouls.cc/) friend Christopher who has been banging on the Flickr API for years and came up with a basic feature set. We talked on Skype and put all of the features (stories) into Pivotal Tracker. While we were on Skype, I set up a GitHub repository, a Engine Yard account, set up my Amazon Web Services (AWS) account and got the domain name ([Aproxymator](http://aproxymator.com/)) and off we went.

After that, every two or three days, we'd do a conference call on Skype, going through the delivered features, giving feedback, iterating and coming up with new ideas. Paul would walk us through the code and explain how the tests worked, how he was refactoring everything and helping us keep our heads around everything. Along the way, I pulled in Sean, Ado, Jim, James and Kuri and it turned into a Rails 3 tutorial as well.

One month (three actual work weeks of Paul and Brian's time) later, we have a working site. It's still half way between a vanity service to fit my own needs and something useful to others. I'm going to have to noodle on it and figure out whether we should continue iterating on the multiuser stuff or to focus on making it more useful for me.

Right now, it allows you to enter your own AWS account and use the service to backup and mirror your own Flickr feed. It's got some basic API stuff that we're working on. Christopher is now taking over the code, which was super-easy with all of the stories in Pivotal Tracker, all of the tests properly written and everything beautifully documents.

One thing that I do know for sure now. You can get to an MVP with one designer and one engineer and HyperTiny (and other shops like them) can help teams bootstrap in a way that allows a smooth transfer of the code to another development team. I saw it with my own eyes. True story.