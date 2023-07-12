---
title: "day two"
date: 10 Jul 2023
draft: true
tags:
- STC workshop
---
---

On day two we gathered again to decide what ideas we could put to the test and fast prototype. We examined two datasets: [[private/Sculpting Time with Computers/Mila Oiva|Mila Oiva's]] soviet newsreels and this publicly available sample from [BBC Archives](https://archive-downloader.bbcrewind.co.uk/). In the end we decided to focus on the news reels, which have richer metadata, and test two methods that map to our discussions of [[private/Sculpting Time with Computers/historical time|historical time]] and meaningful objects, and [[private/Sculpting Time with Computers/cinematic time|cinematic time]] and fast/slow editing:

- [Open clip](https://github.com/mlfoundations/open_clip) --> an open source implementation of CLIP pretrained on the LAION 2B dataset. The basic idea behind CLIP is to have text and images in a shared representational space so that we can calculate the distance between them.

- [Cinescale](https://cinescale.github.io/) --> a shot scale classification model trained on a set of manually annotated frames from 124 films. The goal is to classify different shots by their scale: close-up, medium shot, long shot, etc. In [[public_notes/Creanalytics|this paper]] I tried shot classification without annotations using face detection, but that approach is of course limited to faces, whereas this can pick up close-ups of objects for example.

We know these techniques have limitations, as explored during [[day one]] of the workshop. However, we also think that combined, these methods complement each other and can be useful for the analysis of temporal dynamics in large collections of moving images. Testing this combination against the newsreel data set is helpful because thanks to [[private/Sculpting Time with Computers/Mila Oiva|Mila's]] sustained work on these reels we know something about their local as well as global structures so we can apply methods to the collection of moving images, and at the same time use what we know about this collection to evaluate the methods.

During the [[panel on high-dimensional cinema]], I referred to this as working towards "aesthetically sensitive systems", and in our discussion the day after [[private/Sculpting Time with Computers/Nanne van Noord|Nanne van Noord]] suggested "aesthetically sensitive retrieval" as an applied version of this idea. We wrapped up the day with some [[ideas and next steps]] along these lines.

