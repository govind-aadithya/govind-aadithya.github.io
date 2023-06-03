---
title: "Helping Hand"
excerpt: "The project was made as an attempt to implement an assistive tech for people disabled neck down. Here, the direction of the eye is supposed to command the directional movement of a manipulator while the manipulator manipulates the object of interest. <br/><br/><img src='/images/Pupil_tracking_helping_hand.jpg'>"
date: 2016-03-10
collection: portfolio
---

Hardware used
===
1. Logitech camera

2. Dynamixel AX-12A Servos

About the project
===
With the goal of developing an assitive technology for severly disabled, we, at SRM Team Humanoid, developed a 6-DOF Robotic arm with inverse kinematic controller. To enable user to control the same, a pupil tracking algorithm was developed using Computer Vision which is used to provide directional and motion command to the hand. As a proof of concept we used it to manipulate a bottle as shown in the image.  

<img src='/images/Helping_hand.jpg'>


The pupil tracking was done using the following approach. The region of interest (ROI) is identified using pre-trained Haar-Cascade Classifier for an eye. Then, a grayscale thresholding is done on the ROI and Hough circles are used to identify the potential circles. If the number of circles is greater than two, the larger one is utilized as it will more accurately represent the centre of pupil.


<iframe width="560" height="315" src="https://www.youtube.com/embed/tV8FXf3_5Ro" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
