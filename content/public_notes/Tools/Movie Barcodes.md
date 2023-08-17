---
title: Movie Barcodes
draft: false
tags: tools
date: 09 Aug 2023
date_created: 09 August 2023, 02:12
date_modified: 09 August 2023, 02:37
---
---

Recently I've been revisiting ["movie bar codes"](https://thefilmstage.com/movie-barcode-an-entire-feature-film-in-one-image/) like this one, from [Made by Machine](https://movingpixel.net/project/mbm/):

![[assets/made_by_machine_whole_barcode.jpg]]


These are images, in effect data visualisations, that render a whole film as a single image. The process to make them involves sampling frames from a video file, and stretching them as lines in chronological order to visualise the colour-time dynamics of the underlying moving images. The idea has been around for a while, and there are now on-demand printing services that sell you a poster of your favourite film bar code.

Movie bar codes can be created with relatively simple processing and manipulation of [[public_notes/Video as data|Video as data]], with no machine learning involved.  They are nice to look at but also tells something about the films, and I think they can be used as a pre or post processing technique in combination with other more advanced methods.

Here are some tools I've been using to make movie bar codes:

- [Movie Barcodes](https://timbennett.github.io/movie-barcodes/) --> back end: [FFMPEG](https://www.ffmpeg.org/) + [PIL](https://en.wikipedia.org/wiki/Python_Imaging_Library)
- [Movie Barcode](https://github.com/MarcBresson/movie-barcode/tree/main) --> wrapped as a Python library. Update: only runs on Python 3.10
- [movie-barcodes](https://github.com/andrewdcampbell/movie-barcodes) --> command line application, back end is [OpenCV](https://opencv.org/) and [numpy](https://numpy.org/)

I've been trying these out to make an image for the cover of my new book, [[public_notes/Cinema and Machine Vision|Cinema and Machine Vision]], possibly warped as as a circle, similar to [this example](https://rlang.io/create-a-radial-movie-tv-barcode-using-polar-coordinates/) (in R). The polar transformation seems rather onerous to implement directly in python (for me anyway), but a similar effect can be achieved using the polar filter in [GIMP](https://www.gimp.org/), or the ImageMagick's [polar distortion transformation](https://imagemagick.org/Usage/distorts/#polar). I intend to do a mini tutorial on this for my visualisation students, but here's a first preview:
![[cover_just_ring.png]]