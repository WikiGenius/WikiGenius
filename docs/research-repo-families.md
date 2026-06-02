# Research Repository Families

This document shows how the public and private repositories should be organized around the research identity.

## Core Rule

Public repositories are portfolio evidence. Private repositories are for unpublished research, datasets, paper-specific code, ablations, and experiments that should not be exposed before publication.

Archived repositories are preserved as history, but they are not part of the active public portfolio.

## Family 1: Structure-Aware Active Scanning

| Repo | Visibility | Role |
|---|---|---|
| [`line-scan-mobile-manipulator-demo`](https://github.com/WikiGenius/line-scan-mobile-manipulator-demo) | Public, pinned | Main public scaffold for line-scan / RGB-hyperspectral active scanning with a mobile manipulator. |
| [`research-reading-map`](https://github.com/WikiGenius/research-reading-map) | Public, pinned | Reading and architecture map for active perception, coverage planning, estimation, and control. |
| Private scanning/paper repos | Private | Exact unpublished algorithms, datasets, calibration, logs, ablations, and paper figures. |

## Family 2: Mobile Manipulation and ROS2 Systems

| Repo | Visibility | Role |
|---|---|---|
| [`ros2-moveit-grasping-demo`](https://github.com/WikiGenius/ros2-moveit-grasping-demo) | Public, pinned | Perception-guided grasping and manipulation execution with ROS2/MoveIt2. |
| [`ros2-mobile-robotics-labs`](https://github.com/WikiGenius/ros2-mobile-robotics-labs) | Public, pinned | ROS2 mobile robotics scaffold for future launch/simulation patterns. |
| [`hello_world_ros2_edx`](https://github.com/WikiGenius/hello_world_ros2_edx) | Public support | Earlier ROS2 learning/migration evidence; do not pin unless expanded. |

## Family 3: State Estimation, SLAM, and 3D Perception

| Repo | Visibility | Role |
|---|---|---|
| [`GTSAM_SLAM_VISION`](https://github.com/WikiGenius/GTSAM_SLAM_VISION) | Public, pinned | Factor-graph visual SLAM and pose-estimation experiments. |
| [`orb_slam_demo`](https://github.com/WikiGenius/orb_slam_demo) | Public support | ROS2 scaffold for ORB-SLAM-style visual state-estimation demos. |
| [`nerf-lab`](https://github.com/WikiGenius/nerf-lab) | Public support | NeRF / ray-based perception lab connected to active viewpoint selection and scene representation. |
| Private estimation/perception repos | Private | Unpublished estimation experiments, private sensor data, and paper-specific results. |

## Family 4: Control, Dynamics, and Robot Math

| Repo | Visibility | Role |
|---|---|---|
| [`robotics-control-learning-labs`](https://github.com/WikiGenius/robotics-control-learning-labs) | Public, pinned | Public control hub for state-space models, LQR, observers, and related support repos. |
| [`ipendulum`](https://github.com/WikiGenius/ipendulum) | Public support | MATLAB/Simulink inverted-pendulum lab with PID, LQR, pole placement, observers, LQG, and demo animations. |
| [`wmm-trajectory-tracking`](https://github.com/WikiGenius/wmm-trajectory-tracking) | Public support | Whole-body mobile-manipulator trajectory tracking. |
| [`RoboticScrewTheoryToolkit`](https://github.com/WikiGenius/RoboticScrewTheoryToolkit) | Public support | Screw theory, Jacobians, inverse kinematics, and robotics math. |
| [`Cruise_control`](https://github.com/WikiGenius/Cruise_control) | Public support | MATLAB/Simulink control and energy/control modeling artifact. |
| Private uncertainty/control repos | Private | Unpublished control studies, paper-specific experiments, ablations, and uncertainty-aware control work. |

Archived control history:

| Repo | Visibility | Role |
|---|---|---|
| [`3dof-robot-arm-report`](https://github.com/WikiGenius/3dof-robot-arm-report) | Archived | Older robot-arm modeling, kinematics, and control report preserved as history. |

## Family 5: Applied CV/AI Prototypes

Keep applied CV/AI prototypes private or archived unless they become polished public demos with a clean README, data policy, runnable example, and relevance to robotics/perception.

Examples that should usually stay private:

- OCR prototypes with private data,
- document/image extraction tools,
- YOLO/TFLite experiments with unclear data rights,
- app/product prototypes unrelated to the robotics research profile.

## Pinning Strategy

Pinned repos should tell a coherent research story:

1. `line-scan-mobile-manipulator-demo` - main research anchor.
2. `ros2-moveit-grasping-demo` - manipulation execution.
3. `GTSAM_SLAM_VISION` - estimation and SLAM.
4. `robotics-control-learning-labs` - control foundations.
5. `ros2-mobile-robotics-labs` - ROS2 systems foundation.
6. `research-reading-map` - theory and architecture map.

Do not pin private repos, forks, old coursework, archived repos, or support repos unless they become polished enough to replace a current pin.

`ipendulum` is now public and belongs under the pinned control hub. It does not need to be pinned separately unless the profile later shifts toward control education as the main signal.

## What To Improve Next

For each pinned repo, aim to add real public-safe evidence as the work matures:

- one runnable minimal example when it exists,
- one figure/GIF/screenshot from real or approved public-safe work,
- one short `docs/` note explaining the method or scope,
- one `results/` artifact only when the result is real and clearly labeled,
- clear limitations saying what is simplified or withheld.

For `ipendulum`, next useful improvements are a controller comparison table, a short state-space derivation note, and a `results/` folder with reproducible metric outputs.
