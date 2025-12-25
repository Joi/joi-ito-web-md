---
title: "Technology, Security and Cyber Arbitration"
date: 1999-02-04T00:00:00
permalink: https://joi.ito.com/weblog/1999/02/04/technology-secu.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/1999/02/04/technology-secu.html
extracted: 2025-12-25
---

An article I prepared for the Inter-Pacific Bar Association about Cyber Arbitration.
**For the [Inter-Pacific Bar Association](http://www.ipba.org/) Newsletter

February 4, 1999

by Joichi Ito

*Technology, Security and Cyber Arbitration***

As the technical advisor for the Cyber Arbitration program
held at the IPBA annual conference in Auckland last year and for the Cyber Arbitration
program to be held at the IPBA annual conference in Bangkok this year, I am
responsible for providing assistance and advice regarding the technical requirements
of the Cyber Arbitration programs and providing guidance as to what the future
will hold for Cyber Arbitration. In this article, I would like to discuss the
technology used at the Auckland program, future technical possibilities, and
various security concerns related to Cyber Arbitration.

**Auckland Cyber Arbitration Demonstration**

At the IPBA annual conference in New Zealand, we conducted
the Cyber Arbitration demonstration using PictureTel video conferencing technology,
which is widely used internationally. PictureTel has many configurations with
various quality levels. We chose to use the 128K system, which is equivalent
to two ISDN channels, because ISDN is either deployed or is being deployed in
most countries and is the most common transmission speed used for video conferencing
today. The purpose of using such technology was to give a true-to-life example
of what a Cyber Arbitration might look like using widely available technology.
Because a videoconferencing bridge was used to allow split screen multi-point
video conferencing this also caused an inevitable delay in sound and picture
transmission since the bridge has to decode everyone's video signals and create
a multi-screen signal to send to each participant.

**Cyber Arbitration and the Internet**

Although the Auckland Cyber Arbitration demonstration showed
that an arbitration using multipoint videoconferencing technology was feasible
even given the low-level of current widely available technology (and, per force,
will be much more feasible with the rapid advance of the general level of technology),
one of the critical issues highlighted by the demonstration was cost. ISDN,
telephone and leased lines offer dedicated circuits which allow high quality
communications, but the cost of creating a network of high speed ISDN connection
worldwide for several hours can become prohibitive.

This is where the Internet comes in. The Internet promises
to lower the cost of communications by allowing multiple users to share circuits,
making communications much more efficient, thus lowering the cost. Nevertheless,
at present, one of the primary problems with trying to conduct video conferencing
over the Internet is that the Internet is what is called "best effort" connectivity.
On the Internet, one traditionally does not have a dedicated circuit, but instead,
shares the circuit with everyone else who happens to have their routes going
over the same lines. When any segment of the chain of routers, leased lines
or servers that one would go through to reach each other gets crowded, the connectivity
slows down and video frames freeze up and audio starts to cut out. This sort
of "lossy" video is now quite common on the Internet, but is used primarily
for non-critical or entertainment applications. It is absolutely inadequate
for the requirements of a real Cyber Arbitration, and is why we were unable
to demonstrate a Cyber Arbitration using the internet in Auckland.

Nevertheless, high quality video transmission and video conferencing
is currently being tested around the world. Using high speed lines with special
routing technology, Internet service providers will be able to guarantee bandwidth
to users requiring high quality and high speed lines. Applications are being
developed to allow personal computers and hardware from many vendors to communicate
using open standards, thus lowering the price of video conferencing equipment.
It is likely that, over the next several years, it will be quite common to find
video conferences being conducted over the Internet at quality levels equivalent
to, if not superior to the quality currently being achieved using 128K ISDN
and PictureTel. Until such time, however, it will still be of benefit to use
the infrastructure and technology available to us today to work out many of
the legal and procedural issues that we can identify only through actually conducting
Cyber Arbitrations.

**The Internet and Security**

One of the primary concerns in the age of open networks is
security. E-mail and other internet communications (such as the types that would
be necessary to conduct Cyber Arbitrations) are typically transferred through
several servers and travel over open networks. It is a trivial matter for even
a minimally computer-literate individual to, for example, intercept and even
replace e-mail while it is traveling between a lawyer and his client. In the
age of advanced digital technology, wiretaps are not conducted by people "listening"
to phone calls, they are conducted by voice recognition software which can scan
thousands of connections or scan stored conversations in databases. E-mail is
searched by keyword or intelligent pattern matching software that can search
through and organize billions of pages easily. Not surprisingly, therefore,
thousands of computers which serve mail are penetrated each year and corporate
espionage on computer networks has become a growing concern and a real threat.

This is why cryptography and digital signatures are essential
to ensure the integrity of a Cyber Arbitration system. Digital signatures using
public key cryptography are becoming more and more widely used. Digital signatures
allow e-mail or any other form of electronic message to be digitally signed
by the sender and for that signature to be verified by the recipient. Digital
signatures are typically authenticated by a certification authority ("CA").
The CA uses some method of identification verification and then certifies the
key which is used to sign documents.

Using public key cryptography, documents can also be encoded
in a way that allows only the holder of a particular key to decode and view
the document. Public key cryptography is unique in comparison to other forms
of cryptography in that the key used to encode (encrypt) the document is different
from the key used to decode (decrypt) the document. The key used to encrypt
the document is referred to as the public key and the key used to decode the
document is referred to as the secret key. By distributing one’s public key widely,
anyone who receives the public key can then send confidential encrypted documents
to the holder of the secret key without fear of the un-encrypted (plaintext)
data falling into the hands of unauthorized viewers.

In combination with digital signatures which use the same public
and secret keys as public key encryption technology, public key technology allows
people to conduct private and authenticated communications over the internet.
It also allows the creation of tamperproof documents and allows electronic documents
to be presented "in writing" which can not be modified without breaking the
digital signature associated with the document.

The risk that a public key that you believe belongs to a trusted
colleague is not actually the correct key is supposed to be managed by the CA.
The problem with the CA is whether one can trust the CA. Companies running CA's
are not infallible and possibly more importantly, they are overseen by government
agencies which may be incentivized to allow forgeries or deception to occur
in order to collect information about unfriendly governments, organizations
or individuals.

A CA managed by the IPBA with an identification verification
procedure which is open, capable of being audited, and conducted face to face
at the IPBA’s annual meetings could easily become one of the few trusted forms
for authentication of keys. Such an authentication mechanism could be used not
only to ensure the integrity and confidentiality of Cyber Arbitrations, but
also could be used to manage membership, standardize document execution, store
and date evidence, conduct encrypted telephone and video conferencing, and a
myriad of other applications.

**Conclusion**

New technology will allow international arbitration and negotiation
to become faster, more efficient and less expensive. Although procedures and
law will have to be developed and modified as technology develops, many of the
issues (including security issues) will only become apparent as these new technologies
are deployed and tested by real lawyers and arbitrators. This is why continued
research and development of a Cyber Arbitration system by the IPBA is so important
to ensuring a bright and new technological future for international arbitrations.
The IPBA is in a unique position to create a testbed for developing a workable
Cyber Arbitration system and should not let this opportunity slip from its grasp.

*By Joichi Ito*

---

Bibliography

1. Nobuo Miyake, Esq., *The Future is Now: The IPBA and Cyber Arbitration*,
   IPBA Journal, September 1998, pp. 16-18
2. David F. Day, Esq, *Conducting the Electronic Arbitration*, IPBA Journal,
   September 1998, pp. 19-20
3. Jasna Arsic, *International Commercial Arbitration on the Internet*,
   Journal of International Arbitration, pp. 209-231

---

Release Notes

1. Draft Version 1by Joichi Ito February 3, 1999
2. Edited by Joseph Gourneau February 4, 1999 for submission to IPBA
3. Edited by Joichi Ito February 16, 1999 for web publication (In particular,
   modified the 128K = ISDN edit by jg and re-included the bibliography)

---

Copyright 1999, Joichi Ito