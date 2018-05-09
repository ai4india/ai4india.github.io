---
layout: single
title: "Automatic Helmet Detection using Surveillance Videos in Real Time"
description: "Simultaneous Localisation and Mapping in 2018"
header:
  overlay_image: /assets/images/projects/cell-segmentation/screenshot1.png
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
---

## Aim

Two-wheeler is very popular in India. However, there is high risk involved because of less protection. To reduce the risk involved, its often enforced to drive within speed limits (famous *Speed Thrills, but Kills*), follow traffic rules and more importantly, **Wear Helmets**.

Unfortunately in India, these rules arent given importance it deserves. Due to the scale of vehicles in Indian roads, its very difficult for Traffic Police to monitor the violators. The existing methods are very human intensive and prone to human errors. So automating this process is crutial. Moreover, the algorithm that should be designed must be robust, must be able to deal with low resolution images, lighting conditions and occulsion etc. Therefore without saying this makes it a difficult problem (particularly in Indian Setting) and an socially pressing problem to solve to save many innocent lives at stake in Indian Roads.

Algorithm must be capable of the following (in version 1):

* Real-time implementation
* Occlusion management
* Perspective Correction
* Temporal Changes handling (Environmental changes, lighting conditions and dynamic background)
* Quality of Video Feed and FPS (frames per second)


## Datasets:

* [Sparse Traffic Video from IIT Hyderabad Campus](https://sites.google.com/site/dineshsinghindian/dataset)

* [INRIA Person Dataset](http://pascal.inrialpes.fr/data/human/)

* [LSVRC2014 Object Detection Dataset](http://image-net.org/challenges/LSVRC/2015/ui/det.html)


## Proposed Algorithm

From the input image, using SSD find the places where the two-wheelers are present. Find the person present in the vicinity of the proposed region using people detection algoritms. Then using a metric to find the upper part of the body (possibly a head detection engine) localise the head/upper part of the detected person (who is assumed to be the driver). Using a standard SVM classifier or CNN classify whether the person has helmet or not.

Once the decision is made, store the image incase there is a clear violation of traffic rules and notify the concerned officials.
