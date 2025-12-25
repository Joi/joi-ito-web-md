---
title: "My email not good enough for you?"
date: 2007-08-02T00:00:00
permalink: https://joi.ito.com/weblog/2007/08/02/my-email-not-go.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2007/08/02/my-email-not-go.html
extracted: 2025-12-25
---

I think it's because a lot of spam comes from Asian domains and IP addresses, but more and more ISPs and companies are banning email from addresses in Asia. I now get at least a few of these a day:
> : host smtp1.\*\*\*.com[xx.xx.xx.xx] said: 550  
> Rejected: No spam wanted here. Your email was deemed to be spam and is not  
> accepted. Send a message to postmaster@\*\*\*.com if you feel this  
> rejection is in error. (in reply to end of DATA command)  
> Reporting-MTA: dns; 35.145.221.202.bf.2iij.net  
> X-Postfix-Queue-ID: 8880B67052  
> X-Postfix-Sender: rfc822; jito.\*\*\*.com  
> Arrival-Date: Thu, 2 Aug 2007 17:53:05 +0900 (JST)

I don't know exactly what you guys can do about it, but blocking regions seems a bit blunt and rude. The IP address I'm sending from is a pretty legitimate block of address owned by WIDE.

The reason I suspect that it is an Asian thing is that the usual response from the various "postmasters" is, "oh, it's because the email is from an Asian address."

Is there any way to get my IP address added to some white-list so this doesn't happen or will the physical proximity of my mail server always cause my IP address to be painted with the spam brush?

Although I suppose that's how it feels when blog comments get stuck in my spam queue. The only difference is that I look at those regularly and let them through. These spam rejection notices are basically 86 at the door deals.