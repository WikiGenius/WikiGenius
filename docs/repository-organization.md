# Repository Organization Map

This document organizes the GitHub account around the research identity:

> Structure-aware planning and control for mobile manipulation, where robot motion is designed not only to reach a target but also to actively acquire useful visual or spectral information under physical, geometric, sensing, and uncertainty constraints.

The account has two layers:

1. **Private research layer** - unpublished algorithms, datasets, experiments, paper drafts, and sensitive research code.
2. **Public portfolio layer** - polished evidence that demonstrates capability without leaking publishable novelty.

## Current Public Shape

The public active repository set is intentionally focused. Archived repositories are preserved as history, references, or old learning work, but they are not part of the main public research story.

Current active public repositories:

| Repo | Role |
|---|---|
| `WikiGenius` | Profile README and organization map. |
| `line-scan-mobile-manipulator-demo` | Main public scaffold for structure-aware line-scan / RGB-hyperspectral active scanning. |
| `ros2-moveit-grasping-demo` | ROS2 / MoveIt2 perception-guided grasping and mobile-manipulation execution evidence. |
| `GTSAM_SLAM_VISION` | Factor-graph visual SLAM and state-estimation evidence. |
| `robotics-control-learning-labs` | Public control-foundation lab scaffold and pinned control hub. |
| `ipendulum` | Public inverted-pendulum MATLAB/Simulink support lab for PID, LQR, observers, LQG, and animations. |
| `ros2-mobile-robotics-labs` | Public ROS2 mobile-robotics learning scaffold. |
| `research-reading-map` | Research reading map for active perception, coverage planning, estimation, and control. |
| `wmm-trajectory-tracking` | Public trajectory-tracking / control support artifact. |
| `RoboticScrewTheoryToolkit` | Robotics math, screw theory, kinematics, and Jacobian support artifact. |
| `Cruise_control` | MATLAB/Simulink control and mobile-robot energy artifact. |
| `3dof-robot-arm-report` | LaTeX technical report for robot-arm modeling and control. |
| `nerf-lab` | NeRF / neural mapping support lab for 3D perception and SLAM intuition. |
| `orb_slam_demo` | ROS2 scaffold for ORB-SLAM-style visual state-estimation demos. |
| `hello_world_ros2_edx` | ROS2 Humble migration/learning evidence from ROS1 course concepts. |

## Public vs Private Rule

### Keep Private

Use private repositories for:

- unpublished paper implementations,
- novel planning/control algorithms before submission,
- raw RGB/hyperspectral datasets,
- experiment logs, ablation studies, and parameter sweeps,
- internal notes, drafts, figures, and reviewer-response work,
- code that reveals the exact method before publication,
- applied CV/AI prototypes that include private data, client work, or unfinished product ideas.

Suggested private naming pattern:

```text
paper-structure-aware-line-scan-planning
private-hsi-mobile-manipulator-data
private-active-scanning-experiments
private-uncertainty-aware-control
private-paper-figures-and-logs
```

### Make Public

Use public repositories for:

- simplified demos,
- reproducible labs,
- portfolio evidence,
- course-derived work with attribution,
- technical reports after cleanup,
- reading maps and paper lists,
- selected results that do not reveal unpublished details.

Suggested public naming pattern:

```text
line-scan-mobile-manipulator-demo
ros2-moveit-grasping-demo
robotics-control-learning-labs
ros2-mobile-robotics-labs
research-reading-map
```

## Public Portfolio Pillars

### 1. Active Scanning / Coverage Planning

This is the main research identity.

| Repo | Status | Action |
|---|---|---|
| `line-scan-mobile-manipulator-demo` | Public core, pinned | Add simplified planner, figures, demo GIF, and public metrics. |
| `research-reading-map` | Public core, pinned | Add paper taxonomy for active perception, coverage planning, and state estimation. |

Keep unpublished HSI/RGB scanning code private until paper-ready.

### 2. Mobile Manipulation Execution

This proves the robot execution layer.

| Repo | Status | Action |
|---|---|---|
| `ros2-moveit-grasping-demo` | Public core, pinned | Add launch workflow, perception interface diagram, screenshots, and execution metrics. |
| `ros2-mobile-robotics-labs` | Public core, pinned | Add ROS2 labs that support the main research direction. |
| `hello_world_ros2_edx` | Public support | Keep as learning/migration evidence. Do not pin. |

Legacy ROS/perception projects are archived until they are polished into public-safe portfolio artifacts.

