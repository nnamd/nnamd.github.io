---
title: Following Viewpoint
description: Geometric Mechanics
img-feat: cover_view.png
website: 
methods:
  - SE(2)
tools:
  - Python
  - Pygame



sample-img-1: geo_1.png
sample-img-alt-1: Setup Image
# sample-img-caption-1: Example Image of Stylized Demonstration From Participant (Flow)

sample-img-2: geo_2.png
sample-img-alt-2: More Setup
# sample-img-caption-2: Example Image of Stylized Demonstration From Participant (Space)

sample-img-3: geo_3.png
sample-img-alt-3: Final Math
sample-img-caption-3: OMIC Project Overview 


sample-video-1: viewpoint.mkv
sample-video-alt-1: Viewpoint Supplementary Video
---


## Overview
In this project I explored the use of SE(2) as a mode of moving objects relative to one another. The main question of this work is can we retain a moving shape within the middle of a target’s FOV? The parent triangle is controlled by the user where the second triangle charts a continuous circle in the POV of the first. 

## Technical Details
For this we consider the 2D problem where we’re treating perspective as the reference frame that we’re in and wanting to again create a shape about the ref of configuration *g_a*. This becomes a particularly interesting problem when we start to consider the time component of config *g_b* as its charting its shape while also being ‘rigid’ in its location. 

The real first step in this is first having setup a PID controller in order to find adequate body velocities to track the circle. From there, We can treat this as a rigid body problem where we have the center of that circle or whatever shape we’d want to chart mapped to a specific point. The main idea here is that we’d get one component of the body velocities from the holding shape of the circle and another from transforming the body velocities happening at g_a (that we’re directly controlling) to what the velocities should be at some time specific value of h that again is just based on the initial config of g_b(t). And from there its just a matter of using the Adjoint w/ that h function we gathered prior.   

The last thing you’d also need to do however at every time step is to track circle itself in space so we can update our controller, that I did just by tracking the changes made to a central anchor of the shape. 




