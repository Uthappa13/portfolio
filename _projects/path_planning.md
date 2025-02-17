---
name: Path Planning for Warehouse Robots Using Informed RRT* and ROS2
tools: [Python, ROS2, Gazebo]
image: /portfolio/images/path_planning1.png
description: This project implements the Informed RRT* path planning algorithm and simulates the generated path using TurtleBot3 in the Gazebo environment.
---

# Path Planning for Warehouse Robots Using Informed RRT* and ROS2

## Project Overview

This project implements the Informed RRT* path planning algorithm and simulates the generated path using TurtleBot3 in the Gazebo environment. The algorithm efficiently finds an optimal path between a start and a goal position while avoiding obstacles.

## Languages & Tech stack

- **Python** for implementation.
- **ROS2** for the Robotics framework.
- **Gazebo** for simulation.
- **Matplotlib** for visualization.
- **numpy, geometry_msgs, nav_msgs** libraries used


## Methodology

- **Informed RRT* Algorithm**
    - Generates a random tree structure within the search space.
    - Expands towards a goal while avoiding obstacles.
    - Uses heuristics to improve path efficiency.
    - Optimizes paths dynamically as new nodes are added.

- **Simulation in Gazebo**
    - The path computed by Informed RRT* is passed to TurtleBot3.
    - TurtleBot3 moves through waypoints using ROS2 control messages.
    - The robot’s pose updates dynamically based on odometry feedback.

- **Simulation in Gazebo**
    - Explored states and the final path are displayed using Matplotlib.
    - The robot’s movement is visualized within Gazebo.


## Project Snippets

- **Path Visualization in Matplotlib**
    ![Path Visualization](/portfolio/images/rrt1.png)

- **Path Simulation in Gazebo**
    ![Path Simulation](/portfolio/images/rrtstar_video.gif)


## Detailed code on Github

<div class="left">
{% include elements/button.html link="https://github.com/Uthappa13/PathPlanning_WarehouseRobot" text="Code on Github" %}
</div>
