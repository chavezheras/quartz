---
title: Creanalytics
draft: true
tags: 
date_created: 25 Sep 2023
date_modified: 25 Sep 2023
margin: 0
width: 1920
height: 1200
transition: slide
theme: moon
---


# Creanalytics
### _Between Data Analysis and Media Synthesis_

Dr Daniel Chávez Heras

![[assets/images/db3a81949ab652d55054d76b287e03fa_MD5.jpg|250]]

[@chavezheras@sigmoid.social](https://sigmoid.social/@chavezheras)

[movingpixel.net](https://movingpixel.net/)

note: Thank you for the invitation, delighted to be here.

---

![[assets/images/creanalytics_cover.png]]

note:

Recent paper of the same name
I will go over one of the examples of paper to illustrate the idea and main argument behind creanalytics

---


# Archives and Datasets

![[assets/images/4e8d25b2f1c29232da6e892367c5ef79_MD5.jpg]]

note: 
Archives for humans to keep and explore
Datasets for machines to process and produce

Archives are created under a historical impulse; they are organised according to the record-keeping needs of the cultures that build them. This historical impulse requires a high degree of structuring, usually in the form of hierarchical ontologies that facilitate cataloguing and retrieval, and that aspire to a certain degree of historical accuracy, integrity, and permanence.

Datasets also respond to the sense-making needs of the cultures that build them however they come together under a different impulse; they tend to be contingent assemblages, made in response to specific a priori needs and questions relevant to engineering and the sciences.
In data science and machine learning engineering, datasets tend to be granular, flattened to matrix-like structures whose individual items are not meant to be publicly accessible or even individually meaningful to human observers.
 
Contemporary AI has succeeded in part for not caring at all about whether specific media artefacts are deemed significant enough by human critics to go ‘on the record’.

Archives and datasets produce value in almost opposite ways: while archives endow their constituent artefacts and records with additional symbolic layers, making them stable and tractable, datasets that feed contemporary AI systems atomise these artefacts, stripping them from context in order to make patterns visible through computational processing. In the first case value is produced by stability and addressability, in the second by aggregation and mutability.

Image by Erik Desmazières

---

# Moving Image Archives and Datasets

note:

Film archives, understood here as organised collections of individual films and other moving images, with records that include directors, years, countries of origin, performers, producers, etc. 

However, each of these films can also be thought of as a collection of frames and a dataset of images. And through computing, these individual frames can relate much more freely, not only to other frames in the same film, but to a multitude of other frames in a multitude of other films. 

Film archives can be thought in this way as potential collections of datasets, or more precisely, large latent datasets themselves.

---
# Levels of analysis


| Artefact     | Processing level       | Example                                                     |
|--------------|------------------------|-------------------------------------------------------------|
| Cinema       | Social – aggregate     | Popular Hollywood cinema                                    |
| Film         | Human                  | Jurassic Park (1993)                                        |
| Clip         | Human/computer         | Raptors in the Kitchen Scene (https://youtu.be/dnRxQ3dcaQk) |
| Shot         | Human-computer         | 130 frames (5.421 s)                                        |
| Frame        | Computer/human         | Individual frame (512 × 340 pixels)                         |
| Pixels       | Numeric – disaggregate | Vector ([176800x1]); Tensor ([16, 3, 340, 512])             |


---


# Creanalytics
## Analysis through creative generation

note:

Analytic and generative approaches in computing tend to be split between scientific and creative domains, with their respective tools and communities of practice.

Deployed as analytical engines, computers can be used to find patterns across vast collections of imagery, and these patterns are often expressed as relations of proximity in space. 

But to amount to knowledge, these spatial correlations require interpretation and explanation, which unfold sequentially, as critics seek to organise these patterns to infer causal relations and temporal representations between data objects and events. By coupling an analytical engine with a generative one, computing can be used to configure narratives about these proximity patterns and enable explanatory propositions through compositional techniques familiar to media scholarship.

---

# Supercuts
## Data sampling through film editing

---

>Over the past century, we have come to think of nearly every aspect of our lives as composed of data. The supercut is part of this; indeed, every time we use a search engine, we commission a computer to make us something quite like a supercut. Thus, the supercut entails not simply a mode of editing, but a mode of thinking expressed by a mode of editing. […] Just as capitalism treated workers as machines as a prelude to workers being replaced by machines, so also supercutters simulate database thinking in apparent anticipation of a moment, perhaps in the near future, when neural networks will be able to search the entirety of digitized film history and create supercuts themselves, automatically.

\- Max Tohline, 2021

---

>In the near future there will be a simple software or app, feeding its algorithm with keywords and other elements of interest, which will automatically generate a perfect supercut of media content of any kind within a blink of an eye.

\- Miklós Kiss, 2013

---

## Movie Clips YouTube channel
 ![[assets/images/e3ee5592f9728d7d204e90a475a2a42f_MD5.jpg]]

note: 
An archive-like collection that is publicly available online: the _Movieclips_ YouTube channel ([2006](https://journals.sagepub.com/doi/full/10.1177/13548565231174592#bibr29-13548565231174592)), which serves as a corpus that is both large and consistent enough to be analysed and intervened using computational methods. 

This channel is operated by the American media company _Fandango_, which owns the popular review aggregator website _Rotten Tomatoes_, and the recommender platform _Flixter_, and which is itself jointly owned by the Warner and Universal media conglomerates. 

In their YouTube channel _Movieclips_ is described as ‘the largest collection of licensed movie clips on the web’. At the time of writing, it had over 58 million subscribers and almost 60 billion aggregated views. 

In terms of sheer size and exposure, these numbers dwarf most film archives, but it is important to note that in terms of breadth and diversity, these movie clips are only one deep but thin slice of global film production, namely, recent Hollywood popular cinema licenced by these large media companies.

---

## Movie Clips Corpus

- 2691 clips 
- 350 films
- From 1931 to 2019
- 287 unique directors


---

### Pre-trained FER detection 

![[assets/images/ladybird_FER_1.jpeg]]

---

### Shot scale detector

![[assets/images/schot_scale_detector.jpg]]


---

# Feature Engineering

|Feature|Value|
|:----|:----|
|People|1|
|Scale|23.2|
|Inferred motion|0.24|
|Scale category|‘CU’|
|Inferred motion category|‘Stable’|
|Top emotion|‘Angry’|
|Top emotion confidence|0.79|

---

### Shot duration distribution

![[assets/images/shot_histogram.jpeg]]


---


### Shot scale breakdown

![[assets/images/shot_scale_chart.jpeg]]

---

### Shot emotion breakdown

![[assets/images/shot_emotion_chart.jpeg]]


---

<iframe src="https://player.vimeo.com/video/602000956?h=71ac4fdc22" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/602000956">Big Angry Faces v.01</a> from <a href="https://vimeo.com/chavezheras">Daniel Ch&aacute;vez Heras</a> on <a href="https://vimeo.com">Vimeo</a>.</p>

---

![[assets/images/computational_supercuts.png]]

---

