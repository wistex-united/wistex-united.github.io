---
title: 2024-11-26 WISC Meeting
layout: default
parent: Meeting Notes
---

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Simulation and Environment

### Adam
  - Exploring learning with Mujoco
  - Josiah suggest Webot simulation as a way to consider

### Zhihan
  - Successfully transferred V2 to NAO robot
  - Ensuring coordination parameters match between simrobot and abstract
  - Not yet integrated with Abhinav's version; plans to merge changes later
  - Adding tutorial documentation
  - Plan to implement new features:
    - Kick skill implementation in V2
    - Medium-level skills (e.g., walk to point)

### Version Integration Discussion
  - Multi-agent training switch to V2
  - Zhihan's version is focus on transferring and training
  - Abhinav's version focusing on reconfiguration
  - Plan to move changes to Abhinav's branch
  - Current issues:
    - V2 exhibits unusual behavior with angled kicks
    - Strategy: Transfer to Zhihan's branch first (similar to V1)
  - Goal: Achieve stable status combining both versions

### Will
  - Working on multi-agent reinforcement learning
  - Plans to transfer work to V2 in future phases
## Referee Gesture
### Zisen
  - In paper sent by peter, MobileNet-V2 proven viable on NAO hardware
  - Still need for improved efficiency due to concurrent vision pipeline processing
  - Insight from paper, number of filters impacts inference time more than layer count
  - Tried vanilla GAN for new domain data augmentation
  - Josiah suggest also try diffusion for data augmentation

## Environment Issues
### Yuhao
  - Fixed environment bugs, but shared memory has its natural issues
  - GNU-related challenges
  - Multiple robot simulation causing problems in SimRobot
  - BCO implementation pending after merge training
  - Josiah suggests focus on single-agent behavior cloning before scaling to multi-agent

## Framework Discussion
  - RLite: Complex implementation, documentation has latency from code
  - Tianshou: 
    - Undergoing refactoring
    - Lightweight design
    - Better performance
  - CleanRL: Preferred for research purposes