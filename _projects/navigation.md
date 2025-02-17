---
name: Aruco-Assisted Navigation of a Warehouse Robot
tools: [C++, ROS2, Gazebo]
image: /portfolio/images/navigation1.jpg
description: This project focuses on developing a ROS2 package that enables a robot to navigate a warehouse environment.
---

# Aruco-Assisted Navigation of a Warehouse Robot

## Project Overview

This project focuses on developing a ROS2 package that enables a robot to navigate a warehouse environment using Aruco markers for guidance. While navigating, the robot detects and reports objects present in the environment. The key objectives include:
- Moving the robot through the environment by detecting Aruco markers.
- Executing predefined actions based on marker identification.
- Detecting and reporting the pose of objects in the environment.

## Languages & Tech stack

- **C++** for implementation.
- **ROS2** for the Robotics framework.
- **Gazebo** for simulation.


## Project Workflow

- **Robot Navigation Logic**
    - Move forward until an Aruco marker is detected.
    - Stop at ≤ 0.4m from the detected marker.
    - Perform an action based on the marker ID.
    - Continue navigating until the end marker is detected.
    - Upon reaching the end, detect and report the pose of batteries.

- **Object Detection and Pose Estimation**
    - The RGB camera detects Aruco markers and publishes data to /aruco_markers.
    - The logical camera detects floating objects and publishes to /mage/advanced_logical_camera/image


## Project Snippets

 <!-- **Path Visualization in Matplotlib** -->
<!-- ![Vibration Data](/portfolio/images/bearing_project2.png) -->

- **Navigation Simulation in Gazebo**
    ![Nav sim](/portfolio/images/nav1.png)


## Detailed code on Github

<div class="left">
{% include elements/button.html link="https://github.com/Uthappa13/Navigation_WarehouseRobot" text="Code on Github" %}
</div>
