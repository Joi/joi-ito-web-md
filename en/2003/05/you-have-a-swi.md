---
title: "You have a switch? SSH1? A wep key? Ha! You're not safe."
date: 2003-05-28T00:00:00
permalink: https://joi.ito.com/weblog/2003/05/28/you-have-a-swit.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2003/05/28/you-have-a-swit.html
extracted: 2025-12-25
---

![ettercap.gif](http://joi.ito.com/archives/images/ettercap.gif)  
When the WiFi network went down at FiRe and Max quickly mapped out the network, grabbed a free IP address and started hunting for the rogue network, it was useful and cool. I hadn't messed around with "security tools" recently so I decided to spend one hour searching for some tools that would work on my Mac.

First I downloaded trusty nmap which scans your network for computers, does an OS fingerprint and will often find the name, revealing the owner. It will also do quiet portscans to see what services are running on the machines.

Then I found [ettercap](http://ettercap.sourceforge.net/). (Lastest version doesn't run properly on the OS X, use version 0.6.7.) This is a full-featured packet sniffer with an easy to use interface. It is unique in that instead of doing IP sniffing, it uses ARP hacking and MAC address spoofing to allow you to sniff across switches. It has a variety of "plug-ins" that let you easily capture email, passwords and keyword filtered bits and pieces into files or onto the screen. It lets you insert your own text into connections so you could for instance type a command into someone's telnet session. Of course you can also terminate other people's sessions and connections. Another interesting feature in the recent release is that you can now sniff SSH1 sessions. (Lucky for Dan [we installed SSH2](http://weblog.siliconvalley.com/column/dangillmor/archives/001009.shtml#001009) on his computer.)
> ettercap README
>
> 5.4.4 SSH1 MAN-IN-THE-MIDDLE

When the connection starts (remember that we are the master-of-packets, all packets go through ettercap) we substitute the server public key with one generated on the fly and save it in a list so we can remember that this server has been poisoned before.

Then the client send the packet containing the session key ciphered with our key, so we are able to decipher it and sniff the real 3DES session key. Now we encrypt the packet with the correct server public key and forward it to the SSH daemon.

The connection is established normally, but we have the session key !! Now we can decrypt all the traffic and sit down watching the stream ! The connection will remain active even if we exit from ettercap, because ettercap doesn't proxy it (like dsniff). After the exchange of the keys, ettercap is only a spectator... ;)

I also googled around a bit and found a wep key cracker for WiFi wep keys and a password cracker for unix and windows passwords that all seemed easy enough to run.

My point is, an old fart like me with a some curiosity and an hours works was able to load up enough gear onto my Mac to do the basics. With a bit more time and skill, I could probably find the exploits so I could break into the computers I found on the network instead of just watching and messing with their connections.

If you want to feel safe using a WiFi network, AT LEAST use SSH2 port forwarding, [PGP](http://www.pgp.com/) and some security on your network like a [Sputnik](http://www.sputnik,.com/) with security turned on.