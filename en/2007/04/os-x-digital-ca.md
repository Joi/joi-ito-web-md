---
title: "OS X digital camera import bug with UTC"
date: 2007-04-21T00:00:00
permalink: https://joi.ito.com/weblog/2007/04/21/os-x-digital-ca.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2007/04/21/os-x-digital-ca.html
extracted: 2025-12-25
---

I've tracked down a weird bug when importing images on my Mac. When my OS X time zone is set to UTC, all of my images are dated 1/1/1970. When I set it to a time zone like JST, the date becomes correct. The dates are affected on my RAW files after they are imported. In other words, when I change to UTC, all of the dates become 1/1/1970. When I change the time zone, images imported in the past become correct.

However, if I process an image using Capture One and convert RAW to jpg, the bad date is fixed and doesn't revert when I change the time zone.

This occurs if I copy the files from the memory directly or if I use Image Capture to import the images.

Has anyone else had this problem? I guess most people don't have their computers set to UTC...