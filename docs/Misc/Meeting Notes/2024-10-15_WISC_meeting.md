---
title: 2024-10-15 WISC Meeting
layout: default
parent: Meeting Notes
---

- Moved the documentation to GitHub pages.
- SimRobot IL
  - Trying to run SimRobot on GPU without rendering for maximum speed.
  - Headless mode still renders with CPU and is very slow (10% GPU speed).
- Mujoco NAO
  - Adding joint information to the simulation.
  - Manually adding motors and calibrating with the real robot.
- Vision
  - Using keypoints on the human body to estimate gesture via MediaPipe (lightweight).
- AbstractSim V2
  - Adding config files; making everything modular.
  - Continuous control dynamics don't match SimRobot/the real robots very well.
  - Potentially try a discrete action space or walk to point?
  - Can try training a network to approximate true robot dynamics.
