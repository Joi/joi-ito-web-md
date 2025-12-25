---
title: "Low cost GPS jammer"
date: 2002-12-29T00:00:00
permalink: https://joi.ito.com/weblog/2002/12/29/low-cost-gps-ja.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2002/12/29/low-cost-gps-ja.html
extracted: 2025-12-25
---

This may not help Sadaam, but just in case you're put under GPS surveillance house arrest by an oppressive government, you'll need to learn how to build your own GPS jammer.
> [phrack](http://www.phrack-dont-give-a-shit-about-dmca.org/show.php?p=60&a=13)
>
> ```
>   A low cost device to temporarily disable the reception of the civilian  
>
> course acquisition (C/A) code used for the standard positioning service  
>
> (SPS)[1] on the Global Positioning System (GPS/NAVSTAR) L1 frequency of  
>
> 1575.42 MHz.
> ```

This is accomplished by transmitting a narrowband Gaussian noise signal,  
with a deviation of +/- 1.023 MHz, on the L1 GPS frequency itself. This  
technique is a little more complicated than a simple continuous wave (CW)  
jammer, but tends to be more effective (i.e. harder to filter) against  
spread spectrum based radio receivers.