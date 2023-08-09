---
title: Movie Barcodes
draft: false
tags: tools
date_created: 09 August 2023, 02:12
date_modified: 09 August 2023, 02:37
---
---

There are a few tools online to generate ["movie barcodes"](https://thefilmstage.com/movie-barcode-an-entire-feature-film-in-one-image/) like this one, from [Made by Machine](https://movingpixel.net/project/mbm/):

[[content/assets/13a8ca18e7b11309f5447486df8b5a74_MD5.jpg|Open: made_by_machine_whole_barcode 1.jpg]]
![[content/assets/13a8ca18e7b11309f5447486df8b5a74_MD5.jpg]]


The process variously involves sampling frames from a video file, and stretching them as lines in chronological order to visualise the colour-time dynamics of the underlying moving images. The idea has been around for a while, and there are now on-demand printing services that sell you a poster of your favourite film bar code.

This involves a relatively simple processing and manipulation of [[Video as data]], with no machine learning involved. Yet, it tells us something about the films, I think it can be used as a pre or post processing technique in combination with other methods.

- [Movie Barcodes](https://timbennett.github.io/movie-barcodes/) --> backend: [FFMPEG](https://www.ffmpeg.org/) + [PIL](https://en.wikipedia.org/wiki/Python_Imaging_Library)
- [Movie Barcode](https://github.com/MarcBresson/movie-barcode/tree/main) --> wrapped as a Python library
- [movie-barcodes](https://github.com/andrewdcampbell/movie-barcodes) --> command line application

I've been trying these out for the book cover of my book, possibly warped as as a circle, similar to [this example](https://rlang.io/create-a-radial-movie-tv-barcode-using-polar-coordinates/) (in R). The polar transformation seems rather onerous to implement directly in python (for me anyway), but a similar effect can be achieved using the polar filter in [GIMP](https://www.gimp.org/), or the ImageMagick's [polar distortion transformation](https://imagemagick.org/Usage/distorts/#polar).