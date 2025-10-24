# BEHAVIOR Robot Suite: Streamlining Real-World Whole-Body Manipulation for Everyday Household Activities

## This repository is a fork of the original [BEHAVIOR Robot Suite](https://github.com/behavior-robot-suite/brs-ctrl) repository.

* A 3D printer–friendly version of the JoyLo arms, featuring optimized 3D models for improved printability and easier assembly.

### Changes

* Merged `jcC.obj` and `jcSpace_33mm.obj` into a single `jcC.obj`.
* Adjusted the M2 nut pocket in `jcA.obj` to be tighter to ensure the fit of the nut.
* Added a slight draft and chamfer to the bottom of `jcB.obj` to make the holder easier to insert.
* Reduced the height by 0.9mm from the motor insertion area in `l2.obj`, `l2back.obj`, `l4.obj`, `l5.obj`, and `jcC.obj` so that the motor can be freely moved without the parts touching each other.
* Fixed mesh issues in `l3.obj`.
* Added an alignment key to `l2.obj` and `l2back.obj` to ensure precise alignment during assembly.
* Rotated all parts so they can be printed with the fewest possible supports.

#### Note

* The final dimensions of the JoyLo arms remain unchanged, except for the wrist hinge (if a spacer is inserted).
* If exact dimensions are critical, **do not insert the spacer**.
  * Note that the wrist hinge might damage the cable.

### Printing instructions

* Print all parts, one set per arm.
  * Mirror `jcA.obj` and `jcC.obj` for the right side.

#### Recommended printing parameters

* Material: PLA
* Layer height: 0.2mm
* Outer wall thickness: 0.8mm
* Infill density: 50%
* Infill pattern: Grid or Gyroid
* Supports: Required.

* Do not rotate. Just print as provided.
* Units are in millimeters.

#### Recommended printer setup

* Tested with Bambu X1 Carbon (0.4mm hardened steel nozzle) using BambuStudio as the slicer.
* Filament: Bambu PLA Basic.
* Default 0.20mm Standard profile with the following modifications:
  * Ironing Type: Top surfaces
  * Bottom shell layers: 5
  * Sparse infill density: 50%
  * Sparse infill pattern: Gyroid
  * Enable Support: Yes


### Assembly instructions

