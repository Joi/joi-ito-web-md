---
title: "Lunch with Aaron"
date: 2003-04-01T00:00:00
permalink: https://joi.ito.com/weblog/2003/04/01/lunch-with-aaro.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2003/04/01/lunch-with-aaro.html
extracted: 2025-12-25
---

|  |
| --- |
| Aaron and Daiji Hirata talking about UTF-8 |

Had lunch with Aaron Swartz.
> [Aaron Swartz: The Website](http://www.aaronsw.com/)
>
> Aaron Swartz is a teenage writer, coder, and [hacker](http://www.tuxedo.org/~esr/faqs/hacker-howto.html#WHAT_IS). In 1999, he won the ArsDigita Prize for excellence in building non-commercial web sites. In 2000, he co-authored [the RSS 1.0 specification](http://purl.org/rss/1.0/), now used by thousands of sites to notify their readers of updates. In 2001, he [joined](http://lists.w3.org/Archives/Public/w3c-rdfcore-wg/2001Apr/0062) the W3C's [RDF Core Working Group](http://www.w3.org/2001/sw/RDFCore/) which is developing the format for the Semantic Web. In 2002, he became the [Metadata Advisor](http://www.creativecommons.org/aboutus/people#15) to the [Creative Commons](http://www.creativecommons.org/). The rest of the time, he works on [a variety of other projects](http://www.aaronsw.com/projects).

He has a [Weblog](http://www.aaronsw.com/weblog/) and also runs the [Google Weblog](http://google.blogspace.com/). [Larry](http://cyberlaw.stanford.edu/lessig/blog/) sent me email to make sure that we met while Aaron was visiting Japan. Thanks Larry!

So, we talked a lot about RSS. RSS 2.0 isn't truely XML compliant, but even one of the co-founders of XML, Tim Bray, uses PERL regex to parse XML a lot of the time and doesn't bother with the formalities of running a true XML parser.
> [Tim Bray's Blog](http://tbray.org/ongoing/When/200x/2003/03/16/XML-Prog)
>
> Now here's the dirty secret; most of it is machine-generated XML, and in most cases, I use the perl regexp engine to read and process it. I've even gone to the length of writing a prefilter to glue together tags that got split across multiple lines, just so I could do the regexp trick.

Well, if one of the founders of XML thinks that XML parsers are a pain, they probably are. Most RSS news feeders do not parse RSS as XML, but just clean it up and figure it out and doesn't reject non-XML compliant feeds. I have a feeling that these standards committees, while very important, are starting to get away from the original spirit of the Internet of "keep it simple, make it work".

Aaron, is a no-bullshit guy and who spent a lot of time with the W3C folks trying to get them to understand why RSS was so important. Well, I say, lets get on with it and just make it all work, even if it isn't formal XML. RSS is hot right now and wide adoption could revolutionize everything from digital cameras to DRM.