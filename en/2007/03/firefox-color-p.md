---
title: "Firefox color profile handling"
date: 2007-03-15T00:00:00
permalink: https://joi.ito.com/weblog/2007/03/15/firefox-color-p.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2007/03/15/firefox-color-p.html
extracted: 2025-12-25
---

I am visiting Mozilla today for a board meeting. After a few inquiries, I was able to track down Stuart Parmenter who is working on the color profile issue that I [blogged about in my last post](http://joi.ito.com/archives/2007/03/14/my_m8_and_my_struggle_with_color.html). The good news is that Stuart is a photo and color geek and has already figured this out and fixed it. ([It is Bug 16769 in Bugzilla@Mozilla](https://bugzilla.mozilla.org/show_bug.cgi?id=16769).) Firefox 3.0 will have a bunch of improvements including dealing with color profiles in images properly. There are a few more tests that are required, but it will soon be in the tree and should be available in the Alpha of [Firefox 3.0](http://www.mozilla.org/projects/firefox/3.0a1/releasenotes/).

Special thanks to Stuart for the tutorial on color!

UPDATE: Special special thanks to Tim Rowley who did most of the implementation part in Mozilla.

UPDATE 2: The fix should be in Alpha 4 of Firefox 3.0 not Alpha 3 that is coming out next in a week or two.