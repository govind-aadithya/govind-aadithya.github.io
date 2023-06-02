---
title: "Sharp Shooter"
excerpt: "Goal of the project was to track an object of specific color and aim to shoot it when it reaches a specific treshold.
<br/><img src='./images/Sharp_Shooter.jpg'>"
collection: portfolio
---

Hardware used
===
1. Robotis Bioloid GP 

2. Dart/Nurf gun

3. Logitech camera

4. Robotis Servos

About the project
===
The project was aimed at tracking a specific colored object and shoot at it's area goes beyond a specific threshold. 

The robot is fitted with a camera attached to two servo motors which are capable of executing a Pitch and Yaw motions. Once the pre-coded color appears in the frame the target is locked and the robot starts to track the object. The tracking is done via a PID controller with the visual feed and the error of object from the centre (in Pixel) is used as control input. In the initial phase of the video, the tracking and it's accuracy is demonstrated. Once the tracked object crosses a specific pre determined size, the robot then uses inverse kinematics to compute the target location to aim and shoot at it. The end effector position is determined by position of the image on the feed and the camera's roll and yaw angles which is then frame transferred to the base (sholder joint) of the Bioloid to execute the inverse kinematics calculations. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/BUanlEODqq4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe> 

Fun fact:

This project was demonstrated in the Freestyle event of Robogames'2016 and the robot ended up shooting a bystanding judge, with great accuracy, who happened to wear the same color as the one being tracked. The judges were impressed with the accuracy though (Lol!). 

**Disclaimer:  This project was done to implement and tranfer leraning from course works in a fun way. As a responsible roboticist, there was, is, and will never be intentions to weaponize robots.  I stand by the and support the "Open Letter" issued by the leading robotics companies.**
