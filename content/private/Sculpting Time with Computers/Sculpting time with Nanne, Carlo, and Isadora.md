---
title: "Sculpting time with Nanne, Carlo, and Isadora"
date: 07 Jul 2023
draft: true
tags:
- example-tag
---
---

Nanne
Middle frame from each shot
Extract openclip features LAION 2B

Isadora 
Has been failing in interesting ways: tried to merge df with gender info and didn't work
CSV file gender info

Carlo
Shot scale detection
Cinescale.github.io --> cinescale detector
The anatomy of video editing paper
To the news reels


## 6 July

9:00-9:30 Coffee and introductions (plenum)
- Informal introductions over coffee

9:30-11:00 Perspectives on cinematic time (guided discussion)
- Introduction to the workshop
	- Me and Andrea
	- Announcements
		- Venue - health and safety measures, access, toilets, water fountain
		- Agenda - note evening event at the Nash
		- Contact points: embankment room extension and my number
	- The workshop
		- Overall purpose: towards aesthetically sensitive systems
		- Specific objectives: a prototype to analyse cinematic time computationally
		- Format: sprint-like design methodology that includes ideation, fast-iteration, and low-fidelity prototyping phases. Over two days, in small interdisciplinary working groups. Note: some people are not there for day 2
		- Introduction to the clusters - Note: different forms of expertise and contribution
	- Cinematic time - a definition and a prompt: debates in the study of cinematic time; what makes it difficult and interesting as phenomena to study
		- Challenges and opportunities (clusters) ― film, computational, collections, design
		- Discussion in plenum ― identify gaps of interest for ideation

11:00-11:15 Break

11:15-13:30 Ideation session 1: exploration (mixed group work)
- Introduce ideation exercise. Goal: produce ~50 ideas
- Styles of inquiry:
	- A world of objectkcs: technical,  engineering,  systematic, universal
	- A world of subjects: human, subjective, empathetic, diverse

> [. . .] from  the  perspective  of  a  systems  engineer,  is  the  'man-machine  interface'  ―  the  technical  specification  of  the  ways  in  which  a  user  will  observe,  control  or  feed  information  to  the  product.  A  second  mode  of  engagement  with  human  concerns  is  the  design  process  of  'requirements  capture',  where  a  complex  human  context  must  be  reduced  to  a  finite  set  of  defined  'features' that  should  be  implemented  in  the  eventual  product.
> 
> Excerpt from: [When Systemizers Meet Empathizers: Universalism and the Prosthetic Imagination](https://doi.org/10.1179/030801810X12772143410485)


## Worlds of subjects
### Emotions, functions, forms, and creative techniques

| Affect | Function | Form | (creative) Techniques | Notes |
|--------------|-----------|------------|------------|------------|
| nostalgia | represent memory | flash-back | hypodiegetic voice over/music | example: [Her (2013)](https://youtu.be/Ewq5tStHmdk) see: [Flashbacks in Film book](https://www.routledge.com/Flashbacks-in-Film-Memory--History/Turim/p/book/9781138974371)|


## Worlds of objects
### Data, features, tasks, and analytic techniques

| Data | Features | Tasks | (analytic) Techniques | Notes |
|--------------|-----------|------------|------------|------------|
| [short videos annotated with short descriptions](https://m-bain.github.io/webvid-dataset/) | visual and textual features | [text-to-video retrieval](https://meru.robots.ox.ac.uk/frozen-in-time/) | video and image joint encoder | from the paper [Frozen in Time](https://arxiv.org/abs/2104.00650) |

- Prompt 
	- in groups, write as many ideas for a system/tool you wish existed for the anlaysis of cinematic time: 20 ideas in 20 minutes (20x20).
	- Anything goes: we are not concerned with viability, specific technologies, data, etc.
	- Example 1 ― flashback detector: a system that detects flashbacks in films
	- Example 2 ― discontinuity editor: a tool for automatically re-editing films (edit-style transfer)
	- Example 3 ― an interface to see the parts of a film an audience has to imagine to make sense of the plot

13:30-15:00 Lunch

15:00-17:00 Ideation session 2: refinement (mixed group work)
- Introduce refinement exercise. Goal: refine to <5 ideas
- Prompt: all vote for the most stimulating ideas (reduce by half)
- Prompt: in groups, discuss promising ideas and try to break them down to the level of inputs and outputs, with an emphasis on where the inputs might come from, e.g. where can we find them or how can we produce them
- Each group refines to 1 idea.

17:00-18:00 Break (campus suggestions: Somerset House / Bush House terrace)

18:00-19:30 [High-dimensional cinema](https://kingsdh.net/2023/06/05/high-dimensional-cinema-6-july-2023/) (public event, Nash Lecture Theatre K2.31)

---

## 7 July

10:00-11:30 Prototyping session 1: paper (group work)
- Introduction to paper prototyping: configure ideas as inputs and outputs, break down processed in specific tasks and sub tasks
- Example: computational Burch 1 (2x2 matrix and manual annotations)

11:30-12:00 Break

12:00-13:30 Prototyping session 2: paper/Jupyter (group work)
- Identify existing libraries/tools/methods and if they need modification
- Implementation and testing
- Example: computational Burch 2 (shot-boundary detection and labelling task)

13:30-15:00 Lunch

15:00-16:30 Prototyping session 3: paper/Jupyter (group work)
- Running experiments at scale over a dataset

16:30-17:00 Break

17:00-18:00 Conclusions and prospects for future research (plenum)
- Debriefing and next steps.
