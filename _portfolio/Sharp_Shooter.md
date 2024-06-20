---
title: "Sharp Shooter"
excerpt: "The goal of the project was to track an object of a specific color and aim to shoot it when it reaches a specific threshold. <br/><img src='/images/Sharp_Shooter.jpg'>"
date: 2016-02-16
collection: portfolio
---

Hardware used
===
1. Robotis Bioloid GP 

2. Dart/Nurf gun

3. Logitech camera

4. Dynamixel AX-12A Servos

About the project
===
The project was aimed at tracking a specific colored object and shooting at it when its area was beyond a specific threshold. 

The robot is fitted with a camera attached to two servo motors which are capable of executing Pitch and Yaw motions. Once the pre-coded color appears in the frame the target is locked and the robot starts to track the object. The tracking is done via a PID controller with the visual feed and the error of object from the center (in Pixel) is used as a control input. In the initial phase of the video, the tracking and its accuracy are demonstrated. Once the tracked object crosses a specific pre-determined size, the robot then uses inverse kinematics to compute the target location to aim and shoot at it. The end effector position is determined by the position of the image on the feed and the camera's roll and yaw angles which is then frame transferred to the base (shoulder joint) of the Bioloid to execute the inverse kinematics calculations. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/BUanlEODqq4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe> 


Fun fact:

This project was demonstrated in the Freestyle event of Robogames'2016 and the robot ended up shooting a by standing judge, with great accuracy, who happened to wear the same color as the one being tracked. The judges were impressed with the accuracy though (Lol!). 

**Disclaimer:  This project was done to implement and transfer learning from the course works in a fun way. As a responsible roboticist, there was, is, and will never be intentions to weaponize robots.  I stand by and support the "Open Letter" issued by the leading robotics companies.**
