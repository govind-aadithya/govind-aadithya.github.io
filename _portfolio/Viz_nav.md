---
title: "Embodied AI and Visual Navigation challenge"
excerpt: "A challenge to navigate to a specific pose represented by First Person View (FPV) on all four directions of the agent with just the current FPV as the input.  <br/><br/><img src='/images/maze_robot.gif' height='100'>"
date: 2023-12-01
collection: portfolio
---

About the project
===
This project was done as a part of Robot Perception coursework. 
The objective of the project was to autonomously navigate the robot, with just visual navigation with First Person View input, to a given goal representation. 

Solution:
Graph SLAM stores the key points and descriptors alongside the current pose as a linked list. This helps us track the flow/movement of the robot through the environment. The pose is comuted with forward stepping the keystroke. This linked list forms our Graph SLAM base. Loop closure is not considered in the solution, but adding a loop closure with multiple pointers to this solution will make a better representation of the map.

The VPR in this solution is implemented as a simple key point and feature search over the Graph. The node with the maximum match over a threshold is then extracted as the target location. This solution can be further fine-tuned with an implementation leveraging Visual Bag Of Words or VLAD leveraging the fact that the patterns that could occur in the maze are already known.

Below is a visual representation of the solution.

<img src='/images/GSlam.gif' height='300'>
<img src='/images/VPR.gif' height='300'>


More detailed breakdown of the project can be found in the repository [here](https://github.com/govind-aadithya/Viz_nav).
