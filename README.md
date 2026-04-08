# CARLA-Alpamayo-for-Autonomous-Vehicle-Validation
CARLA + Alpamayo for Autonomous Vehicle Validation
## Overview

The **Alpamayo-Carla-Digital Cockpit** is an end-to-end autonomous vehicle validation and visualization system that integrates:

- **CARLA 0.9.15** — open-source AV simulator for scenario generation and sensor data output
- **Alpamayo R1-10B VLA Model** — NVIDIA Vision-Language-Action model for perception, reasoning, and trajectory planning
- **Digital Cockpit (Kirkstone AMI)** — embedded automotive dashboard running on EWAOL + Yocto Linux

The system runs entirely on **AWS Cloud** infrastructure and optionally bridges to **NVIDIA Jetson AGX Thor** hardware for real-world steering angle output.
