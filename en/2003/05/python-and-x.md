---
title: "Python and XML and the agony of defeat"
date: 2003-05-10T00:00:00
permalink: https://joi.ito.com/weblog/2003/05/10/python-and-xml.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2003/05/10/python-and-xml.html
extracted: 2025-12-25
---

I learned Python (thanks to Sen) in a week. I wrote a birthday script, a script to scrape blogshares and put the shareholders in my sidebar and even wrote a vcard handler. I was on a roll. Then... Sifry sent me some Technorati stuff to mess with. XML? Cool, should be easy. I was just about to do the Parsing XML section of [Dive Into Python](http://diveintopython.org/) anyway. Great! ...not
> Dive Into Python
>
> As I was saying, actually parsing an XML document is very simple: one line of code. Where you go from there is up to you.

So 2 hours later, I have 4 different installations of Python on my PowerBook and one on my FreeBSD machine and I can't get Mark's first example to work
> >>> xmldoc = minidom.parse('~/diveintopython/common/py/kgp/binary.xml')

I've just about given up. The O'Reilly Python & XML is cryptic, I've googled around and tried a bunch of stuff and am totally frustrated. I guess I thought I was becoming a programmer, but I'm just a wimpy little script kiddie. >sigh<

Continue reading [Python and XML and the agony of defeat](https://joi.ito.com/weblog/2003/05/10/python-and-xml.html#more).

So for those of you who are interested in how far I've gotten. I did see a post by Mark that the Python that comes with OS X doesn't have the necessary XML libraries so I downloaded PyXML. Well, when I try to install it, it says "NameError: name 'distutils' is not defined"

On my FreeBSD Box the Python error is:  
> Traceback (most recent call last):  
> File "", line 1, in ?  
> File "/usr/local/lib/python2.2/site-packages/\_xmlplus/dom/minidom.py", line 19  
> 15, in parse  
> return expatbuilder.parse(file)  
> File "/usr/local/lib/python2.2/site-packages/\_xmlplus/dom/expatbuilder.py", li  
> ne 924, in parse  
> result = builder.parseFile(fp)  
> File "/usr/local/lib/python2.2/site-packages/\_xmlplus/dom/expatbuilder.py", li  
> ne 207, in parseFile  
> parser.Parse(buffer, 0)  
> xml.parsers.expat.ExpatError: undefined entity: line 119, column 366