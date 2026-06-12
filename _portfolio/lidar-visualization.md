---
title: "Autonomous Perception & LiDAR Visualization"
excerpt: "Developed a ROS 2 & RViz2 simulation environment to process and visualize high-density LiDAR point clouds from the KITTI dataset."
collection: portfolio
---

**Tech Stack:** *ROS 2, RViz2, Linux (Ubuntu), Point Cloud Data, KITTI Dataset*

<img src="/images/lidar-preview.gif" alt="LiDAR RViz2 Visualization" width="100%" style="border-radius: 8px; border: 1px solid rgba(255,255,255,0.1); margin-bottom: 20px;">

### Overview
Developed a simulation environment to process and visualize high-density LiDAR point clouds and camera feeds for autonomous vehicle perception.

### Key Implementations
* Replayed and analyzed complex `.mcap` sensor data from the KITTI Vision Benchmark Suite using **ROS 2**.
* Configured **RViz2** to synchronize multi-sensor streams, overlaying 3D LiDAR point clouds with real-time 2D camera feeds to simulate real-world autonomous navigation.
* Handled spatial transforms (TF) and simulated clock synchronization to ensure accurate playback of multi-modal environmental data.