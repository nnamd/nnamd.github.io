---
title: Classification and Dataset Collection For the Laban Efforts 
description: Machine Learning
img-feat: Space.png
website: 
methods:
  - Classical Machine Learning
  - Feature Importance
tools:
  - SKLearn/Sci-Kit
  - Python
  - R


samples-title: Samples

sample-img-1: Flow.png
sample-img-alt-1: Flow Image 
sample-img-caption-1: Example Image of Stylized Demonstration From Participant (Flow)

sample-img-2: Space.png
sample-img-alt-2: Space Image 
sample-img-caption-2: Example Image of Stylized Demonstration From Participant (Space)
---


## Abstract
Robot motion has been shown to impact both the perception of social and functional goals that robot's carry, even when unintended. The Laban Efforts, one of the primary modes of creation and interpretation of the expressivity of motion, has been well documented and explored in the field. However, many of the existing explorations feature unscalable hand-designed motions. Even in learning-based or rule-based models, they are either limited in platform or have attempted translation across form factors unsuccessfully. We sought to address these issues by offering a dataset of Laban Effort-based demonstrations on a robotic arm, arguing that crowd-sourcing from the target platform is a valid and pivotal alternative. Additionally, we do preliminary analysis of a classification on the effort axes to better understand how the Laban Efforts can manifest in an object-seeking task. We find that the weight and space axes had the highest performance (> 90%) after reducing to a subset of features using LASSO. LASSO additionally offers some relative insight into future predictors to use as starting points to potentially modulate effort perception. This work is currently in progress.


## Technical Details
For the data collection, a record and replay module was designed using an existing **Kinova Gen3**'s compliant controller utilizing the **ROS** framework in Python. The models were trained on a set of 15 engineered features extracted from the collected dataset of robot joint angles and velocities over time. Much of the feature set of was influrenced by features explored in different form factors for past work. Feature reduction strategies in **LASSO** and removal based on **Variable Inflation Factor** were both explored and reported. The work focuses on the training of classical machine learning models  with performance ratings in **F1-score**, **Confucian matrices**, and **runtime** being points of reference to analyze performance. The chosen models were *K-Nearest Neighbors, Logistic Regression, Guassian Naive Bayes, Support Vector Machines, and a multi-layer feedforward network*. Hyperparamters of the network were optmized based on  a restricted grid search. Models were trained using the **Sci-kit** library/environment. 