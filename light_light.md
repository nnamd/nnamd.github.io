---
title: "Lighty Light Zoom Zoom"
description: Embedded Systems Project
img-feat: work.png
website: https://
methods:
  - PWM
  - Concurrency
  - Pair Programming
tools:
  - C
  - GitHub
  - Freedom Development Board
samples-title: Samples
sample-img-1: work.png
sample-img-alt-1: Work example 1 screenshot
sample-img-caption-1: Work example 1 screenshot
sample-img-2: work.png
sample-img-alt-2: Work example 2 screenshot
sample-img-caption-2: Work example 1 screenshot
sample-img-3: work.png
sample-img-alt-3: Work example 3 screenshot
sample-img-caption-3: Work example 3 screenshot
sample-img-4: work.png
sample-img-alt-4: Work example 4 screenshot
sample-img-caption-4: Work example 4 screenshot
---

## Overview
I, in a group of 2, created a system that would light up LEDs based on the direction and intensity at which the microcontroller was shook. The change in acceleration data read periodically on the board is used to increase the intensity of the LEDs on the board relative to the direction. Shaking the system along its width will increase RED LED’s intensity, shaking it along its length increases the GREEN LED’s intensity, and shaking it up and down increases the BLUE LEDs intensity. All three directions can be utilized to create a myriad of colors. When you stop shaking the board in a respective direction the corresponding LED will then fade out until it turns off. This system took advatage of concurrency in order to manage the simultaneous reading of acceleramotor data and its accompanying response.

Link to [project page](https://pages.github.coecis.cornell.edu/ece3140-sp2020/aky26-nan46/) and [showcase video](https://www.youtube.com/watch?v=oMNsw_Cgbkg)