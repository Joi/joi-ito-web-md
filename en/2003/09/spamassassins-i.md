---
title: "SpamAssassin's in my way..."
date: 2003-09-01T00:00:00
permalink: https://joi.ito.com/weblog/2003/09/01/spamassassins-i.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2003/09/01/spamassassins-i.html
extracted: 2025-12-25
---

Two of my emails to [ado](http://www.kung-foo.tv/blog/) got blocked by [SpamAssassin](http://au2.spamassassin.org/index.html) today. According to him SpamAssassin message, my server was an open relay. I asked about this on [#joiito](http://joi.ito.com/joiwiki/IrcChannel) and [crysflame](http://monsoon.typepad.com/atoll/) pointed to an article that explains that [Osirusoft](http://relays.osirusoft.com/) which Spam Assassin uses to check for open relays is broken. "Apparently, after having been DDOS'ed, the Osirusoft people have 'given up the ghost' and are now returning back every IP as a spam source when queried!"

So if you want to get mail from me, please reconfigure SpamAssassin as [explained on the use PERL; site.](http://use.perl.org/article.pl?sid=03/08/27/1626247)

UPDATE: [µthe inquirer](http://www.theinquirer.net/?article=11263) has an article about this.