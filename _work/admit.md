---
title: Admittance Control of Bravo 7
description: Dynamics & Controls
img-feat: initial_config.jpg
website: 
methods:
  - Simulation
  - Admittance Control
tools:
  - MATLAB
  - Python

samples-title: Samples
sample-img-1: sim_results.gif
sample-img-alt-1: Bravo Arm Simulation 
sample-img-caption-1: Gif of Simulated Forces on Bravo Arm
sample-img-2: admittance_sim_plot.png
sample-img-alt-2: Admittance Control Sim Plot
sample-img-caption-2: The real admittance controller response on the Bravo 7 when force is applied to the manipulator’s end effector
sample-img-3: final_graph_hardware.png
sample-img-alt-3: Admittance Control On Hardware Graph
sample-img-caption-3: The simulated admittance controller demonstrates compliance when a 25N force is applied to the manipulator’s end effector
---

## Overview

Underwater manipulation tasks require precise manipulator and vehicle control to safely complete tasks like environmental sampling and dock maintenance. As underwater vehicle-manipulator systems (UVMS) are subject to complex hydrodynamic motions, UVMS must account for any undesired dynamic changes or external forces that occur during a manipulation task. In this paper, we propose an admittance control law that uses measured end-effector forces to determine the compliant motion required to minimize interaction forces. With this approach, we demonstrate, both in simulation and hardware, results for compliant motion of a manipulator that minimizes interaction forces.