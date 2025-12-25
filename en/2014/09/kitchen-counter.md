---
title: "Kitchen counter bio hacking"
date: 2014-09-01T00:00:00
permalink: https://joi.ito.com/weblog/2014/09/01/kitchen-counter.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2014/09/01/kitchen-counter.html
extracted: 2025-12-25
---

![](http://m.c.lnkd.licdn.com/mpr/mpr/p/8/005/07f/193/2c24306.jpg)

I first heard about [Synbiota](https://www.synbiota.com/welcome_page/welcome) at SXSWi this year, when they won an Accelerator Award. According to the announcement, "Synbiota is a virtual collaboration site that connects scientists, researchers, universities and others from around the world to solve complex problems using genetic engineering." That week they announced the world's first Massive Open Online Science (MOOS) event. Called [#ScienceHack](http://sciencehack.synbiota.com/), hundreds of researchers from around the globe (some as clueless as us!) would use a new "wetware" kit to produce prohibitively expensive medicine at a fraction of the price.

A month later I got this email:

> From: Connor Dickie  
> To: Joi Ito  
> Cc: Kim de Mora  
> Date: Apr 17, 2014, at 11:12  
> Subject: ML alumni wins SXSW prize for SynBio startup & Invitation to #ScienceHack
>
> "I'm writing to invite you to participate in [#ScienceHack](https://sciencehack.synbiota.com/), our distributed science effort to make real medicine for just a fraction of current costs using Synthetic Biology and the [Synbiota](https://synbiota.com/) platform. O'Reilly Radar recently called #ScienceHack [the most ambitious distributed science project](http://radar.oreilly.com/2014/04/distributed-science.html), and knowing your interest in biotech, I thought I'd reach out to you with a cool opportunity to learn with us.
>
> Participation is easy - I'll ship you one of our "Violacein Factory" wetware kits, and connect you with Kim de Mora at iGEM HQ (CC'd) who is not only interested to build one of the kits, but also has the required wet lab skills. It will take about an hour and a half for the in-silico design and build of the actual DNA part. Kim would handle the incubation etc. You would then come back to his lab in about 5 days to look at the results.
>
> We recently built a Violacein Factory kit here in [Canada](http://www.brittwray.com/2014/04/01/growing-violacein-factories-with-synbiota/), and more recently at [Genspace](http://www.genspace.org/blog/2014/04/10/sciencehack-violacien-factory-design-automation-with-opentrons/) in NYC, and everyone learned a bunch and helped us make significant advances towards our goal of an optimized violacein-producing organism.
>
> I'll be in Boston/Cambridge on the 27th-through-30th as part of a Canadian trade delegation, and will have some time to meet you and chat about the opportunity in person if it interests you.
>
> With regards,
>
> Connor Dickie  
> <http://alumni.media.mit.edu/~connord/>

I knew about [iGEM](http://igem.org/Main_Page). It was the spinout from MIT that brought high school and college students together to hack DNA much in the same way that robot competitions bring together kids interested in robots to hack and learn and compete. What's amazing is that iGEM, now bringing together over two thousand students at their Jamboree, takes the state of the art of synthetic biology and brings it to the masses.

Violacein is a natural purple compound made by *Chromobacterium violaceum*, a bacteria that is found in the soil in the tropics such as the Amazon. Violacein is created by the bacteria as a natural defense against amoebic creatures that try to eat it and is viewed as a potential anti-parasitic. It also appears to show promise as a treatment for cancer. The problem is that it currently costs $356,000 per gram because of the difficulty of harvesting it in the wild.

An opportunity to learn synthetic biology through doing it (my favorite way to learn) was too good to turn down so I immediately accepted the challenge. I started by taking the required safety courses for playing with recombinant DNA : General Biosafety for Researchers, check. Bloodborne Pathogens: Researchers, check. Hepatitis Information form, check. General Chemical Hygiene (web) and Managing Hazardous Waste (web). Check and check.

Then I started hunting for a place to do the actual work. That turned out to be a bit more of a challenge. Although the kit and process provided by Synbiota were basically safe and non-toxic, work with recombinant DNA and bacteria required a proper wet lab at MIT which are in short supply and used for more important things than the Media Lab director messing around with street bio.

After discussing with the team and looking at what we needed, we decided that my kitchen would be the least disruptive place to do the work.

On July 27, the Synbiota team and Kim from iGEM gathered at my house with a rag tag team of researchers from the Media Lab and elsewhere to work on the Violacein Factory #Sciencehack. We started with a briefing on what we were actually doing.

Our mission was to be one of the hundreds of teams participating in trying to innovate on developing the most effective method of synthesizing Violacein using synthetic biology.

Scientists have determined the metabolic pathway in *Chromobacterium violaceum* that converts tryptophan, a common amino acid, into violacein. This pathway involves five enzymes and various genetic sequences for their production. These "parts" of genetic code can be positioned differently in the DNA molecule and each combination has different attributes and tradeoffs - the optimal sequence and combination being currently unknown.

[![Synbiota kit parts](https://farm4.staticflickr.com/3897/14522997009_e1f6a9b500_c.jpg)](https://www.flickr.com/photos/joi/14522997009/ "Synbiota kit parts")

The #ScienceHack Violacein Factory Kit co-designed with [Genomikon](http://www.genomikon.ca/) which develops synthetic biology kits, had vials of all of the various genetic "parts" and the other materials needed to assemble these parts into a plasmid. According to Synbiota:

> This Kit includes everything you need except:
>
> • pipettes, nitrile gloves, petri dishes, PCR tubes, lab coats (for the full biotech experience, but any ol' trench coat will do!)  
> • ice buckets and ice  
> • 42 C water bath with epi tube floaty blanket  
> • 37 C incubator  
>   
> All the above can be found around the house, from online suppliers, at your local university lab store, or in a friendly scientist's stash.

Kim from iGEM brought everything from the iGEM lab. He walked us through the kitchen version of the protocol for using all of the equipment safely.

Synbiota, in addition to putting together this amazing #ScienceHack project has developed a suite of online tools to publish and share lab books online (I guess I don't need that fancy paper notebook I bought!), design DNA using a very nice graphical interface and provide researchers with a whole suite of tools to do synthetic biology as a community. Everything was very well designed and worked well.

First, I created an account on the Synbiota website and logged into [our notebook](https://www.synbiota.com/projects/610/workspace_pages/). Justin explained the [violacein pathway](https://www.synbiota.com/workspace_page_attachments/4872) and explained how we can use the online gene editor, GENtle3, ([video](https://www.youtube.com/watch?v=EZRtrtwPVI8)) to design the gene sequence online.

In GENtle3, we were able to drag and drop any of the genetic parts that came in the kit into our sequence and as long as we [followed the basic rules of which parts could be connected to each other](https://www.synbiota.com/projects/610/workspace_pages/12990). The sequence I designed was [Anc-ABEDDDC-Cap](https://www.synbiota.com/launch_gentle3/610/2474), where A, B, C, D, E represent the enzymes that make up the violacein metabolic pathway. (Visit the sequence tab in the Sciencehack project to view this and other designed sequences.)

The sequence had to start with the [Anchor--Origin-X'](https://www.synbiota.com/launch_gentle3/610/2443) part because that was the part that was attached to the magnetic bead. One of the keys to being able to do all of this amazing work in a kitchen had to do with this innovation.

In the kit were tiny sub-micron magnetic beads with the anchor part - a strand of DNA attached to it. What this meant is that we could use a small but very strong external magnet held to the side of the container - the epi tube - to pull all of the genetic material we were working with to the side of the epi tube allowing us to insert and extract liquids from the container using pipettes while leaving our working material secured to the container.

What we needed to do after designing our sequence was to assemble it. We did this putting the beads in a epi tube, adding a "wash", removing the wash, adding a genetic part from a color coded tube that corresponded with the next link in our design, adding the T4 DNA ligase, the "genetic glue" to attach that new part to the strand on the bead, removing the excess material, washing again, and then repeating until we had added each part in order to the bead. Theoretically, we should now have a long strands of DNA attached to each bead representing our version of the DNA sequence (plasmid) that we designed.

The last step was to use a buffer to remove the bead from the strands and we had a little drop of genetic material that when inserted into a living bacteria should create all of the enzymes necessary to produce violacein from tryptophan.

The next step was what was called "transformation" which is the process that takes our plasmid and inserts it into a bacteria, in our case*E. coli.* The "competent" *E. coli* designed for easier transfection were created at iGEM. The process we used for transformation was called "heat shock" which involved adding our genetic material to a salt solution with the *E. coli* and then rapidly heating it which caused the genetic material to be absorbed into the *E. coli*. The device used for heating, I noticed, had a sticker from the "MIT Property Equipment Office" on it. Definitely a bit punk rock. After the "shock" we added liquid material with nutrients and minerals that "rebooted" the *E. coli*, waking it up and preparing it to be incubated for execution of the DNA code we just inserted.

The *E. coli* were then spread onto petri dishes with Jello-like "food" as well as an antibiotic, chloramphenicol. The chloramphenicol would kill all other bacteria on the dish except our own because we had cleverly included a chloramphenicol resistance building genetic part in our sequence.

[![Heat shocker](https://farm3.staticflickr.com/2903/14523010398_ef70839040_c.jpg)](https://www.flickr.com/photos/joi/14523010398/ "Heat shocker")

We then sent the petri dishes back to iGEM for incubation. The results were not perfect, but none-the-less, it looks like violacein and other molecules from the pathway were created (some other got different colours). The images of my petri dish show a kind of blackish zig-zag smear which are billions of bacteria producing metabolites because the executed DNA I designed and created. At this point I don't know for sure whether violacein was created - I need to do more verification and experimentation, but for a first go at building a complex metabolic pathway, not too shabby. Something else that is cool, is that my intended DNA design was very long, 12,000 base pairs, the next #ScienceHack step is to verify that the entire code I designed was actually assembled properly. We shared our designs, protocols and procedures with the rest of the teams. The next step was to look at the work of the other teams and try to find out what we could improve and try again.

In two half days of work, we were able to do in our kitchen what would have been Nobel Prize winning work a decade ago. We designed a sequence of genes, actually assembled the genes and then injected them into a bacteria and rebooted the bacteria.

Also, unlike traditional labs where one team would do the work and publish a paper and then other teams would try to replicate the work, we worked as one large team of parallel labs sharing our work as we went along, iterating, innovating and discussing.

I think that there is a good chance that one of the hundreds of teams will discover an efficient way of synthesizing, extracting, and purifying violacein and that soon we will have something that will probably initially look something like a homebrew beer brewing contraption producing the extremely rare compound for researchers with instructions on how anyone can build one of these violacein factories.

--

Disclosure : After this experience, I was so excited that I donated to iGEM and decided to invest in Synbiota.