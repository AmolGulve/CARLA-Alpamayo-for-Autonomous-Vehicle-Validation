# CARLA-Alpamayo-for-Autonomous-Vehicle-Validation
CARLA + Alpamayo for Autonomous Vehicle Validation
## Overview

The **Alpamayo-Carla-Digital Cockpit** is an end-to-end autonomous vehicle validation and visualization system that integrates:

- **CARLA 0.9.15** — open-source AV simulator for scenario generation and sensor data output
- **Alpamayo R1-10B VLA Model** — NVIDIA Vision-Language-Action model for perception, reasoning, and trajectory planning
- **Digital Cockpit (Kirkstone AMI)** — embedded automotive dashboard running on EWAOL + Yocto Linux

The system runs entirely on **AWS Cloud** infrastructure and optionally bridges to **NVIDIA Jetson AGX Thor** hardware for real-world steering angle output.
The Alpamayo-Carla-Digital Cockpit includes the following functionalities
Sensor Data Generation
CARLA simulator generates sensor outputs including camera frames, vehicle pose, and velocity during scenarios.
Data Preprocessing
Data Adapter normalizes, adjusts resolution, buffers in frame cache, and formats ego-motion into vectors. This also receives the output trajectory waypoints optionally to CARLA from Alpamayo  for steer/throttle/brake for real time control 
AI Inference Processing
Alpamayo inference service asynchronously processes inputs using Vision-Language-Action model for output generation. Optionally output trajectory waypoints and reasoning trace to CARLA steer/throttle/brake for real time control
Digital Cockpit Dashboard Visualization
The layout includes Cluster/IVI Containers to display speed, speed limit alert and LDW for comprehensive visualization
