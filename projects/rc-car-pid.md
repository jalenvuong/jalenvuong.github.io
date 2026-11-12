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
{% include video id="5nadyTWDfc8" provider="youtube" caption="Demo of PID controller on RC car" %}

## Outcome
The car was able to self correct and go in a straight line for at least 4 meters.
