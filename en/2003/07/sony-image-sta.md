---
title: "Sony Image Station with MetaWeblog API"
date: 2003-07-05T00:00:00
permalink: https://joi.ito.com/weblog/2003/07/05/sony-image-stat.html
language: en
categories: []
author: Joichi Ito
source_path: /weblog/2003/07/05/sony-image-stat.html
extracted: 2025-12-25
---

Hirata just demo'ed an experiment we did with Sony. It's a moblog gateway. It receives email from a cell phone with a photo attached. The Sony team made an XML RPC metaWeblog API interface to Sony Image Station. We take the picture, talk to Sony Image Station using metaWeblog API and post the picture in a photo album. Then the gateway talks to Movable Type using the metaWeblog API to create an entry with the thumbnail from Image Station that clicks thru to the full picture on the Image Station site. The text and the title get entered into Movable Type and the category is pre-set. We are using the metaWeblog.newMediaObject (which Movable Type current supports) to send the images. **Please support this standard so photo sites can use the API.**

We'll continue doing tests with the research group and hope to do some syndication stuff soon. ;-) This is not a product and is really just an experiment. I'm hoping more and more groups in Sony start looking at the open standards and that the open standards people start thinking photos, video and audio as micro-content. Totsuka-san from Sony CSL Content and Applications Lab (sorry about the mistake Totsuka-san!) had an interesting comment today. He said that pictures are attached to email as second class citizens and the text is still the core of the data. I think the idea is to try to get multi-media micro-content to be more important. ;-)

PS I don't have a URL for this since we have only received an OK to demo it at the conference. Stay tuned.