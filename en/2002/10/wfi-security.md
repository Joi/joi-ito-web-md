---
title: "W-Fi Security?"
date: 2002-10-31T00:00:00
permalink: https://joi.ito.com/weblog/2002/10/31/wfi-security.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2002/10/31/wfi-security.html
extracted: 2025-12-25
---

> InfoWorld
>
> [WiFi eyes better wireless LAN security](http://www.infoworld.com/articles/hn/xml/02/10/30/021030hnwifi.xml?s=rss&t=news&slot=2)
>
> By Stephen Lawson   
> October 30, 2002 11:37 am PT
>
> THE WIRELESS ETHERNET Compatibility Alliance (WECA), which certifies IEEE 802.11 wireless LAN products with the WiFi label, on Thursday will announce a new set of mechanisms to combat the security problem that has plagued wireless LANs.
>
> A WECA official did not provide details of the mechanisms but said they are intended to replace the current security system based on WEP (Wireless Encryption Protocol).
>
> WEP, which is built in to products that use the IEEE 802.11b and 802.11a standards, is easy for intruders to break into, according to many analysts and other observers. A task group within the working group that administers 802.11 in the Institute of Electrical and Electronic Engineers Inc. (IEEE) is developing a new security specification that would require equipment to support several different strong algorithms for encrypting traffic. That work is not done yet, and products using it are not expected until the second half of next year.

Duh... This is a pretty big problem. People think that having a WEP key is actually secure. You can crack normal WEP keys in a few minutes by sniffing traffic and using programs such as [wepcrack](http://sourceforge.net/projects/wepcrack) which is available on the web. There are some chipsets out that have better security, but most of the AP's we all use are completely vulnerable. On the other hand, if you aren't worried about people hijacking traffic and if you encrypt everything you do internally, you're fine. Just don't for a moment think that just because you set a WEP key that you're secure. (Kudo's to Chris for telling me about wepcrack. ;-) )