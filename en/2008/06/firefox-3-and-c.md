---
title: "Firefox 3 and Color Management"
date: 2008-06-21T00:00:00
permalink: https://joi.ito.com/weblog/2008/06/21/firefox-3-and-c.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2008/06/21/firefox-3-and-c.html
extracted: 2025-12-25
---

Firefox 3 supports color profiles, but you have to turn this setting on manually.

[There are some great blog posts that describe this in detail](http://www.dria.org/wordpress/archives/2008/04/29/633/), which you should read for more information, but this "feature" greatly improves the accuracy of the colors.

Color profiles provide a kind of map for your computer about what colors in an image should look like. Your camera, monitor and printer all have color profiles. The color profile of a image will allow your printer and monitor to accurately render the colors of an image by mapping the image colors to the profile of your printer or monitor.

What Firefox (and IE before IE 7) used to do was to ignore the color profile in images and just tell the OS that the profile was a generic color profile (sRGB). Roughly speaking, this is fine since MOST image files are sRGB. However, for anyone tweaking their saturation or color balance in iPhoto, Aperture, Lightroom, etc. it was EXTREMELY frustrating because this often caused images posted on the Internet to look different (washed out and desaturated) from what they looked like in the image editor. Although "save as sRGB" got around some of these issues, it still caused problems in many cases. ([Some color geeks helped me understand in a discussion on one of my Flickr photos](http://flickr.com/photos/joi/2459733138/).)

Anyway, I think that the esoteric discussions about color are interesting, but for most people, the bottom line is, if you turn color profile support "on" on Firefox 3, many images will end up appearing much closer to the color of the original and less washed out. You do this by typing "about:config" in the address bar of Firefox 3. Click thru confirmation page and find: gfx.color\_management.enabled. Double click that until it says "true". Then restart Firefox 3.

There are a number of monitor color calibration gadgets and software packages like Eye One Match which will allow you to calibrate your monitor (and camera and printer). If everyone actually did this, we'd all be seeing the same colors. The problem is that many uncalibrated monitors show colors (even across the same brand of monitors) differently. That means that with uncalibrated monitors, the person creating the photo can end up with "warped" colors in the image which then get warped again when being displayed on another uncalibrated monitor. In the past the browser also added another level of "warpage" but with color profile support, you're one step closer to accurate color. To go all the way, calibrate your monitor.

Why doesn't Mozilla support color profiles by default like Safari does? (It is turned off by default on IE 7 too.) It appear to cause a 10-15% performance hit. I've had it turned out since I've been using it and it's not noticeable to me however. Anyway, I hear they are working on optimizing it and turning it on as a default in the future. For now, you'll have to void the warranty and hack Firefox.