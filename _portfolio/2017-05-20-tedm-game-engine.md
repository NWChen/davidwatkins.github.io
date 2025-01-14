---
title: "Tedm"
excerpt: "A C++ game engine with an SDL backend"
collection: portfolio
---

<a href="https://github.com/DavidWatkins/Tedm">
    <img src="{{ base_url }}/images/portfolio/tedm.png" alt="Tedm logo"
         title="Tedm Logo" align="right" />
</a>

# [Tedm](https://github.com/DavidWatkins/Tedm) [![Build Status](https://travis-ci.org/DavidWatkins/Tedm.svg?branch=master)](https://travis-ci.org/DavidWatkins/Tedm)
A C++ game engine with an SDL backend

# Dependencies
This library is fairly lightweight, only relying on SDL2 to offer a cross platform graphics library solution. 
- For Ubuntu 16.10
```bash
$ sudo apt-get install libsdl2-2.0 libsdl2-dev libsdl2-image1.2
```
or alternatively run 
```bash
$ sudo bash ./install-deps.sh
```
- For MAC OS X
```bash
$ brew install sdl2
```

# How to build
```bash
$ mkdir build && cd build
$ cmake .. && make
```

# Tutorial
[Tutorial for this project](https://github.com/DavidWatkins/Tedm/blob/master/Tutorial.md)

# Documentation
To build the documentation download doxygen and run:
```bash
$ doxygen doxygen_config
$ firefox documentation/html/index.html
```

<div class="github-card" data-github="davidwatkins/Tedm" data-width="400" data-height="150" data-theme="default"></div>
<script src="//cdn.jsdelivr.net/github-cards/latest/widget.js"></script>
