# ABS on Go2

An independent engineering reproduction of Agile But Safe (ABS), adapting the original Unitree Go1 pipeline to Unitree Go2 and validating the Agile Policy in simulation and on hardware.

## Migration Workflow

1. **Go1-to-Go2 model adaptation:** Replaced the robot model and updated joint ordering, action mapping, observation dimensions, PD gains, and actuator limits for Go2.

2. **Perception and state integration:** Converted Intel RealSense D435i depth observations into forward distance rays, integrated Livox MID360 LiDAR observations for the side and rear regions, and connected LIO-based state estimation.

3. **Simulation training and policy export:** Trained and validated the Go2 Agile Policy in Isaac Gym, then exported the trained policy to ONNX for onboard inference.

4. **Go2 deployment:** Adapted the control pipeline to Unitree SDK2/DDS, connected policy inference to low-level PD joint control, and deployed the runtime on NVIDIA Jetson Orin NX.

5. **Real-to-Sim calibration:** Used real-robot feedback to refine sensor payload mass and inertia, control and perception latency, localization noise, and motor torque-speed constraints in simulation.

## Demonstrations

The project page presents four qualitative Agile Policy rollouts on Unitree Go2 and four Isaac Gym rollouts. The published real-robot demonstrations focus on the Agile Policy deployment path and are not reported as statistical success-rate measurements.

## References

- Original ABS project: [https://agile-but-safe.github.io/](https://agile-but-safe.github.io/)
- Official ABS code: [https://github.com/LeCAR-Lab/ABS](https://github.com/LeCAR-Lab/ABS)

This repository documents an independent reproduction and platform adaptation. The original ABS method and project remain the work of their respective authors.
