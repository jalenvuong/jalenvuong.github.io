---
layout: single
title: "3D Printed Collapsable Bridge"
permalink: /projects/collapsible-bridge/
author_profile: true
bridge:
  - url: /assets/photos/bridge_CAD.png
    image_path: /assets/photos/bridge_CAD.png
    alt: "CAD model of bridge"
    title: "CAD model of bridge"
  - url: /assets/photos/bridge_assembled.png
    image_path: /assets/photos/bridge_assembled.png
    alt: "3D Printed bridge, fully put together"
    title: "Final prototype of bridge, fully assembled"
  - url: /assets/photos/bridge_collapsed.png
    image_path: /assets/photos/bridge_collapsed.png
    alt: "3D printed bridge in most compact form"
    title: "3D printed bridge collapsed"
  - url: /assets/photos/bridge_fea_sim.png
    image_path: /assets/photos/bridge_fea_sim.png
    alt: "FEA test on bridge in Onshape"
    title: "FEA test on bridge in Onshape with point central load"
---

[← Back to all projects](/projects/)

**Tools:** Onshape, FEA, 3D Printing

## Context
Final project for CAD course MECH 203. 

## Project
- Designed a foldable bridge following the project's design criteria
- Ran FEA in Onshape to predict behavior under a center load
- Optimized the design to maximize strength-to-weight ratio

## Constraints
- Bridge must traverse 30 cm
- When collapsed, must fit within 20 cm x 10 cm x 8 cm
- Must weigh less than 200 g
- Must have at least 3 interlocking parts
- Must be PLA
- Ranked by strength to weight ratio

## Process
I started by researching various bridge forms, testing various types of trusses such as a K-truss and Pratt bridge. I made each shape in Onshape and used the simulation tool to test their behavior under a central point load if the bridge was rigidly supported at each end. After all these tests, I figured the best design for this scaled down bridge was a hybrid K-truss and Pratt bridge, as the combination offset each type's individual weakness and performed the best out of every bridge type I tried. Next, I moved to the interlocking constraint. At first, I tried a puzzle piece type of interlocking connection, but making the connecting tight was difficult and the joints were prone to failure during testing. I then pivoted to a rotating joint (see images below) that allowed the two load-bearing sides of the bridge to fold into the envelope and two non-load-bearing connecting pieces to hold the sides upright. This performed significantly better, as the rotating joints were perpendicular to the point load and weren't as prone to failure as the previous prototype, and the connectors allowed me to focus material in the load bearing parts and improve the strength to weight ratio of my bridge. Finally, when printing, I made sure to print the parts flat so that the layer lines would not be subject to shear, which would caule the bridge to fail earlier.
{% include gallery id="bridge" %}

## Outcome
Placed in the top 5 of the entire class with a strength to weight ratio of 120.8.