* Follow the [Assembly Guide](https://behavior-robot-suite.github.io/docs/sections/joylo/step_by_step_assembly_guidance.html) from the original repository.
* BOM are as following table. (for both arms)

#### 3D Printed Parts

| Part | Source | Description | Count | Notes |
|------|--------|-------------|-------|-------|
| [`mount.obj`](hardware/joylo/mount.obj) | 3D Print | Part from the original repository. | 2 | |
| [`mountback.obj`](hardware/joylo/mountback.obj) | 3D Print | Part from the original repository. | 2 | |
| [`jcA.obj`](hardware/joylo/jcA.obj) | 3D Print | Part from the original repository. | 1 | |
| `jcA.obj` (Mirrored) | 3D Print | Mirror for the right side. | 1 | |
| [`jcB.obj`](hardware/joylo/jcB.obj) | 3D Print | Part from the original repository. | 2 | |
| [`jcC.obj`](hardware/joylo/jcC.obj) | 3D Print | Part from the original repository. | 1 | |
| `jcC.obj` (Mirrored) | 3D Print | Mirror for the right side. | 1 | |
| [`l2.obj`](hardware/joylo/l2.obj) | 3D Print | Part from the original repository. | 2 | |
| [`l2back.obj`](hardware/joylo/l2back.obj) | 3D Print | Part from the original repository. | 2 | |
| [`l3.obj`](hardware/joylo/l3.obj) | 3D Print | Part from the original repository. | 2 | |
| [`l4.obj`](hardware/joylo/l4.obj) | 3D Print | Part from the original repository. | 2 | |
| [`l5.obj`](hardware/joylo/l5.obj) | 3D Print | Part from the original repository. | 2 | |
| [`u2d2_mount.obj`](hardware/joylo/u2d2_mount.obj)| 3D Print | Part from the original repository. | 1 | |
| [`spacer.obj`](hardware/joylo/spacer.obj) |3D Print| Optional spacer for the wrist hinge. | 2 | If the wrist hinge is too tight, insert this spacer for easier assembly. |

#### Miscellaneous Parts

| Part | Description | Count | Notes |
|------|-------------|-------|-------|
| M2 x 12mm bolts | For securing `jcA.obj` to `jcC.obj`. | 4 | |
| M2 nuts | Used with M2 x 12mm bolts to secure `jcA.obj` to `jcC.obj`. | 4 | |
| M2 x 8mm screws | For mounting all motors on their housings. | 24 | |
| M2 x 6mm bolts | For mounting all motors onto rotational axes. | 64 | |
| M2 x 10mm screws | For mounting motors to the wrist hinge. | 4 | |
| M3 x 6mm nylon support (M) | For mounting the u2d2 board. | 4 | |
| M3 nuts | Used with M3 x 6mm nylon support (M) to mount the u2d2 board. | 4 | |

* Note the difference of bolts and screws.

---

<div align="center">

[Yunfan Jiang](https://yunfanj.com/),
[Ruohan Zhang](https://ai.stanford.edu/~zharu/),
[Josiah Wong](https://jdw.ong/),
[Chen Wang](https://www.chenwangjeremy.net/),
[Yanjie Ze](https://yanjieze.com/),
[Hang Yin](https://hang-yin.github.io/),
[Cem Gokmen](https://www.cemgokmen.com/),
[Shuran Song](https://shurans.github.io/),
[Jiajun Wu](https://jiajunwu.com/),
[Li Fei-Fei](https://profiles.stanford.edu/fei-fei-li)

<img src="media/SUSig-red.png" width=200>

**Conference on Robot Learning (CoRL) 2025**

[[Website]](https://behavior-robot-suite.github.io/)
[[arXiv]](https://arxiv.org/abs/2503.05652)
[[PDF]](https://behavior-robot-suite.github.io/assets/pdf/brs_paper.pdf)
[[Doc]](https://behavior-robot-suite.github.io/docs/)
[[Algorithm Code]](https://github.com/behavior-robot-suite/brs-algo)
[[Assembly Guide]](https://behavior-robot-suite.github.io/docs/sections/joylo/step_by_step_assembly_guidance.html)


[![Python Version](https://img.shields.io/badge/Python-3.11-blue.svg)](https://github.com/behavior-robot-suite/brs-ctrl)
[<img src="https://img.shields.io/badge/Doc-Passing-green.svg"/>](https://behavior-robot-suite.github.io/docs/)
[![GitHub license](https://img.shields.io/github/license/behavior-robot-suite/brs-ctrl)](https://github.com/behavior-robot-suite/brs-ctrl/blob/main/LICENSE)

![](media/pull.gif)
______________________________________________________________________
</div>

We introduce the **BEHAVIOR Robot Suite** (BRS), a comprehensive framework for learning whole-body manipulation to tackle diverse real-world household tasks. BRS addresses both hardware and learning challenges through two key innovations: **JoyLo** and [WB-VIMA](https://github.com/behavior-robot-suite/brs-algo).

JoyLo provides a general, cost-effective approach to whole-body teleoperation by integrating multifunctional joystick controllers mounted on the ends of two 3D-printed arms.  The mounting arms serve as scaled-down kinematic twins of the robot’s arms, enabling precise bilateral teleoperation. JoyLo also inherits key advantages of puppeteering devices, including intuitive operation, reduced singularities, and enhanced stability. By grasping the JoyCon controllers attached to the kinematic-twin arms, users can operate the arms, grippers, torso, and mobile base in unison. This significantly accelerates data collection by allowing users to perform bimanual coordination tasks, navigate safely and accurately, and guide the end-effectors to effectively reach various locations in 3D space.

![](media/joylo.gif)

## Getting Started

> [!TIP]
> 🚀 Check out the [doc](https://behavior-robot-suite.github.io/docs/sections/brs_ctrl/overview.html) for detailed installation and usage instructions!

To control the Galaxea R1 robot, simply do

```Python
from brs_ctrl.robot_interface import R1Interface
from brs_ctrl.robot_interface.grippers import GalaxeaR1Gripper

# Initialize the robot interface with grippers
robot = R1Interface(
    left_gripper=GalaxeaR1Gripper(
        left_or_right="left",
        gripper_close_stroke=0.0,
        gripper_open_stroke=100.0,
    ),
    right_gripper=GalaxeaR1Gripper(
        left_or_right="right",
        gripper_close_stroke=0.0,
        gripper_open_stroke=100.0,
    ),
)

# Control the robot
robot.control(
    arm_cmd={
        "left": left_arm_action,  # np (6,)
        "right": right_arm_action,  # np (6,)
    },
    gripper_cmd={
        "left": left_gripper_action,  # float between 0.0 and 1.0
        "right": right_gripper_action,  # float between 0.0 and 1.0
    },
    torso_cmd=torso_action,  # np (4,)
    base_cmd=mobile_base_action,  # np (3,)
)
```

To run real-robot JoyLo control, simply run

```bash
python3 scripts/joylo/real_joylo.py
```

To run data collection, simply run

```bash
python3 scripts/data_collection/start_data_collection.py
```

## Check out Our Paper
Our paper is posted on [arXiv](https://arxiv.org/abs/2503.05652). If you find our work useful, please consider citing us!

```bibtex
@inproceedings{
jiang2025brs,
title={{BEHAVIOR} Robot Suite: Streamlining Real-World Whole-Body Manipulation for Everyday Household Activities},
author={Yunfan Jiang and Ruohan Zhang and Josiah Wong and Chen Wang and Yanjie Ze and Hang Yin and Cem Gokmen and Shuran Song and Jiajun Wu and Li Fei-Fei},
booktitle={9th Annual Conference on Robot Learning},
year={2025},
url={https://openreview.net/forum?id=v2KevjWScT}
}
```

## License
This codebase is released under the [MIT License](LICENSE).
