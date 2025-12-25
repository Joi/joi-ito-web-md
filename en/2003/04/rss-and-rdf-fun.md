---
title: "RSS and RDF fun"
date: 2003-04-06T00:00:00
permalink: https://joi.ito.com/weblog/2003/04/06/rss-and-rdf-fun.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2003/04/06/rss-and-rdf-fun.html
extracted: 2025-12-25
---

[![consynrsss.gif](http://joi.ito.com/archives/images/consynrsss-thumb.gif)](http://www.oreilly.com/catalog/consynrss/)I have to admit that I've been feeling guilty about talking so much about RSS and RDF without REALLY understanding what I was talking about, a state which I think I fixed today. (While staring a pile of books on democracy and constitution law...) First I read [Ben Hammersley's new O'Reilly Book *Content Syndication with RSS*](http://www.oreilly.com/catalog/consynrss/). I went and surfed around the Net reading the documentation on RSS and RDF on a variety of sites. Then I decided to try to do something interesting. I've created a new RSS 2.0 feed which includes the entry comments, links to the email or URL of authors of the comments, includes the number of comments in the guid's so that you get an update when someone posts a comment and permalinks in the feed to the comment as well as the item. I included the [BlogChannel module](http://backend.userland.com/blogChannelModule) so I could include my blogroll from [Blogrolling.com](http://www.blogrolling.com). Thanks to [Noel Jackson](http://www.noeljackson.com/archives/000243/index.php), I figured out how to include my [Creative Commons License](http://www.creativecommons.com) in my RSS feed.

The feed is [here.](http://joi.ito.com/index20.xml) Feedback would be appreciated.

So, I finally understand what Dave, Boris and many others have been trying to get me to understand. It's flexibility vs. simplicity. RSS 2.0 is cool because it extends the simplicity of the original 0.9x RSS with modules. RSS 1.0 is cool because there are so many things you can do with RDF. The problem with RDF is that it is so ugly to read. Honestly, this morning I wouldn't understand what I have just written. The geek inside me is now awake and I want to learn everything there is to know about RDF, but it took a bunch of people pummeling me to get me to care, whereas plain old RSS 0.91 got me excited just looking at the code. So, I guess I'm on Dave's side in terms of keeping it simple and helping to get it widely accepted. On the other hand, the RDF stuff really does allow a lot of the semantic web attributes that we are talking about in the emergent democracy debate and the RDF framework, once it really starts to get picked up inside of applications could be really powerful.

Anyway, the main feed for my blog is now my [RSS 2.0 feed](http://joi.ito.com/index20.xml).

*Sorry to everyone who has to reload the feeds because I've rebuild everything. Also, I've made them the last 30 entries instead of just 15 since that was the limit for 0.91. Let me know if that's too many entries.*