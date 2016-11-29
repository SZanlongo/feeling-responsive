---
layout: page
subheadline: "Robot Coordination Space"
title:  "Development"
teaser: "Generates a coordination space for n robots with n static obstacles residing in a 2D plane."
breadcrumb: true
header:
   image_fullwidth: "development/projects/robot-coordination-space/robot-coordination-space_01.jpg"
permalink: "/development/projects/robot-coordination-space/"
---

[GitHub link](https://github.com/motion-planning/robot-coordination-space)

- Takes as input the obstacle and policy files from a working trajectory given by the MSL Library.
- Generates an n-dimensional coordination space indicating which areas result in a collision.
- Provides ability to:
  - Plot 2D robot trajectories
  - Plot 2D and 3D coordination space and it's collision states
  - Plot 2D and 3D A* trajectory through Coordination Space, providing a safe path from start to goal configurations
