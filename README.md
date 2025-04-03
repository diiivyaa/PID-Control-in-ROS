# Husky Robot Simulation with PID Control

## Objective

This project involves simulating a Husky robot in an empty Gazebo world with a single pillar using Robot Operating System (ROS). The main goal is to implement a PID controller to guide the Husky robot towards the pillar and make it stop at a predetermined distance, while facing the pillar.

---

## Task Description

1. **Environment Setup**  
   - An empty simulation world is used with a single cylindrical pillar.
   - The pillar has:
     - Height: `2.0` units
     - Diameter: `0.2` units

2. **Robot and Pillar Configuration**  
   - A Husky robot will be used as the mobile platform.
   - The location of the pillar and the mass of the Husky robot will be pre-defined for the simulation.

3. **Simulation Goal**  
   - The Husky robot is expected to:
     1. Navigate towards the pillar using PID control.
     2. Stop at a predetermined distance from the pillar.
     3. Align itself such that it faces the pillar upon stopping.

---

## PID Control Task

You are required to design and implement a **PID (Proportional, Integral, Derivative) controller** for this simulation to:

- Control the velocity of the Husky robot towards the pillar.
- Reduce and eventually eliminate the positional error.
- Maintain stability without oscillations or overshooting.

---

## Deliverables

1. **PID Controller Implementation**  
   Implement the PID algorithm to control the movement of the Husky robot.

2. **PID Tuning**  
   Tune the PID parameters (`Kp`, `Ki`, `Kd`) properly to achieve:
   - Smooth approach
   - Minimal overshoot
   - Precise stopping at the predetermined distance
   - Stable final orientation facing the pillar

3. **Report**  
   Include the following in your report:
   - Explanation of the PID algorithm and its components.
   - Rationale for your chosen PID parameters and tuning process.
   - Analysis of the controller's performance.
   - Any challenges faced during implementation and how you addressed them.

---

## Notes

- The simulation should demonstrate that the robot can consistently approach and stop at the desired distance from the pillar.
- The Husky robot must always face the pillar when stopped.

---

## Recommended Tools

- ROS (Robot Operating System)
- Gazebo Simulator
- RViz (optional, for visualization)
- Python / C++ (for PID implementation)





