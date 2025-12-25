---
title: "Microsoft Downplays Severe Internet Explorer Security Vulnerability"
date: 2002-08-14T00:00:00
permalink: https://joi.ito.com/weblog/2002/08/14/microsoft-downp.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2002/08/14/microsoft-downp.html
extracted: 2025-12-25
---

*First spotted on David Farber's IP List*
  
  
Microsoft's Internet Explorer has a vulerability in it's implementation of SSL. It allows anyone with a valid CA-signed certificate to generate a fake certificate for any domain. This is because MS IE does not check the "Basic Constraints" which should tell whether a CA has authority to verify another domain.
  
  
This is a significant vulnerability which would allow a "man-in-the-middle" attack without any dialog boxes. This means that someone could think they are accessing their bank or online shop securely and directly, but in fact be accessing through a hostile site. The hostile site could watch the transaction or modify the transaction without the user knowing it.
  
  
Aparently MS is downplaying it. The link below is a detailed report of the bug on BugTraq.
  
  
[SecurityFocus HOME Mailing List: BugTraq - Internet Explorer SSL Vulnerability 08/05/02](http://online.securityfocus.com/archive/1/286290/2002-08-08/2002-08-14/2)