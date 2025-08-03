# Indoor Navigation on Husky A200 (Simulation + Real Hardware)

This project demonstrates **end-to-end indoor autonomy** for the **Husky A200** robot, both in simulation and real-world environments, using **ROS 2 Humble** and **Nav2**.  
It includes **online mapping**, **localization**, and **autonomous navigation**, along with **custom Behavior Tree (BT) nodes** for advanced behaviors.

---

## Features
- **Autonomous Navigation**
  - Path planning using **NavFn** global planner
  - Local trajectory control using **DWB Controller**
- **Online SLAM & Localization**
  - **SLAM Toolbox** for real-time mapping
  - **AMCL** for map-based localization
- **Sensor Fusion**
  - Fused IMU and wheel odometry using **robot_localization EKF**
  - Reduced odometry drift by **70%**
- **Custom Behavior Trees**
  - Extended **nav2_bt_navigator** with:
    - **Docking behavior**
    - **Object approach behavior**
    - **Teleoperation fallback**
- **Simulation + Hardware Support**
  - Works in **Gazebo simulation**
  - Deployable on **real Husky A200 hardware**

---

## Tools & Technologies
- ROS 2 Humble
- Nav2 (planner_server, controller_server, bt_navigator)
- SLAM Toolbox
- robot_localization
- Gazebo
- C++ (custom BT nodes)

---

## Project Structure
