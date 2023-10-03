# Motion Planning for Self-Driving Cars

![Cover](./media/cover.gif)

This course will introduce you to the main planning tasks in autonomous driving, including mission planning, behavior planning and local planning. By the end of this course, you will be able to find the shortest path over a graph or road network using Dijkstra's and the A* algorithm, use finite state machines to select safe behaviors to execute, and design optimal, smooth paths and velocity profiles to navigate safely around obstacles while obeying traffic laws. You'll also build occupancy grid maps of static elements in the environment and learn how to use them for efficient collision checking. This course will give you the ability to construct a full self-driving planning solution, to take you from home to work while behaving like a typical driving and keeping the vehicle safe at all times. For the final project in this course, you will implement a hierarchical motion planner to navigate through a sequence of scenarios in the CARLA simulator, including avoiding a vehicle parked in your lane, following a lead vehicle and safely navigating an intersection.

## The Planning Problem

This module introduces the richness and challenges of the self-driving motion planning problem, demonstrating a working example that will be built toward throughout this course. The focus will be on defining the primary scenarios encountered in driving, types of loss functions and constraints that affect planning, as well as a common decomposition of the planning problem into behaviour and trajectory planning subproblems. This module introduces a generic, hierarchical motion planning optimization formulation that is further expanded and implemented throughout the subsequent modules.



## Mapping for Planning

The occupancy grid is a discretization of space into fixed-sized cells, each of which contains a probability that it is occupied. It is a basic data structure used throughout robotics and an alternative to storing full point clouds. This module introduces the occupancy grid and reviews the space and computation requirements of the data structure. In many cases, a 2D occupancy grid is sufficient; learners will examine ways to efficiently compress and filter 3D LIDAR scans to form 2D maps.



## Mission Planning in Driving Environments

This module develops the concepts of shortest path search on graphs in order to find a sequence of road segments in a driving map that will navigate a vehicle from a current location to a destination. The modules covers the definition of a roadmap graph with road segments, intersections and travel times, and presents Dijkstra’s and A* search for identification of the shortest path across the road network.



## Dynamic Object Interactions

This module introduces dynamic obstacles into the behaviour planning problem, and presents learners with the tools to assess the time to collision of vehicles and pedestrians in the environment.



## Principles of Behaviour Planning

This module develops a basic rule-based behaviour planning system, which performs high level decision making of driving behaviours such as lane changes, passing of parked cars and progress through intersections. The module defines a consistent set of rules that are evaluated to select preferred vehicle behaviours that restrict the set of possible paths and speed profiles to be explored in lower level planning.


## Reactive Planning in Static Environments

A reactive planner takes local information available within a sensor footprint and a global objective defined in a map coordinate frame to identify a locally feasible path to follow that is collision free and makes progress to a goal. In this module, learners will develop a trajectory rollout and dynamic window planner, which enables path finding in arbitrary static 2D environments. The limits of the approach for true self-driving will also be discussed.

## Smooth Local Planning

Parameterized curves are widely used to define paths through the environment for self-driving. This module introduces continuous curve path optimization as a two point boundary value problem which minimized deviation from a desired path while satisfying curvature constraints.

# Introduction

## 1. Overview

Be at the forefront of the autonomous driving industry. With market researchers predicting a $42-billion market and more than 20 million self-driving cars on the road by 2025, the next big job boom is right around the corner.

This Specialization gives you a comprehensive understanding of state-of-the-art engineering practices used in the self-driving car industry. You'll get to interact with real data sets from an autonomous vehicle (AV)―all through hands-on projects using the open source simulator CARLA.

Throughout your courses, you’ll hear from industry experts who work at companies like Oxbotica and Zoox as they share insights about autonomous technology and how that is powering job growth within the field.

You’ll learn from a highly realistic driving environment that features 3D pedestrian modelling and environmental conditions. When you complete the Specialization successfully, you’ll be able to build your own self-driving software stack and be ready to apply for jobs in the autonomous vehicle industry.

It is recommended that you have some background in linear algebra, probability, statistics, calculus, physics, control theory, and Python programming. You will need these specifications in order to effectively run the CARLA simulator: Windows 7 64-bit (or later) or Ubuntu 16.04 (or later), Quad-core Intel or AMD processor (2.5 GHz or faster), NVIDIA GeForce 470 GTX or AMD Radeon 6870 HD series card or higher, 8 GB RAM, and OpenGL 3 or greater (for Linux computers).

---

## 2. Learn Objects

- Understand the detailed architecture and components of a self-driving car software stack
- Implement methods for static and dynamic object detection, localization and mapping, behaviour and maneuver planning, and vehicle control
- Use realistic vehicle physics, complete sensor suite: camera, LIDAR, GPS/INS, wheel odometry, depth map, semantic segmentation, object bounding boxes
- Demonstrate skills in CARLA and build programs with Python
