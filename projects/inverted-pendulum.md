---
layout: single
title: "Inverted Pendulum Simulation"
permalink: /projects/inverted-pendulum/
author_profile: true
pendulum_plots:
  - url: /assets/photos/cartanglegraph.png
    image_path: /assets/photos/cartanglegraph.png
    alt: "Plot of pendulum angle over time"
    title: "Pendulum angle over time"
  - url: /assets/photos/cartgraph.png
    image_path: /assets/photos/cartgraph.png
    alt: "Plot of cart position over time"
    title: "Cart position over time"
---

[← Back to all projects](/projects/)

**Tools:** Python, PID controls, Mathematical Modeling

## Context
Personal project to practice mathematically modeling systems and to get further practice with control systems.

## Project
- Modeled an inverted pendulum balanced by a cart using PID control
- Derived the equations of motion using the Lagrangian
- Plotted the behavior in Python and tested it with a range of different masses

## Process
The hardest part of the project was definitely writing the control loop. I first calculated the equations of motion using the Lagrangian method. With the EOMs, I moved on to writing the control system. I struggled a lot because I initially attempted to control the entire system only using a PID loop for the cart. However, that led the cart to drive straight off the edge in one direction because it only attempted to make the arm vertical. I then pivoted to a nested PID loop; an outer loop which keeps the cart centered and produces a desired lean angle for the pendulum, and an inner loop which tracks the lean angle and updates the cart's force. That allowed the cart to actually stay within a reasonable length.

{% include gallery id="pendulum_plots" layout="half" %}

## Outcome
I was able to successfully create a control system for an inverted pendulum on a cart. I learned about nested PID control loops and how to apply them to systems where multiple dimensions are being controlled. In the future, I aim to create a physical inverted pendulum to apply my control system on and to investigate alternative control systems that might not require a nested control loop.
