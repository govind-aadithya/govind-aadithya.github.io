---
title: "Fire Detector"
excerpt: "The aim of the project was to develop a Computer Vision algorithm to detect fire from video feed. This can be used in public places with surveillance cameras to monitor and notify any cases of fire breakout. <br/><br/><img src='/images/Fire_Detection.jpg'>"
date: 2015-11-25
collection: portfolio
---

About the project
===
This project aimed at developing a safety system that monitor fire break out from survilance cameras and warns the security and other emergency systems to take the necessary safety actions. The project was executed using computer vision using OpenCV-Python. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/Hm-Vrb0lZRc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

The approach taken uses converting the color space to YUV and uses channel thresholding to extract the ROI related to "fire". Since this is a stand alone computer vision approach, this may have false positives. So, it has to be coupled with physical sesors to reinforce the warning.
