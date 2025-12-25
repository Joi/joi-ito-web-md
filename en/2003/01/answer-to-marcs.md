---
title: "Answer to Marc's question about how our moblog works"
date: 2003-01-09T00:00:00
permalink: https://joi.ito.com/weblog/2003/01/09/answer-to-marcs.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2003/01/09/answer-to-marcs.html
extracted: 2025-12-25
---

> [Marc Canter](http://blogs.it/0100198/2003/01/08.html#a499)
>
> I'd like to ask Joi to tell us all, how his moblogging implementation works. What is the mechanism of getting that photo from the phone, to the PC and then into a blog. I know you use Moveable Type. Do you send the photo as an email attachment or some other form? Do you completely bipass the 'mobile carriers' or simply pay for he usage/bandwidth time? If your scenario is other than email, then what routing, access or commercial gateways do you have to navigate through - to get data onto the net?

We use email. Email is received and processed by a Python script. The script stores the attached jpg image in a directory and renames it with a unique name. It then posts the entry to MT using the MetaWeblog API to create an entry with the subject of the email as the title and puts the body of the email and an img src link to the jpg in the entry wrapped in div tags. Pretty simple. It would be easier if someone added more image handling in the API. Take a look at the [Python script](http://radio.weblogs.com/0114939/outlines/December 25, 2002 - Neoteny Blogging Team mail2entry (attached image mail to MT tool) script released to publicDecember 25, 2002 - Neoteny Blogging Team mail2entry (attached image mail to MT tool) script released to publichttp://joi.ito.com/archives/200) for more details.

We pay the carrier for the transmission of the email. Wish it were flat fee, but it's by the packet. Need to find a less "intelligent" network.