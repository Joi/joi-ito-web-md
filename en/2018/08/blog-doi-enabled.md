---
title: "Blog DOI enabled"
date: 2018-08-22T00:00:00
permalink: https://joi.ito.com/weblog/2018/08/22/blog-doi-enabled.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2018/08/22/blog-doi-enabled.html
extracted: 2025-12-25
---

As part of my work in developing the [Knowledge Futures Group](https://mitpress.mit.edu/kfg) collaboration with the MIT Press, I'm doing a deep dive into trying to understand the world of academic publishing. One of the interesting things that I discovered as I navigated the different protocols and platforms was the Digital Object Identifier (DOI). [There is a foundation](http://www.doi.org/) that manages DOIs and coordinates a [federation of registration agencies](http://www.doi.org/registration_agencies.html). DOIs are used for many things, but the general idea is to create a persistent identifier for some digital object like a dataset or a publication and manage it at a meta-level to the URL, which might change over the lifetime of the drafting and the publication of an academic journal article or the movement of a movie through a supply chain.

One registration agency, [Crossref](https://www.crossref.org/), focuses on DOIs for academic publications and citations across these publications and their service has proliferated the use of DOIs as a convenient and effective way of rigorously managing and tracking citations. Many services, like [ORCID](https://orcid.org/) which manages affiliations and publications for academics, use DOIs as one way to import and manage publications.

Although DOIs can be used for many things, because they are somewhat non-trivial to get and set up and because of the success of Crossref which services academic publishers, they have become somewhat synonymous with authority, trustworthiness and formal publishing. Although [Geoffrey Bilder from Crossref warns us that this is not true](https://www.crossref.org/blog/dois-unambiguously-and-persistently-identify-published-trustworthy-citable-online-scholarly-literature-right/) and that DOIs shouldn't signal that, I think that in fact they do, for now.

Something I noted as I started playing with all of the various tools available to academics to manage their profiles and their citations, and having only one peer reviewed paper to my name so far (thanks Karthik, Chelsea and Madars for that!), was that my blog posts weren't getting indexed. Also, as I was doing research while working on my dissertation, [I noticed that blogs generally weren't very heavily cited](https://joi.ito.com/weblog/2018/05/28/citing-blogs.html). Using my privilege and in the name of research, I started bugging Amy Brand, director of the MIT Press, who worked on the adoption of DOIs when she was at Crossref. I asked whether I could get DOIs for my blog posts.

It wasn't as easy as it sounds. First of all, you need a DOI prefix--sort of like a domain--registered through one of the registration providers. Amy helped me get one, under the MIT Press, via Crossref. Boris defined the DOI suffix format, set up a submission generator and integrated everything into my blog. Alexa from MIT Press worked on getting the DOIs from my blog to Crossref. The next problem is that "blogs" are not a category of "thing" in the DOI world so the closest category according to the experts was "dataset." So, this thing, formerly known as a blog post, that I'm writing is now a dataset contribution to the scholarly world. I do believe that it meets the standard of something that someone might possibly want to cite, so I don't feel guilty having a DOI assigned to it. I hope that Crossref would consider adding a blog post "creationType" or extend the schema more broadly for other citable web resources.

Also, I wish APA would update their [blog citation format](http://blog.apastyle.org/apastyle/2016/04/how-to-cite-a-blog-post-in-apa-style.html) so that the name of the blog is part of the citation and not just the URL. In a rare act of disobedience, I've gone rogue and added the name of this blog in the APA citation template on this blog against their official guidelines. Strictly speaking, the APA citation for this post would be "Ito, J. (2018, August 22). Blog DOI enabled. [Blog post]. <https://doi.org/10.31859/20180822.2140>" but the citation tool here gives you: "Ito, J. (2018, August 22). Blog DOI enabled. Joi Ito's Web [Blog post]. <https://doi.org/10.31859/20180822.2140>". Sorry not sorry if you get dinged on your paper for using the modified format.

> I may sound a bit naive, but as I read more academic papers in fields that I work in, I realize that they tend to cite academic papers more than blog posts even if there are better blog posts than the cited papers. It makes sense, but just noticing more specifically first hand.
>
> — Joi Ito (@Joi) [May 13, 2018](https://twitter.com/Joi/status/995638425922560000?ref_src=twsrc%5Etfw)

[When I tweeted about the issue of blog posts not being cited](https://twitter.com/Joi/status/995638425922560000), one of the concerns from the Twittersphere was lack of peer review for blogs. I think this is a valid request and concern, but not all things that are worthy of being cited need to be peer reviewed. On the other hand, clearly citing others, noting any contributors and their contribution to a blog post, and having some sort of peer review when it makes sense, is probably a good idea.

I'm not stuck on the use of the world "blog" although that's what I think this is. I just think that having an ability to rapidly publish, as blogs enable us to do, and have it connect to the world of academic literature is something worth considering.

Recently, academic preprint servers have become very popular and a growing number of academics are skipping journal publishing altogether, putting their papers on archive servers and presenting them at conferences instead of submitting them to journals.

My sense is that blogs can play a role in this ecosystem if we can tweak the academic publishing side, the culture on both sides and some of the practices on the blogging side. Geoffrey suggests that DOIs should be assigned to anything that is citationworthy and I agree, but I think that blogs are and could be even more like informal publications than just a merely citationworthy blobs of data.

Boris Anthony who has been my partner in thinking about this stuff and has been designing and maintaining my blog for the last 15 years or so has been thinking deeply about the semantic web and the creation of knowledge and was critical in [getting it sorted out on this blog](https://borisanthony.net/2018/08/22/doi-enabling-jois-weblog-phase-i/). He was also the one who convinced me not to convert all of my blog posts into DOI'ed objects, but to pick the ones that might have some scholarly value. :-)

PS There appears to be a [DOI plugin for Wordpress](https://wordpress.org/plugins/the-winnower-publisher/) using a prefix registered by the developer.

###### Credits

[Boris Anthony for doing the actual technical and design work to get the DOIs deployed on this site and for help with the ideas and the editing of the post.](https://borisanthony.net/2018/08/22/doi-enabling-jois-weblog-phase-i/)

Amy Brand for her guidance in getting, understanding and writing about DOIs.

Alexa Masi for helping us sort out how to get the DOIs properly formatted and sent over to Crossref.