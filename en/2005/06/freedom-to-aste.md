---
title: "Freedom to Asterisk"
date: 2005-06-25T00:00:00
permalink: https://joi.ito.com/weblog/2005/06/25/freedom-to-aste.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2005/06/25/freedom-to-aste.html
extracted: 2025-12-25
---

Last night I got [Asterisk](http://www.asterisk.org/) working on my PowerBook with the help of Benjamin who runs [astmasters.net](http://sunrise-tel.com/). Asterisk is an open source PBX. It allows your computer to send, receive, route and provide services on a wide variety of voice connections including SIP, IAX and various interfaces for normal phone lines. I've always had fairly complicated phone line and call management needs and now I can program everything myself. There is an amazing feeling of liberation when you realize how much control of your phone system you can actually have. Asterisk is a bit difficult to do without some help, but once you start to get your head around it, it feels like you're running a mini phone company. They even use legacy words like "trunk lines" which were named after the cabinets in the phone companies that held the groups of 9999 lines. It's going to take me awhile to get it completely configured, but I'm not going to feel truly VoIPy until I am in total control of my phone system.

Take THAT telephone monopolies! ;-)

UPDATE: François asked for more detail in the comments.

I'm using the PowerBook now mostly to play around. It will eventually be on a stationary machine. The first step will be to forward all of my calls to Asterisk. These include Vonage, Free World Dial, Voice Pulse and a few other VoIP things that I have. I will also try to find a service provider who will take all of my business lines and convert them to VoIP and forward them to my PBX. Vonage and Sound Pulse will allow me to dial out. The idea is to have all of my calls aggregate at my Asterisk PBX. Then, I can have various profiles on Asterisk that I can change in a number of ways. I'm hoping I can use, email, phone, Jabber presence, SMS and various other methods of changing my profile. The profiles will be set up to forward calls appropriately to me or my assistants. The calls can forward to a soft phone on my computer, my cell phone or any other phone that I register with Asterisk. I can also send calls to voicemail. If I can get caller ID working properly, I can set up different groups to allow me to let certain people through for emergencies.

Because the system is so flexible, there are a variety of configurations so I'm trying to figure out what I really want and how best to do it before investing in a bunch of interface cards. One key point will be whether I do the POTS termination myself or have a service provider manage my POTS lines. (POTS = Plain Old Telephone Service)