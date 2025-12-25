---
title: "My letter to the governor of Nagano about his security audit"
date: 2003-12-19T00:00:00
permalink: https://joi.ito.com/weblog/2003/12/19/my-letter-to-th.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2003/12/19/my-letter-to-th.html
extracted: 2025-12-25
---

The governor of Nagano ordered an security audit of their network with a focus on the Basic Residents Registry system of the central government. I was asked to take a look at the audit and provide a 3rd party opinion. Since I am on the central government panel working on the security of the Basic Residents Registry, my letter has become a bit controversial and apparently my phone is ringing off the hook right now in Tokyo. Lucky for me I'm in the US...

I'm not looking forward to returning to Tokyo.

The central government denies security problems and I am going to have to deal with this when I return to Tokyo...

The audit is not yet completed and my audit of the audit is an opinion based on incomplete information. I will be meeting with both sides when I return to Tokyo and will probably be required to write another opinion after the final results of the audit have been submitted and I have heard the arguments from the central government.

[Mainichi reports some of this in English](<br />
http://mdn.mainichi.co.jp/news/archive/200312/16/20031216p2a00m0dm004000c.html)

Here's the letter.

> December 11, 2003
> Governor Yasuo Tanaka
>
> Dear Governor Tanaka:
>
> I have reviewed in detail the security audit that your outside auditors conducted on three towns in Nagano. I reviewed their process, data and analysis. I also interviewed the key members of the team for several hours and discussed their methodology and conclusions.
>
> Generally speaking, the security level at the sites was below average and a variety of personal information about your citizens is at risk of being stolen and modified.
>
> The team conducted audits from the Internet and from inside the local government offices. The team was given very limited time to conduct their audits. The penetration test from the Internet was not successful. The tests from inside the government offices were quite successful. The audit was limited to computers inside the local government offices, so the Jyukinet was not attacked directly. However, the computer that connects directly to Jyukinet, the “CS server” and the “Reams server” which is inside the local government network both have databases of the Jyukinet data of the citizens living in the city. Both of these servers were vulnerable and the audit team was able to take control of them. This would theoretically allow them to edit, delete and create new citizen records. It was not tested, but it is likely that editing this database would cause these false records to be sent to the central Jyukinet system.
>
> In addition, there were numerous files containing sensitive personal information unrelated to Jyukinet accessible on the local government network with no protection.
>
> Although it was not possible to penetrate the local government network from the Internet, there were dialup accounts for remote offices that allowed users to connect to the local government’s network. It is possible that these dialup accounts could be exploited to allow someone to dial into the network. In addition, the library in one city was directly connected to the network. As anyone can use the library’s machines or connect their computer to the network, anyone can download the sensitive files being “shared” on the machines without any “hacker skills”.
>
> Breaking into the CS Server and the Reams server, which contained Jyukinet data for the local citizens, was quite easy. They were running systems that had not been properly updated with security patches. The passwords were very obvious on the system as well as on the database and were quickly cracked. The software running on the server was written with “buffer overflow” vulnerabilities that show a lack of understanding of security by the developer of the code. I recommend a third party security audit of the software running on these systems. A computer engineer using freely available tools would be able to exploit any of these vulnerabilities to gain access to the Jyukinet data.
>
> In summary, I believe that the security level of the networks were below average and any average computer network engineer could break into and steal or damage a variety of personal information including Jyukinet information. The people working in the office and in particular, the vendors providing the system security are not sensitive to security and privacy issues. The servers have not been maintained properly and the selection of passwords (many had default passwords or easily guessable passwords) was irresponsible and showed a complete lack of attention to security. I strongly urge that the priority on security for privacy purposes be increased significantly, both in local government offices and vendors providing solutions to these local governments. I believe that the citizens and the people responsible for protecting their information are significantly at risk.
>
> Best regards,  
> Joichi Ito