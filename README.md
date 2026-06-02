# Muhammed Elyamani

PhD researcher in Electrical Engineering at KFUPM working on robotics, control, motion planning, and state estimation for mobile manipulation.

My research focuses on **structure-aware planning and control for mobile manipulation**, where robot motion is designed not only to reach a target but also to actively acquire useful visual or spectral information under physical, geometric, sensing, and uncertainty constraints.

The initial application is **line-scan-inspired RGB / hyperspectral scanning using a mobile manipulator**, with extensions toward state estimation, coverage planning, and uncertainty-aware control.

## Research Identity

I am building a research program around robot motion that connects:

- active visual and spectral scanning,
- mobile manipulation and whole-body motion planning,
- coverage and viewpoint planning,
- geometric and sensing constraints,
- factor-graph state estimation and visual SLAM,
- control under uncertainty.

The public GitHub profile is organized as a portfolio of evidence. Public repositories demonstrate methods, engineering skill, reproducible workflows, and learning artifacts. Private repositories hold unpublished research code, datasets, experiments, and paper-specific implementations until they are ready for release.

## Current Research Direction

### Structure-Aware Active Scanning

The goal is to plan mobile manipulator motion that improves information acquisition, not just task completion. The robot should reason about what it can see, what it still needs to cover, how the sensor geometry affects measurement quality, and how robot kinematics or uncertainty constrain the scan.

Key constraints include:

- line-scan / push-broom sensing geometry,
- RGB and hyperspectral visual information,
- camera visibility and viewing angle,
- surface coverage and scan quality,
- robot reachability and base-arm coordination,
- collision avoidance and physical limits,
- pose uncertainty and estimation quality.

## Public Portfolio Pillars

### Active Scanning and Coverage Planning

- [`line-scan-mobile-manipulator-demo`](https://github.com/WikiGenius/line-scan-mobile-manipulator-demo) - public scaffold for line-scan-aware active scanning with a mobile manipulator.
- [`research-reading-map`](https://github.com/WikiGenius/research-reading-map) - reading and architecture map for mobile manipulation, active perception, coverage planning, state estimation, and control.

### Mobile Manipulation Execution

- [`ros2-moveit-grasping-demo`](https://github.com/WikiGenius/ros2-moveit-grasping-demo) - ROS2 / MoveIt2 perception-guided grasping with object localization, Cartesian approach, gripper control, and retreat planning.
- [`ros2-mobile-robotics-labs`](https://github.com/WikiGenius/ros2-mobile-robotics-labs) - ROS2 Humble learning labs for mobile robotics workflows.

### State Estimation, SLAM, and 3D Perception

- [`GTSAM_SLAM_VISION`](https://github.com/WikiGenius/GTSAM_SLAM_VISION) - visual pose estimation and factor-graph SLAM experiments in MATLAB.
- [`orb_slam_demo`](https://github.com/WikiGenius/orb_slam_demo) - ROS2 scaffold for ORB-SLAM-style visual state-estimation demos.
- [`nerf-lab`](https://github.com/WikiGenius/nerf-lab) - NeRF / ray-based perception lab for view synthesis, 3D representation, and active-perception intuition.

### Control and Robotics Foundations

- [`robotics-control-learning-labs`](https://github.com/WikiGenius/robotics-control-learning-labs) - reproducible control labs for state-space modeling, LQR, observers, and MATLAB/Simulink.
- [`ipendulum`](https://github.com/WikiGenius/ipendulum) - MATLAB/Simulink inverted-pendulum lab with PID, LQR, pole placement, observers, LQG, and demo animations.
- [`wmm-trajectory-tracking`](https://github.com/WikiGenius/wmm-trajectory-tracking) - whole-body mobile-manipulator trajectory tracking support.
- [`RoboticScrewTheoryToolkit`](https://github.com/WikiGenius/RoboticScrewTheoryToolkit) - screw theory, Jacobians, and robot kinematics foundations.
- [`Cruise_control`](https://github.com/WikiGenius/Cruise_control) and [`3dof-robot-arm-report`](https://github.com/WikiGenius/3dof-robot-arm-report) - supporting control/report artifacts.

## Public vs Private Policy

**Public repositories** are for:

- portfolio evidence,
- simplified demos,
- reproducible labs,
- course-derived work with attribution,
- polished technical reports,
- reading maps and non-sensitive notes.

**Private repositories** are for:

- unpublished paper implementations,
- novel algorithms before submission,
- raw datasets and experiment logs,
- hyperspectral/RGB data that may have sharing limits,
- parameter sweeps and ablation studies,
- drafts, figures, and reviewer-response experiments,
- unpublished uncertainty-aware control experiments that are not ready for public release.

When research is ready, a private repository can be distilled into a public release repo with a clean README, citation, license/notice, reproducible scripts, selected results, and a paper/report link.

## Technical Stack

**Robotics:** ROS2, MoveIt2, Gazebo, RViz  
**Control:** MATLAB, Simulink, state-space control, LQR, observers  
**Estimation:** GTSAM, factor graphs, visual pose estimation, SLAM  
**Perception:** RGB, hyperspectral / line-scan-inspired sensing, computer vision, NeRF/view synthesis  
**Programming:** Python, C++, MATLAB  
**Research Tools:** LaTeX, Git, experiment logs, paper reading maps

## Current Goal

Convert learning and implementation work into a coherent research portfolio:

- private publishable research repos,
- public portfolio evidence repos,
- reproducible demos and labs,
- clean READMEs and result folders,
- technical reports and paper links,
- a clear path from robotics theory to runnable systems.

See [`docs/repository-organization.md`](docs/repository-organization.md) for the repository organization map and [`docs/research-repo-families.md`](docs/research-repo-families.md) for the cross-repo family structure.
