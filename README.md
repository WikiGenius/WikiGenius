# Muhammed Elyamani

**PhD researcher in robotics and control · Perception-aware motion planning**

How should a robot move to obtain the information it needs to accomplish a task?

My research explores how motion planning can account for sensing quality, uncertainty, and task objectives alongside kinematic, dynamic, and collision constraints. The goal is to develop methods that can be adapted to different robots and sensing modalities through their respective models.

RGB-D and hyperspectral sensing are initial application interests. They do not define the scope of the research, and mobile manipulators are one possible platform rather than a requirement.

## The research story

**Observe → estimate → evaluate sensing opportunities → plan → execute → observe again**

The central idea is to connect what a robot needs to know with where and how it moves. Depending on the task, a planner might prioritize visibility, coverage, informative measurements, or reduced uncertainty while balancing motion cost and feasibility.

My public projects build parts of this story. They are separate implementations and learning studies—not yet one integrated, validated perception-aware planning system.

## Start with these projects

| Project | What is implemented | Connection to the research |
| --- | --- | --- |
| [Mobile-manipulator planning and tracking](https://github.com/WikiGenius/wmm-planning-and-tracking) | MATLAB planning, base–arm coordination, torque-level tracking, and simulation/report artifacts | A foundation for generating and executing sensing trajectories |
| [NeRF Lab](https://github.com/WikiGenius/nerf-lab) | Camera geometry, neural density learning, and opacity/depth rendering experiments | Scene representation for studying viewpoint-dependent observations |
| [ROS2 / MoveIt grasping](https://github.com/WikiGenius/ros2-moveit-grasping-demo) | C++ arm/gripper execution, Cartesian approach and retreat, and launch files | Connecting a target pose to robot motion; the full perception stack is external |
| [Screw Theory Toolkit](https://github.com/WikiGenius/RoboticScrewTheoryToolkit) | Python kinematics, Jacobians, and inverse-kinematics utilities | Reachability and geometric reasoning for candidate sensing poses |
| [GTSAM SLAM Vision](https://github.com/WikiGenius/GTSAM_SLAM_VISION) | MATLAB visual pose-estimation and factor-graph experiments | Estimation foundations for planning with uncertain poses |
| [iPendulum](https://github.com/WikiGenius/ipendulum) | PID, state feedback, observers, and MATLAB/Simulink demonstrations | Control and estimation foundations for reliable execution |

The linked repositories describe their requirements and limitations. Included figures are project artifacts; their presence alone does not establish reproducibility or hardware validation.

## Explore by research role

| Role | Repositories | Current scope |
| --- | --- | --- |
| Motion planning and control | [WMM planning and tracking](https://github.com/WikiGenius/wmm-planning-and-tracking), [UGV–Panda geometric control](https://github.com/WikiGenius/ugv-panda-geometric-control) | Simulation implementations. UGV–Panda has a documented Jacobian defect pending correction |
| Estimation and scene representation | [GTSAM SLAM Vision](https://github.com/WikiGenius/GTSAM_SLAM_VISION), [NeRF Lab](https://github.com/WikiGenius/nerf-lab) | Research/learning prototypes, not complete SLAM systems |
| Robot geometry and execution | [Screw Theory Toolkit](https://github.com/WikiGenius/RoboticScrewTheoryToolkit), [MoveIt grasping](https://github.com/WikiGenius/ros2-moveit-grasping-demo) | Kinematic utilities and a robot-specific manipulation demo |
| Sensing and data collection | [Husky image capture](https://github.com/WikiGenius/husky-gazebo-image-capture), [traffic-sign detection](https://github.com/WikiGenius/ros-husky-traffic-sign-detection) | ROS2 image/odometry capture and a legacy ROS 1 perception demo |
| Control foundations | [iPendulum](https://github.com/WikiGenius/ipendulum), [Cruise Control](https://github.com/WikiGenius/Cruise_control) | Focused educational control and simulation studies |
| Reading and navigation | [Research reading map](https://github.com/WikiGenius/research-reading-map), [control hub](https://github.com/WikiGenius/robotics-control-learning-labs), [ROS hub](https://github.com/WikiGenius/ros2-mobile-robotics-labs) | Reading structure and project indexes; not standalone experimental results |

## From components to a research contribution

The next step is to couple sensing objectives with motion decisions and evaluate the resulting trade-offs against explicit baselines. Sensor observation models and robot constraints will be chosen for each application; a common planning idea does not imply identical models for every platform.

[Line-scan mobile-manipulator demo](https://github.com/WikiGenius/line-scan-mobile-manipulator-demo) is an early application scaffold for scanning and coverage experiments. It currently has no complete runnable demo. It is one possible test case for the broader research direction.

## Earlier work and collaboration

Archived computer-vision applications such as [StreetStat](https://github.com/WikiGenius/StreetStat) and [CrowdScope](https://github.com/WikiGenius/CrowdScope), course exercises, and upstream forks document earlier work. They support the learning history rather than serving as completed PhD contributions.

I welcome collaboration on planning, estimation, sensing models, and reproducible robotics experiments. Open an issue in the relevant project to discuss technical work. Each repository retains its own scope, validation status, and license terms.

**Tools:** Python, C++, MATLAB/Simulink, ROS2, MoveIt2, Gazebo, GTSAM, and PyTorch.

Unpublished manuscripts, confidential data, and collaborator feedback are kept private until approved for release.
