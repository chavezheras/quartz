---
title: "Videogrep"
date: 16 May 2023
draft: true
tags:
- supercut
- montage
- tool
- words and images
---
---

>Videogrep is a command line tool that searches through dialog in video files and makes supercuts based on what it finds. It will recognize .srt or .vtt subtitle tracks, or transcriptions that can be generated with vosk, pocketsphinx, and other tools.

Sam posted an implementation of Videogrep that runs on Colab, which made me think of running this on a Jupyter Lab instance from our College's computer cluster, and then possibly using it for teaching. The college does not host its own notebook instance, as far as I know, but the cluster can serve a headless Jupyter that can be "tunnelled in" through ssh.

Here's the [repository](https://github.com/antiboredom/videogrep).

And here's the [Colab minimal example](https://t.co/QGKTLxOZ52).

Here are other examples from Sam's repo:

-   [silence extraction](https://github.com/antiboredom/videogrep/blob/master/examples/only_silence.py)
-   [automatically creating supercuts](https://github.com/antiboredom/videogrep/blob/master/examples/auto_supercut.py)
-   [creating supercuts based on youtube searches](https://github.com/antiboredom/videogrep/blob/master/examples/auto_youtube.py)
-   [creating supercuts from specific parts of speech](https://github.com/antiboredom/videogrep/blob/master/examples/parts_of_speech.py)
-   [creating supercuts from spacy pattern matching](https://github.com/antiboredom/videogrep/blob/master/examples/pattern_matcher.py)