---
title: "Animatronic Hand: A Tele-operation Prototype"
excerpt: "An Animatronic Hand that mimics hand gestures via remote actuation commands. Done during the NJIT Hardware Hackathon, Byte into Hardware. <br/><br/><img src='/images/Archi.png' height='300'>"
date: 2023-04-01
collection: portfolio
---

Hardware
===
1. 3D Printed Animatronic Hand
2. Tower Pro Servos (SG90)
3. Logitech Web Cam
4. Arduino
5. IMU - MPU6050.

About the project
===
This project was done as a part of the NJIT Hardware Hackathon 2023, "Byte into Hardware". This was a 24hr hackathon where we had to develop a working model in the theme of Assistive Technology. We targeted assistance for workers in "Hazardous Environments" and as PoC for teleoperative assistance, we executed this project.

The project uses Computer Vision to perform gesture tracking and interpret the geture made by the user. This is then sent to the Arduino as actuation commands to make the Animatronic hand replicate the gesture.
To complete the loop, we used a logitech webcam to provide a video feed to the user by couping it with servos for yaw control. The command to the yaw control is given via an IMU that tracks the yaw of the user's head.


<iframe width="560" height="315" src="https://www.youtube.com/embed/Sb4F23Tmr3c?si=DhgsqGnh2qYovL29" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


More detailed breakdown of the project can be found in the repository [here](https://https://github.com/govind-aadithya/Animetronic-Hand).
