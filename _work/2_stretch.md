---
title: Various Stretch RE2 Projects
description: Behavioral Studies & Applied Robotics
img-feat: Effort_Classifier.png
website: 
methods:
  - Human Subject Studies
  - Qualitative Research
tools:
  - Python
  - R
  - Jamovi


sample-img-1: pickup.gif
sample-img-alt-1: Pickup Gif 
# sample-img-caption-1: Example Image of Stylized Demonstration From Participant (Flow)

sample-img-2: uncalibrated.gif
sample-img-alt-2: Uncalibrated Gif
# sample-img-caption-2: Example Image of Stylized Demonstration From Participant (Space)

sample-img-3: omic.png
sample-img-alt-3: Weight Image 
sample-img-caption-3: OMIC Project Overview 

sample-img-4: states.png
sample-img-alt-4: States 
sample-img-caption-4: Mealy Machine States

sample-video-1: rss.mp4
sample-video-alt-1: RSS Supplementary Video
---


## Overview
Consequential robot motion and sound has been shown to impact the perception of robotic systems; this could affect the perceived trust in their ability to carry out their objectives. These projects explored two avenues, one through sound the other through motion on a Stretch RE2. The former acted as a replication study based on previous efforts on mobile robots using continuous and functional sound as a way to indicate completion and convey location. The latter explored using motion as a way to convey key state information: whether a module of the robot was in-fault and why. 

[Sound Paper](https://roboticsconference.org/2024/program/papers/32/)

## Technical Details
I worked on the experimental design and setup of both studies. I designed finite state machines in order to manage robot behavior for the sound study navigation task from the pickup location to drop-off for the participants. I utilized R and Python for the data analysis. For the motion study, I designed services and actions in ROS to enable pickup based on Aruco tags and also to allow for the execution of other expressive motor behaviors during navigation. In a group of 2, we explored a set of relevant states and failures that could occur during a pick and place task and worked to replicate the environment and states for our human-subject study.  

