---
layout: page
subheadline: "Multi-Robot Planning for Non-Overlapping Operator Attention Allocation"
title:  "Past Research"
teaser: "Supplemental materials"
breadcrumb: true
# image:
    # thumb:
    # title:
    # caption_url:
permalink: "/research/projects/operator-scheduling"
---

### Authors
Sebastian A. Zanlongo, Mahbubur Rahman, Franklin Abodo, Leonardo Bobadilla

### Abstract
As society increases its reliance on remotely-operated and partially autonomous robots, we face the problem of how to effectively interact with large numbers of robots given a limited number of operators. In this paper, we present a methodology to allocate operator attention across multiple robots before plan execution while minimizing the duration of the plan. Our methodology has the following steps: 1) determine trajectories for robots, and when they will require supervision 2) create a coordination space representing operator attention conflicts 3) apply efficient algorithms to attempt reducing the time-span of robot activity by devising simple control policies, or assigning alternate trajectories 4) return a policy for each robot representing a feasible solution where operator attention is not overextended. Finally, we present simulation and a physical implementation to demonstrate the usefulness of the methodology.

### Motivation
Many current designs assume a 1:1 ratio of robots to remote operators. However, many aspects of a robots' operation can be automated, or at least planned for. With these capabilities, we only need an operator during certain sections of a robots' operation, and this can be scheduled in advance. This allows us to shift the ratio to a setting resembling $m$ robots to $n$ operators, where m >> n.

### Details
The below videos demonstrate, using a physical environment and a virtual simulator, how robots can be rescheduled so an operator can oversee robots, without splitting their attention across multiple critical activities.

##### Physical Demonstration
Software Simulation
<iframe width="560" height="315" src="https://www.youtube.com/embed/sjNepxbuajo" frameborder="0" allowfullscreen></iframe>

Hardware Experiment
<iframe width="560" height="315" src="https://www.youtube.com/embed/cG3xOQm0F4g" frameborder="0" allowfullscreen></iframe>

##### Simulation Demonstration
Two Robots with Critical Sections
<iframe width="560" height="315" src="https://www.youtube.com/embed/GBPwdvwb7w0?list=PLLzGu1x2MExwC1EAuVeDTuEHAlGR5GKya" frameborder="0" allowfullscreen></iframe>

Two Robots with Multiple Critical Sections
<iframe width="560" height="315" src="https://www.youtube.com/embed/jfUDwTf57Bs?list=PLLzGu1x2MExwC1EAuVeDTuEHAlGR5GKya" frameborder="0" allowfullscreen></iframe>

Three Robots with Two Critical Sections
<iframe width="560" height="315" src="https://www.youtube.com/embed/506dWPT00Ag" frameborder="0" allowfullscreen></iframe>

Three Robots with Multiple Critical Sections
<iframe width="560" height="315" src="https://www.youtube.com/embed/IgrjOQ0hKOU?list=PLLzGu1x2MExwC1EAuVeDTuEHAlGR5GKya" frameborder="0" allowfullscreen></iframe>