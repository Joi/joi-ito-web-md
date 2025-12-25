---
title: "Real-time streaming is stupid"
date: 2005-02-17T00:00:00
permalink: https://joi.ito.com/weblog/2005/02/17/realtime-stream.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2005/02/17/realtime-stream.html
extracted: 2025-12-25
---

I'm listening to [Andrew Odlyzko](http://www.dtc.umn.edu/~odlyzko) giving a talk right now about why Quality of Service (QoS) and real-time streaming is stupid. He showed a slide showing that P2P and other traffic are generally transmitting files at faster speeds than their bit rates. Basically, if you cache and buffer, you can have outages in the downloads and you'll usually be fine. I agree. I can see why carriers would want to spread the rumor that QoS is some feature that we have to have, but it's strange that so many researchers seem to think we will need QoS supported video streaming. Maybe they need to stop watching cable TV.