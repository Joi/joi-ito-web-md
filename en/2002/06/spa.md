---
title: "Spam"
date: 2002-06-28T00:00:00
permalink: https://joi.ito.com/weblog/2002/06/28/spam.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2002/06/28/spam.html
extracted: 2025-12-25
---

Spam is an issue that has been discussed and discussed. Laws have even been passed about it. The reason I decided to write something now about it is because I've been using a spam filter for awhile and I think it is working. Usually. I also think it represents the proper way of thinking about Spam.

Continue reading [Spam](https://joi.ito.com/weblog/2002/06/28/spam.html#more).

Sen and I have talked about spam a lot and we often talk about how it is yet another basic mistake in the way that the Internet was designed. If only smtp could let you authenticate the user before you received mail, we could make much better mail filter. Alas, this can not be changed now. (Or it would be very difficult.) So we have to come up with some solutions.

The best solution we have found so far is whitelisting. It is a way to make a filter that only lets mail from certain addresses through. Originally Sen had made a script for me where I had a separate mailbox for mail from people who were in my address book. Now we have moved over to [TMDA](http://software.libertine.org/tmda/) which lets you create white lists, black lists and a variety of other things. I have mine set up so that I can create and maintain my own list of addresses and domains that I want to receive mail from. We also have it set up so that if someone sends mail that is from someone not on the list, they get a message asking to reply and confirm that they are a human being. Once we receive the confirmation, the mail comes through. To filter for humans I don't want to get mail from or for that intelligent spam robot, I can make black lists.

There are still various problems with the system, but it works quite well. I still have it set up so that I have a mailbox for all of the mail that is rejected and I go through this periodically to make sure I did't miss something important.

In Japan, spam has become a huge issue because the recipient has to pay for the mail on i-mode phones. NTT Docomo is trying very hard to deal with this issue with filters of their own, but there are still major problems.

I do think that spam should be solved by certificates, authentication, keys, etc. on the user side and not by some huge central server...