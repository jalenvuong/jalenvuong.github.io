---
layout: single
title: "Simple PID Control for RC Car"
permalink: /projects/rc-car-pid/
author_profile: true
---

[← Back to all projects](/projects/)

**Tools:** Arduino, Python, IMUs

## Context
Personal project to get an introduction to control systems.

## Project and Constraints
- Used PID control to keep the RC car moving in a straight line and counteract drift
- Set a goal of driving 4 meters in a straight line to collide with a target directly ahead
- Tuned the gain coefficients to get the behavior I wanted

## Process
At first, I noticed when the car was supposed to go straight forward (e.g. all 4 wheel motors were set to maximum output), the car drifted left significantly. I decided to use the MPU's IMU to detect changes in its yaw. At first, I tried to use a PI controller because I didn't anticipate turning speed to be an issue while self-correcting it's orientation. However, that led to the car sometimes spinning out of the straight line completely, so I pivoted to a PID controller so it wouldn't overshoot it's heading and cause spiraling. 
{% include video id="5nadyTWDfc8" provider="youtube" caption="Demo of PID controller on RC car" %}

## Outcome
The car was able to self correct and go in a straight line for at least 4 meters, reaching the goal distance I set out for the project.
