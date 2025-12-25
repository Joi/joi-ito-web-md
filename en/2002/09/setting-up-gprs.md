---
title: "Setting up GPRS on Menorca"
date: 2002-09-17T00:00:00
permalink: https://joi.ito.com/weblog/2002/09/17/setting-up-gprs.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2002/09/17/setting-up-gprs.html
extracted: 2025-12-25
---

I'm going to write about setting up GPRS in Menorca because:

1) The line is so slow I can't read other people's blogs or my mail easily for new things.

2) I have nothing else to write about really...

3) This MAY come in handy for someone who is struggling like me.

Continue reading [Setting up GPRS on Menorca](https://joi.ito.com/weblog/2002/09/17/setting-up-gprs.html#more).

First, a disclaimer. I still don't understand GPRS and my conclusions below are based on trial and error and deduction. I may be complete wrong about some things.

First of all, GPRS roaming basically doesn't work in most places. Also, most support people don't know what you are talking about.

Second... Most phones act like they know what they are talking about or that they work properly, but they don't.

GPRS is different from using a GSM phone as a modem. It is a separate data network. Each carrier has their own "APN" which I guess stands for "Access Point Number" or something. The APN format is something like "airtelnet.es" for the Vodafone network in Spain. Now the APN in the APN field on the phone will be set for its WAP connection. IE airtelwap.es. This is the wrong APN. So just copying the fields from the phone settings to the computer DOESN'T WORK.

In addition to the APN, you will probably need an ID/PASSWORD. T-MOBILE told me that I didn't need one, but it didn't work without one so far. I had to call Vodafone to get one. I got one, but it didn't work. I called John who gave me his. He said that he had tested mutiple people using it at the same time and it was OK and that the SIM card holder was billed anyway so it wasn't any skin off his back. So... WHY THE HELL TO THEY HAVE THESE ID/PASSWORDS? Anyway, they will probably start blocking multiple log ins just like we did in the ISP business. So... you should probably get your own ID/PASSWORD if you need one and can figure out how to get once, it is totally NON-OBVIOUS. I had to call 3 support people before someone even told me they could give me one and that I needed one.

Also, default setting for my Nokia was "\*99#" to access the GPRS network. Well in Spain, it is "\*99\*\*\*1#" Don't get that wrong. Since "\*99#" is the default, I have to change the dialup settings for GPRS EVERY TIME I start up the computer. But that's OK. Since at least IT WORKS.

I am using a Nokia D211 which is a nifty little PCMCIA card. It does 802.11b, GSM SMS, GSM Modem and GPRS. It was a pain to set up and is a bit funky because the drivers run deeper than your user login so you get asked for the PIN before you log in and sometimes have trouble shutting it down, but it is generally OK.

I also have a Sony-Ericsson T68i which should do bluetooth with my Viao, but I couldn't get the settings on the unit set up correctly either in Austria or Spain. The bluetooth interface program on the C1MRX Viao called "blue space" also sucks. It looks nice, but I have NO IDEA what is going on with all the little sounds and icons. If you want to see an example of a completely "I thought cool design meant cool user experience" interface, buy a Viao and try to get bluetooth working.

I have a Siemens MT50 from Austria and a Seimens S45 from Spain. They both work fine in WAP GPRS mode with their original SIM cards in them. In fact, the Austrian one even roams properly in Spain. It is just impossible for me to figure out how to get the settings OUT OF these little things and into my computer. Also, I have yet to find any way to connect them to a computer other than IR or serial. Unfortunately, my Viao has neither.

I have a Swisscom SIM that Zai got me that I couldn't figure out how to get support for. I have a T-Mobile Austrian SIM which Thomas got me. It seems to have great roaming rates and the phone is content to roam automatically, but the support people had no idea how to get the thing working in another device.

I have a Vodafone Spain SIM Eva/Martin got me and came inside of the Siemens S45. Other than the fact that the only English speaking support person goes on Siesta on Saturdays and for some reason didn't get my id/password registered properly, she was the most knowledgable support person I talked to. It was the only SIM card that ended up working, but maybe that's because I'm in Spain...

You must also beware of phones that are locked in to a specific network. You need to buy one that is open if you want to move sim chips around different phones. My Austrian Siemens phone was open, the Spanish Vodafone Siemens seems closed and the Sony-Ericsson is supposed to be open...

So, blow by blow, here is what happens.

0) You turn on computer  
1) Nokia D211 asks for PIN (for your SIM card)  
2) Nokia D211 asks for Profile. (The Austrian T-Mobile support person tried to convince us that the name of the settings profile was relevant. Probably total bullshit.) Profile includes "GPRS ONLY" and settings including mainly the APN or Access Point Number. "airtelnet.es" in my case. (Extracted from Vodafone support)  
3) Log into Windows XP  
4) Nokia D211 says "Searching for Network" then "Ready for GPRS Activation"  
5) Go to (again, this is at least true in Spain) network connections and you will find that Nokia has installed a "GPRS" dialup settings entry. Go in there and change the "\*99#" to a "\*99\*\*\*1#" Also, if this is your first time, put in an id/password that you get from Vodafone support or from a friend.  
6) Turn off anything that conflicts with your serial port for your Nokia Card. (My blue space program hogs serial ports and conflicted, so "see you later blue space...")  
7) Open the Nokia D211 Manager program and click on Activate.  
8) The familiar dialup connection dialog box opens. Click dial. It should dial, log in, and you should be online.  
9) The manager program is very cool. It graphs GPRS strength and Data Rate.

I have found that Even with a GRPS Strength at 100% I can only get to a max of 30% of the data rate with an average data rate of less than 10kbits/s. So maybe it is the IP Network and not the GPRS network that is to blame...

Also, all of the settings that I talked about configuring in the computer have to be set in the AT commands on a phone that does the talking for you like the other Nokia phones. So, for instance, to set up a Nokia phone for talking on the Spanish Vodafone network, you would tell it something like:  
t+cgdcont=1,"IP","airtelnet.es","",00  
Also, you will have to set DNS manually, which is 212.73.32.3 and 212.73.32.67

Something like that... ;-p