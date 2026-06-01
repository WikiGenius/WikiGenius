# Repository Organization Map

This document organizes the GitHub account around the research identity:

> Structure-aware planning and control for mobile manipulation, where robot motion is designed not only to reach a target but also to actively acquire useful visual or spectral information under physical, geometric, sensing, and uncertainty constraints.

The account has two layers:

1. **Private research layer** - unpublished algorithms, datasets, experiments, paper drafts, and sensitive research code.
2. **Public portfolio layer** - polished evidence that demonstrates capability without leaking publishable novelty.

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
| `line-scan-mobile-manipulator-demo` | Public core | Keep pinned. Add simplified planner, figures, demo GIF, and public metrics. |
| `research-reading-map` | Public core | Keep pinned. Add paper taxonomy for active perception, coverage planning, and state estimation. |

Keep unpublished HSI/RGB scanning code private until paper-ready.

### 2. Mobile Manipulation Execution

This proves the robot execution layer.

| Repo | Status | Action |
|---|---|---|
| `ros2-moveit-grasping-demo` | Public core | Keep pinned. Add launch workflow, screenshots, and execution metrics. |
| `ros2-mobile-robotics-labs` | Public core | Keep pinned. Add ROS2 labs that support the main research direction. |
| `hello_world_ros2_edx` | Public support | Keep public as learning/migration evidence. Do not pin. |
| `ros_project` | Legacy support | Either polish as legacy ROS perception/autonomy demo or archive. |

### 3. State Estimation / SLAM / Uncertainty

This supports the estimation part of the research program.

| Repo | Status | Action |
|---|---|---|
| `GTSAM_SLAM_VISION` | Public core | Keep pinned. Add figures, reproducible sample, and factor graph notes. |
| `orb_slam_demo` | Public support | Add README and clarify relation to state estimation. |
| `nerf-lab` | Public support | Add README and clarify relation to neural mapping / 3D perception. |
| `NeRF-SLAM` | Fork/reference | Keep only if actively used; otherwise archive as reference. |
| `gtsam` | Fork/reference | Keep only if modified; otherwise archive or leave unpinned. |
| `factor-graphs-course` | Fork/reference | Keep as study reference, not portfolio evidence. |
| `realsense-ros`, `realsense2_description`, `realsense_gazebo_plugin` | Fork/reference | Keep if used in scanning pipeline; otherwise archive/unpin. |

### 4. Control / Dynamics / Robotics Math

This proves the control foundation.

| Repo | Status | Action |
|---|---|---|
| `robotics-control-learning-labs` | Public core | Keep pinned until a stronger research-control artifact is polished. |
| `wmm-trajectory-tracking` | High-value support | Keep public only if it is a simplified portfolio artifact; keep private if it contains unpublished methods/results. |
| `RoboticScrewTheoryToolkit` | High-value support | Rename to `robotic-screw-theory-toolkit`; add examples/results. |
| `Cruise_control` | Public support | Add README/results and relate to mobile robot control. |
| `3dof-robot-arm-report` | Public support | Add report PDF, abstract, and figures if available. |

### 5. Computer Vision / AI Prototypes

These support the perception background but should not dominate the robotics profile.

| Category | Status | Action |
|---|---|---|
| OCR / document-understanding prototypes | Private or polished public | Keep private unless cleaned as applied-CV portfolio demos. |
| YOLO / TFLite deployment experiments | Mixed | Keep private or public only if documented as deployment experiments. |
| Crowd/street/search/product prototypes | Public/product | Move into an Applied AI / CV prototypes section if polished; otherwise archive. |
| Domain-specific segmentation or medical-imaging utilities | Mixed | Keep public only if documented; otherwise archive/private. |

### 6. Forks and Reference Repositories

Most forks should not be part of the visible research story.

Examples:

```text
opencv, dlib, darknet, yolov5, YOLOX, YOLOX-ROS, Open3D,
apollo, carla, husky, gazebo_models, Deep_Object_Pose,
KivyMD, kivy, transformers, openai-cookbook, llama
```

Recommended policy:

- Archive unmodified forks.
- Keep only forks that contain useful changes or are active dependencies.
- Never pin forks unless they contain a significant original contribution.
- Add a note in the profile that forks are kept as references/dependencies.

### 7. Old Learning / Coursework / General Programming

These show learning history but dilute the current research identity.

Examples:

```text
Basic-algorithms, Data_Structures, recover, neural_network,
learning-curve, finding_donors, route-planner-algorithms,
SQL_projects, Python, C-Plus-Plus, javascript-algorithms,
19_udacity_dsa, DSND_Term1, aipnd-project
```

Recommended policy:

- Archive most of these.
- Keep public only if they are cleaned and useful as teaching artifacts.
- Do not pin.
- Consider consolidating into a single `learning-archive` repository if desired.

## Pinning Strategy

Recommended pinned repositories:

1. `line-scan-mobile-manipulator-demo`
2. `ros2-moveit-grasping-demo`
3. `GTSAM_SLAM_VISION`
4. `robotics-control-learning-labs` for now; later replace with a polished research-control artifact if appropriate
5. `ros2-mobile-robotics-labs`
6. `research-reading-map`

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

Apply these topics to public portfolio repositories:

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

## Immediate Cleanup Checklist

- [ ] Add topics to the six pinned repositories.
- [ ] Polish `wmm-trajectory-tracking` README and decide whether it should remain public.
- [ ] Add README files to `orb_slam_demo` and `nerf-lab`.
- [ ] Archive unmodified forks that are not actively used.
- [ ] Archive or hide old coursework repositories.
- [ ] Keep private all unpublished structure-aware scanning, hyperspectral, uncertainty-control, and paper-specific repositories.
- [ ] Use public repos only as evidence, not as the full research lab notebook.
