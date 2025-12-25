---
title: "My M8 and my struggle with color"
date: 2007-03-14T00:00:00
permalink: https://joi.ito.com/weblog/2007/03/14/my-m8-and-my-st.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2007/03/14/my-m8-and-my-st.html
extracted: 2025-12-25
---

[![Conference pass for my M8](http://farm1.static.flickr.com/129/418443041_75922c3a73_m.jpg)](http://www.flickr.com/photos/joi/418443041/ "Photo Sharing")

I got the [Leica M8](http://www.leica-camera.us/photography/m_system/m8/) last week. My logic was that I had a lot of M series lenses already. I had waited too long to get the Digital back for my R8 and it was way too low-resolution by the time I finally got it. I didn't want to wait so long to get the M8.

Although I guess I'm still happy I got the M8, I didn't do my research and there are a number of bugs that I'm having to work around.

I already knew about the first bug by the time I actually got my M8. I wanted to use Aperture for my workflow, but Apple doesn't support Leica M8 RAW format so [you need to make a fake RAW profile for the M8 and use the Adobe RAW converter to convert the M8 RAW files before importing them into Aperture.](http://www.leica-camera-user.com/digital-forum/16559-how-use-aperture-m8-dng-files.html) (Thanks for the pointer Ian.) One more step, but OK. Fine. I'm going to assume that Apple will eventually support the M8. (Maybe a bad assumption.)

I encountered my second bug when I started shooting at SXSW. Black cloth and other things in the conference sessions came out looking purple instead of black. Several people saw me visibly panic as I previewed photos that I was taking of Phillip Torrone who had a black shirt on. Someone told me to google "IR Leica M8". Tadaaa... a serious flaw.

The Leica sensor is overly sensitive to infrared and certain materials when lit by a source with strong IR (The lights in the conference) will show up as purple. Since it's not a color balance issue, you can't just white balance it out. [The Leica forums explained that the Pro version of Capture One had profiles that could substantially improve the image and make it look almost right](http://www.leica-camera-user.com/digital-forum/9178-magenta-work-around-capture-one-workflow.html). However, it looks like you will need to get a [special UV/IR filter and a firmware upgrade](http://www.leica-camera.us/news/news/1/4913.html) that is still TBD from Leica to correct for it. Doh. Even after the firmware comes out, needing a new filter for all of my lenses really puts a dent in the [amazing backward compatibility](http://flickr.com/photos/joi/414336715/) that Leica is all about.

After sort of getting this all working, I finally uploaded a bunch of stuff to Flickr and noticed that things looked washed out and lacked saturation compared to how they appeared on my screen. It turns out that Firefox on the Mac doesn't recognize the ICC profile tags so I need to remap the colors and export the images in Aperture instead of just dragging them into Flickr. (Thanks Kevin!) I'm exporting to sRGB IEC61966-2.1 which seems to fix it.

Compare [an image remapped/exported to sRGB IEC61966-2.1](http://flickr.com/photos/joi/420719564/)  
[![SET Players](http://farm1.static.flickr.com/127/420719564_a709638065_m.jpg)](http://www.flickr.com/photos/joi/420719564/ "Photo Sharing")  
to  
[one which is not](http://flickr.com/photos/joi/420682047/)  
[![SET Players](http://farm1.static.flickr.com/179/420682047_33da93e178_m.jpg)](http://www.flickr.com/photos/joi/420682047/ "Photo Sharing")  
in Firefox and Safari on a Mac. They will look the same in Safari, but the second one will look washed out in Firefox.) I also learned, from the same post that Macs and Windows machines typically use a different gamma so even if I get the colors right, the gamma will be off for most of the world. [There is a page that clearly describes these phenomena](http://www.gballard.net/psd/go_live_page_profile/embeddedJPEGprofiles.html).

I guess the lesson here is that the closer you get to perfection, the harder it gets. I'm not upset and I'm learning a lot about imaging and color in the process. It's just amazing how complicated the world of digital photography has become for me in the last few days.

UPDATE: After the OSX update, Aperture is crashing randomly and frequently. Anyone else getting this?