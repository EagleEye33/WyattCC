---
layout: post
title:  "A virtual mailroute delivery robot in Javascript"
date:   2021-12-22
categories: General Posts
author: Wyatt 
---

The aim of this project was to dive head first into a pure javascript project 
using all the fundamentals from program structure to higher-order functions and object-oriented programming.

You can view the interactive animation for the robot here: [deliveryRobotAnimation](https://wyattcolyn.github.io/mailRobot/){:target="_blank"}

- There are some detailed updates for this project below.

There are four robots to select from(four robot functions):
1. The randomRobot is self explanatory: The robot will make pseudo random choices on where to go next 
2. The standardRobot will mimic how real world mail delivery systems work: The robot will make two full complete cycles of the route - one for picking up all the parcels and another for delivering the parcels. This gurantees the robot will complete in a maximum of 26 turns. 
3. The smartRobot is a major improvement in terms of intelligent decision making. smartRobot will check every path around it that is a valid location for dropping off a parcel or picking up a parcel in the current route and move toward the closest one.
4. lazyRobot is similar to smartRobot except there is a small bonus system for paths that include picking up parcels. For example, if a valid drop off location is one step away(assuming the robot already has the parcel to drop off at the location in interest) versus a location two steps away but has three parcels, the robot will move toward picking up the parcels first.