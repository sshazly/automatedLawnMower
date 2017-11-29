
-----------------------------------------------------------

# Dependencies

The following was build using ROS/Kinetic. Dependencies include:

(None at the moment)

--------------------------------------------------------------

# Clonging Repo

git clone https://github.com/sshazly/automatedLawnMower


--------------------------------------------------------------

# Summary

The following repository contains the completed tutorials for creating ROS packages and implementing nodes. Publisher and Subscriber are used to send messages to a node and read messages from that same node using listener.cpp and talker.cpp located in the ~/catkin_ws/src/beginner_tutorials/src/ directory.
# C++ Robotic Motion Controller
[![Build Status](https://travis-ci.org/sshazly/automatedLawnMower.svg?branch=master)](https://travis-ci.org/sshazly/automatedLawnMower)
[![Coverage Status](https://coveralls.io/repos/github/sshazly/automatedLawnMower/badge.svg)](https://coveralls.io/github/sshazly/automatedLawnMower)
---

## Overview

Automated Lawn Mower:

The following package features a 4 wheeled robot with the 2 front wheels that use DC-motors to control the turning and motion. The 4 wheeled robot is used to train and follow a path using position sensors and 

The code is meant to interface with a path-planning algorithm which gives the robot a desired position and orientation at described time increments. 

With the input from the path-planning algorithm the code determines what rotational velocity the DC-motors need to attain in order to drive the front wheels to desired outputs specified by the path-planner, or in the case of the simulation, the path-planner output file.

A simulation is performed in Gazebo. The robot is made to follow a path described in the path-planning output file, which is recorded by the user, and that is the extent of the simulation. Various proximity sensors were also included in the simulation for obstacle detection and a dynamic obstacle is provided in the form of a dog which travels a pseudo random path in the yard.


## Project Logs

The following is a link to the project logs:

https://docs.google.com/spreadsheets/d/e/2PACX-1vRDCi5ylcphjV42Bh_Aa_Iq14gxiu5XBCAERG2IHx4oSVK4L61qoVfIYtC42oFmOEAXIaj9rNNAc3jg/pubhtml


--------------------------------------------------------------
# Directions
Once cloned, the implementation can be achieved by:

1)  Navigating to the ~/catkin_ws/ directory

 	$ cd ~/catkin_ws

2)  Implementing the cmake equivalent for ROS

 	$ catkin_make

3)  Opening five new terminals...

On the first terminal:

 	$ roscore


OR 

run the package

On the first terminal:

 	$ roscore

On the second terminal:
	$ cd ~/catkin_ws/
 	$ source ./devel/setup.bash
 	$ roslaunch automated_lawn_mower conversation.launch

-------------------------------------------------------------------
	

