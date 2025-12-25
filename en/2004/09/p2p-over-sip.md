---
title: "P2P over SIP"
date: 2004-09-16T00:00:00
permalink: https://joi.ito.com/weblog/2004/09/16/p2p-over-sip.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2004/09/16/p2p-over-sip.html
extracted: 2025-12-25
---

[Dr. Mark Petrovic](http://www.earthlink.net/about/leaders/bios/petrovic/) and David Beckemeyer at Earthlink R&D have developed a proof of concept P2P application using SIP called [SIPshare](http://www.research.earthlink.net/p2p/). SIP stands for [Session Initiation Protocol](http://www.toyz.org/cgi-bin/sipwiki.cgi) and is one of the key technologies for the open standards around Voice over IP (VoIP). This application is pure P2P use of SIP. It is completely decentralized. According to David Beckemeyer this project is quite important.
> David Beckemeyer in email
>
> This may not sound like that big of a deal, as file sharing has been done, but I think this is a really big event. It's not about file sharing. Nobody is really going to use the demo app Mark built. It's about demonstrating that pure P2P can be done over SIP and that SIP is about more than just voice and video.

In some sense, the SIP wars to me are about sneaking in some aspects of the original "stupid network" baack into the NAT hell we've created. If we can do what it takes to get NAT boxes to support SIP (be consistent in how they do NAT so the edges can use STUN et al), then we have reclamied the ability to have individually addressable nodes, where we use SIP as the new IP network almost. This may be getting carried away, but anyway...SIP has been waylaid in regulatory and execution problems in the past and many people have written it off as a non-starter. I'm seeing more and more companies who are actually using it for cool stuff and proving that it's ready for prime time now. If you written off SIP and haven't taken a look at what people doing with it for the last six months, I suggest you take another look.

*via [David Beckemeyer](http://www.toyz.org/mrblog/archives/00000168.html)*