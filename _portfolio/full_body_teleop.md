---
title: "Full-body Shadowing"
excerpt: "Building on the upper body teleop project, an attempt to track the whole upper body was done and the joint angles were replicated by the robot to shadow the operator. <br/><br/><img src='/images/ATHum.jpg'>"
date: 2017-05-14
collection: portfolio
---

Hardware
===
1. Robotis Darwin OP3
2. X-Box Kinect RGBD camera 
3. Logitech Webcam

About the project
===
In an attempt to create a robot that can "shadow" an operator (inspired by Real Steel), we extended the upper body motion tracker to a full body motion tracker that is capable of calculate the joint angles of all critical joints.
We then use this joint data to operate the robot alongside generating waliking commands.  

<iframe width="560" height="315" src="https://www.youtube.com/embed/znR0XXcpGIs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

The robot's movements are controlled by a human from a remote place by extracting the joint angles of an operator standing in front of an RGBD Camera. These joint angles are fed to the robot to replicate the human motion as closely as possible. 
In order to give the realtime update of the robot's side to the operator to close the loop, a camera mounted on the humanoid transfers a live feed through a VR Headset to the user. This way, we can virtually give the user the experience of being in the moment while doing the teleoperation.

We competed in the freestyle round of Robogames'17 using this concept and secured a silver medal for the same.
