---
title: "mail2entry script for MT moblog"
date: 2002-12-26T00:00:00
permalink: https://joi.ito.com/weblog/2002/12/26/mail2entry-scri.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2002/12/26/mail2entry-scri.html
extracted: 2025-12-25
---

I've been getting a lot of attention for my moblog even though it's not such a big technical feat really. All you need is a script to convert email into MT entires. We're going to make the code available so that hopefully more people can experiment with moblogging. It's being made available under a standard GPL v.2 license. Please let me know what you think. We hope to continue to improve it. The file is available at: <http://joi.ito.com/archives/src/mail2entry-2002-12-25.tgz>

Here are some notes about installation.
> Warning

This is a first attempt -- there are some things missing, but someone w/appropriate UNIX experience should be able to succeed in installation and configuration. I may update the instructions as I get feedback.

Prerequisites

The ability to read English and follow simple instructions.

A host connected to the Internet which can receive email [1] and:

Python >= 2.2.2  
MT  
enabled w/ the XML-RPC interface  
a blog (determine your blog id)  
a blog user, the associated password [2]

Please note that this code was designed to run on the host which the blog itself is running on. Other configurations may be possible, but I don't recommend them and don't plan on supporting them at the moment.*Thanks for all the work on this Sen*

Please send feedback to me for the moment. We may designate someone to be in charge of the code later. Also, since it uses XML-RPC, it should be easy to get it to work with other blog platforms.

PS The GPL license on this code overrides the CC license on this site.