### 3. State Estimation / SLAM / Uncertainty

This supports the estimation part of the research program.

| Repo | Status | Action |
|---|---|---|
| `GTSAM_SLAM_VISION` | Public core, pinned | Add figures, reproducible sample, and factor graph notes. |
| `orb_slam_demo` | Public support | Add launch/demo workflow when ready. |
| `nerf-lab` | Public support | Add toy rendering examples and 3D perception notes. |

Reference forks for SLAM, RealSense, GTSAM, and related tooling are archived unless actively maintained.

### 4. Control / Dynamics / Robotics Math

This proves the control foundation.

| Repo | Status | Action |
|---|---|---|
| `robotics-control-learning-labs` | Public core, pinned | Add reproducible LQR/observer examples and link focused public control artifacts. |
| `ipendulum` | Public support | Add controller comparison table, state-space derivation note, and reproducible metric outputs. |
| `wmm-trajectory-tracking` | Public support | Add minimal reproducible trajectory-tracking example and plots. |
| `RoboticScrewTheoryToolkit` | Public support | Add examples/results; consider renaming to `robotic-screw-theory-toolkit`. |
| `Cruise_control` | Public support | Add model diagram and metrics. |
| `3dof-robot-arm-report` | Public support | Add compiled PDF release and key figures. |

Unpublished uncertainty-aware control studies, internal ablations, and paper-specific results remain private.

### 5. Computer Vision / AI Prototypes

Applied CV/AI prototypes are useful background, but they should not dominate the robotics profile. Keep them private or archived unless they become polished portfolio demos with clean READMEs, data policy, and reproducible examples.

### 6. Forks and Reference Repositories

Public forks are archived by default. This keeps the profile focused on original research artifacts. Archived forks remain available as history/reference but do not compete with the active portfolio.

Recommended policy:

- Archive unmodified forks.
- Keep only forks that contain useful original changes or are active dependencies.
- Never pin forks unless they contain a significant original contribution.
- If a fork becomes important to the research pipeline, document why in the relevant public repo.

### 7. Old Learning / Coursework / General Programming

Old learning/coursework repositories are archived. They remain preserved, but the active public profile should emphasize current research identity rather than early learning history.

## Pinning Strategy

Pinned repositories:

1. `line-scan-mobile-manipulator-demo`
2. `ros2-moveit-grasping-demo`
3. `GTSAM_SLAM_VISION`
4. `robotics-control-learning-labs`
5. `ros2-mobile-robotics-labs`
6. `research-reading-map`

`ipendulum` is now public and should remain a linked support repo under the pinned control hub unless the future pinning strategy changes.

## Naming Strategy

Use lowercase kebab-case for future public repos:

```text
line-scan-mobile-manipulator-demo
structure-aware-scanning-planner
uncertainty-aware-mobile-manipulation
ros2-active-scanning-demo
factor-graph-visual-estimation
mobile-manipulator-control-labs
```

Avoid future names like:

```text
project_node
code
README
NewProject
research_project
```

## Topics to Use

Use these topics across public portfolio repositories:

```text
mobile-manipulation
active-perception
structure-aware-planning
coverage-planning
line-scan
hyperspectral-imaging
rgb-d
state-estimation
factor-graphs
slam
uncertainty-aware-control
ros2
moveit2
gazebo
matlab
simulink
robotics-control
```

## Release Path From Private to Public

When a paper or experiment is ready to expose:

1. Keep the full research repository private.
2. Create a simplified public demo repository.
3. Remove sensitive datasets, exact unpublished ablations, and private notes.
4. Add `README.md`, `LICENSE` or notice, `docs/`, `src/`, `results/`, `media/`.
5. Include a small reproducible example or synthetic data.
6. Add figures/GIFs that communicate the method without leaking protected details.
7. Link the paper/report only after submission/preprint/publication is appropriate.

## Cleanup Status

- [x] Added topics to the six pinned repositories.
- [x] Added aligned descriptions to core and support repositories.
- [x] Archived unmodified/unneeded public forks.
- [x] Archived old coursework and early learning repositories.
- [x] Added READMEs to active public support repositories that were missing or empty.
- [x] Released `ipendulum` as a public control-support repository.
- [x] Kept unpublished/private-data repositories private.
- [x] Reduced active public repositories to a focused portfolio set.
- [ ] Add real figures, GIFs, metrics, and reports to the active public repositories as experiments mature.
