---
title: "mail2entry moblog code update"
date: 2003-03-12T00:00:00
permalink: https://joi.ito.com/weblog/2003/03/12/mail2entry-mobl.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2003/03/12/mail2entry-mobl.html
extracted: 2025-12-25
---

Aron Atkins has updated mail2entry, the PERLPython script that Sen wrote for posting email with attached pictures to MT.

Continue reading [mail2entry moblog code update](https://joi.ito.com/weblog/2003/03/12/mail2entry-mobl.html#more).

This version includes:

- parsemsg.parse supports multiple image attachments; the content of each image is returned in a list.
- Added saveimage.py, which takes that list of image bodies and either saves them to disk or posts them via newMediaObject.
- Move parsing of sys.argv out of main() -- this avoids the import \* warnings.
- Template changes in settings.py which allow for multiple images. supports both
- JPEG and GIF image types.

His site is at [here](http://www.gweep.net/~aron/) and the code is [here](http://www.gweep.net/~aron/mail2entry-2003-03-10b.tgz).

Also, I have been talking to [Karl Dubost](http://www.la-grange.net/moblog/) about taking over the management of the code and he is also working on a new version. If you guys could coordinate, that would be great. ;-)

*Thanks to both of you for continuing the effort!*