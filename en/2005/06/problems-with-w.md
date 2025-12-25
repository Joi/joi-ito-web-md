---
title: "Problems with Wikipedia in my DNS"
date: 2005-06-12T00:00:00
permalink: https://joi.ito.com/weblog/2005/06/12/problems-with-w.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2005/06/12/problems-with-w.html
extracted: 2025-12-25
---

For the last several days, I haven't been able to access the English Wikipedia from home. This has happened in the past. The reason is that the DNS that my ISP provides me is returning an error when looking up en.wikipedia.org.
> dig en.wikipedia.org  
> ;; Truncated, retrying in TCP mode.  
> ;; communications error to 210.130.232.1#53: end of file

The odd thing is that jp.wikipedia.org and other Wikipedia subdomains resolve. Also, when I try another DNS server, en.wikipedia.org resolves. The DNS server I am using, DNS.CDN-JAPAN.COM (210.130.232.1) is run by IIJ, my ISP. Has anyone else had similar problems either with other domains on IIJ or problems with en.wikipedia.org on other DNS servers?

Sorry, for this obscure and geeky post, but being prevented from using Wikipedia has become extremely irritating.

UPDATE: en, fr, nl, de, pl fail. ja, eo, ko, es, zh work. It appears that the ones which are failing use geodns.

UPDATE 2: I caught up with a senior guy from my ISP IIJ at the Internet Association meeting yesterday and explained the problem to him. He said that MAYBE it is because they are running a load balancing thing that might interact weirdly with geodns. He's looking into it for me.

UPDATE 3: I got a response from my ISP. They said that the "AUTHORITYSECTION" was being returned making the record longer than 512 bytes forcing it to respond via TCP instead of UDP. They said that they thought my firewall was blocking TCP responses from dns. They changed the setting on the nameserver not to add the AUTHORITYSECTION and now it appears to work for me... I've asked them to provide me with another long domain entry greater than 512 bytes so I can see if I can replicate the error...

Technorati Tags: [wikipedia](http://technorati.com/tag/wikipedia)