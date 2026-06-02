# Muhammed Elyamani

PhD Researcher in Robotics and Control focusing on structure-aware planning, state estimation, and active sensing for mobile manipulation.

<p align="center">
  <img src="assets/research_banner.png" alt="Conceptual research banner showing mobile manipulation, line-scan active sensing, coverage planning, and state estimation" width="100%">
</p>

> Conceptual research banner illustrating my current PhD direction. It is a visual summary, not an experimental result.

My current research direction studies active line-scan / one-row RGB scanning for mobile manipulators, where the robot must satisfy visibility, coverage, kinematic, collision, and uncertainty constraints during scanning and inspection tasks.

## Research Identity

- Robotics and control
- Mobile manipulation
- Motion planning
- State estimation
- Active sensing
- ROS2 / MoveIt2 / GTSAM

## Current Research Direction

### Structure-Aware Active Scanning

The goal is to plan mobile manipulator motion that improves information acquisition, not just task completion.

Key constraints include:

- line-scan / pushbroom sensing geometry,
- RGB and hyperspectral visual information,
- camera visibility and viewing angle,
- surface coverage and scan quality,
- robot reachability and base-arm coordination,
- collision avoidance and physical limits,
- pose uncertainty and estimation quality.

## Main Public Research Repositories

| Repository | Role |
|---|---|
| [`line-scan-mobile-manipulator-demo`](https://github.com/WikiGenius/line-scan-mobile-manipulator-demo) | Public scaffold for future line-scan active-scanning experiments. |
| [`ros2-moveit-grasping-demo`](https://github.com/WikiGenius/ros2-moveit-grasping-demo) | ROS2/MoveIt2 manipulation demo with object localization, Cartesian approach, gripper control, and retreat planning. |
| [`GTSAM_SLAM_VISION`](https://github.com/WikiGenius/GTSAM_SLAM_VISION) | MATLAB state-estimation and factor-graph visual SLAM experiments. |
| [`robotics-control-learning-labs`](https://github.com/WikiGenius/robotics-control-learning-labs) | Control foundations and public learning-lab scaffold. |
| [`ros2-mobile-robotics-labs`](https://github.com/WikiGenius/ros2-mobile-robotics-labs) | ROS2 mobile robotics scaffold for future labs. |
| [`research-reading-map`](https://github.com/WikiGenius/research-reading-map) | Public reading map, research architecture, and paper-note templates. |

## Public / Private Research Boundary

Public repositories are for sanitized portfolio evidence, educational examples, toy demos, and reproducible non-confidential artifacts.

Private repositories hold unpublished research code, real experiment logs, private datasets, advisor feedback, ablation plans, paper drafts, and collaboration-sensitive notes until release is appropriate.

## Current Goal

Convert learning into visible research artifacts: clean repositories, experiment logs, plots, demos, reports, and eventually paper submissions.

## Supporting Repositories

| Repository | Role |
|---|---|
| [`ipendulum`](https://github.com/WikiGenius/ipendulum) | Inverted-pendulum MATLAB/Simulink control lab. |
| [`wmm-trajectory-tracking`](https://github.com/WikiGenius/wmm-trajectory-tracking) | Whole-body mobile-manipulator trajectory tracking support. |
| [`RoboticScrewTheoryToolkit`](https://github.com/WikiGenius/RoboticScrewTheoryToolkit) | Screw theory, Jacobians, and robot kinematics foundations. |
| [`Cruise_control`](https://github.com/WikiGenius/Cruise_control) | MATLAB/Simulink control support artifact. |
| [`nerf-lab`](https://github.com/WikiGenius/nerf-lab) | NeRF / ray-based perception support lab for active-perception intuition. |
| [`orb_slam_demo`](https://github.com/WikiGenius/orb_slam_demo) | ROS2 scaffold for ORB-SLAM-style visual state-estimation demos. |

## Technical Stack

**Robotics:** ROS2, MoveIt2, Gazebo, RViz  
**Control:** MATLAB, Simulink, state-space control, LQR, observers  
**Estimation:** GTSAM, factor graphs, visual pose estimation, SLAM  
**Perception:** RGB, hyperspectral / line-scan-inspired sensing, computer vision, NeRF/view synthesis  
**Programming:** Python, C++, MATLAB  

See [`docs/repository-organization.md`](docs/repository-organization.md) for the repository organization map and [`docs/research-repo-families.md`](docs/research-repo-families.md) for the cross-repo family structure.
