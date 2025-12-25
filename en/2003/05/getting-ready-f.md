---
title: "Getting ready for phase two of Technorati hacks"
date: 2003-05-13T00:00:00
permalink: https://joi.ito.com/weblog/2003/05/13/getting-ready-f.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2003/05/13/getting-ready-f.html
extracted: 2025-12-25
---

Good [entry in Web Dawn](http://web-dawn.hypermart.net/archives/000009.html) about Technorati as a reputation system. *Via [Marc Canter](http://blogs.it/0100198/2003/05/12.html#a1066)*. So we need to get Sifry to catch permalinks of what people are linking to better and we need a little more metadata in the XML feeds. The addition metadata which would allow me to implement something like a reputation system would be:

1) The name of the person who posted the entry  
2) The URL (permalink) of the entry on my blog the link points to  
3) Filtering out of all blogroll "false positives" and entry imbedded links only or a separate feed for blogs rolls. (Can you work with Jason D on this?)  
4) Implement pagerank. Take the inbound links/blogs assign the blogs with high inbound links/blogs with high page rank and then do another calculation assigning outbound links from those blogs higher value and give each page a technorati ranking. And do this every 5 minutes.  
5) Make a contextual pagerank where the user can set their own rankings for blogs and ask technorati to calculate the final pagerank.

It would be cool if 4 & 5 could be done on your own site in some way, but not sure how that would work. Anyway, a bit off the top of my head, but I'm trying to figure out my NEXT super duper python project.

Lucky for me Aaron just [wrote xmltramp](http://www.aaronsw.com/weblog/000918) and made my life a whole lot easier.
> Aaron Swartz
>
> In trying to write some code to use [the new Technorati API](http://developers.technorati.com/), I noticed that all the tools for accessing XML documents *sucked*. So I wrote my own: [xmltramp](http://www.aaronsw.com/2002/xmltramp/). It makes handling XML documents in Python a piece of cake:

*Via [Cory](http://www.boingboing.net/)*

By the way, Dave Sifry and Aaron Swartz rock.