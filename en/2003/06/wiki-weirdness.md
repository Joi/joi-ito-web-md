---
title: "Wiki Weirdness"
date: 2003-06-01T00:00:00
permalink: https://joi.ito.com/weblog/2003/06/01/wiki-weirdness.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2003/06/01/wiki-weirdness.html
extracted: 2025-12-25
---

I'm having trouble with my wiki. My apache error log said "Premature end of script headers: moin.cgi". Testing moin.cgi, I get a python error saying that "SERVER\_NAME" is not defined. Hmm... I wonder if someone changed the settings on the machine. I haven't done anything. The files all seem to be there. I've got to run to go give a talk, but I'll be back in a few hours to work on this problem. Until then my Wiki will be offline. My apologies. You can still get the TechnoBot source [here](http://joi.ito.com/src/technobot-0.121/technobot.py).

PS If anyone wants to help me debug this in a few hours (moinmoin/python/apache/freebsd) send me an email. ;-) [[email protected]](/cdn-cgi/l/email-protection)

UPDATE: paulproteus on #moin helped fix the wiki. It's working now. Thanks Paul!! The first line in the cgi script was wrong. Now the BIG question is... how did it get changed in the middle of the night?