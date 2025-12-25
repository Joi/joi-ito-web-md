---
title: "BT appears to be blocking third-party VoIP"
date: 2004-10-28T00:00:00
permalink: https://joi.ito.com/weblog/2004/10/28/bt-appears-to-b.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2004/10/28/bt-appears-to-b.html
extracted: 2025-12-25
---

> David Beckemeyer
>
> [BT appears to be blocking third-party VoIP](http://www.toyz.org/mrblog/archives/00000173.html)
>
> I've been biting my tongue on this since I first ran across it several months back. But now I have to say something. If someone can prove me wrong on this, fine, I'll post a retraction, but now I'm going to say it: **British Telecom appears to be explicitly blocking VoIP for their DSL subscribers.**
>
> I've worked with an associate to examine the situation and all signs point to an explicit blocking of VoIP. In Cisco ACL-speak, it appears there is a rule somewhere in the BT network being applied to inbound packets of the form:
> > deny udp any eq 5060 any

If this is true, this is VERY bad behavior. 5060 is the port that SIP uses. I can understand why a phone company wouldn't want "free phone calls over the Internet" running on their system, but this is exactly the kind of behavior that makes Internet folks dislike telephone company control.

Can anyone else corroborate this fact?

*VoIP stands for "Voice over IP" and SIP is the open standard "Session Initiation Protocol" used to set up calls over the Internet*

UPDATE: Looks like it is a customer router issue, but still may be BT driven. [Update on Mr. Blog.](http://www.toyz.org/mrblog/archives/00000174.html)