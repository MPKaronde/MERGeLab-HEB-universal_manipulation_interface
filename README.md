# MERGeLab HEB-Universal Manipulation Interface

## Modifications from Original UMI SLAM Pipeline
* We use a GoPro Hero 12 Black with the Max Lense Mod 2.0. Our calibration results for this can be found under example/calibration_hero12, while the original Hero 10 setup remains in example/calibration
* We modified the SLAM scripts to no longer use a hardcoded calibration. Running 02_create_map.py and 03_batch_slam.py with the -s flag allows you to pass a path to a camera calibration YAML. Running the run_slam_pipeline.py with -c and a path to the calibration directory will auto run the aforementioned files with -s and the entire rest of the pipeline with the generated outputs.

## Based on Original UMI project:
[[Project page]](https://umi-gripper.github.io/)
[[Paper]](https://umi-gripper.github.io/#paper)
[[Hardware Guide]](https://docs.google.com/document/d/1TPYwV9sNVPAi0ZlAupDMkXZ4CA1hsZx7YDMSmcEy6EU/edit?usp=sharing)
[[Data Collection Instruction]](https://swanky-sphere-ad1.notion.site/UMI-Data-Collection-Tutorial-4db1a1f0f2aa4a2e84d9742720428b4c?pvs=4)
[[SLAM repo]](https://github.com/cheng-chi/ORB_SLAM3)
[[SLAM docker]](https://hub.docker.com/r/chicheng/orb_slam3)
[Cheng Chi](http://cheng-chi.github.io/)<sup>1,2</sup>,
[Zhenjia Xu](https://www.zhenjiaxu.com/)<sup>1,2</sup>,
[Chuer Pan](https://chuerpan.com/)<sup>1</sup>,
[Eric Cousineau](https://www.eacousineau.com/)<sup>3</sup>,
[Benjamin Burchfiel](http://www.benburchfiel.com/)<sup>3</sup>,
[Siyuan Feng](https://www.cs.cmu.edu/~sfeng/)<sup>3</sup>,

[Russ Tedrake](https://groups.csail.mit.edu/locomotion/russt.html)<sup>3</sup>,
[Shuran Song](https://www.cs.columbia.edu/~shurans/)<sup>1,2</sup>

<sup>1</sup>Stanford University,
<sup>2</sup>Columbia University,
<sup>3</sup>Toyota Research Institute

## 🏷️ License
This repository is released under the MIT license. See [LICENSE](LICENSE) for additional details.

## 🙏 Acknowledgement
* This repository is a fork of the original UMI project and draws heavily from it https://github.com/real-stanford/universal_manipulation_interface
* The original UMI GoPro SLAM pipeline is adapted from [Steffen Urban](https://github.com/urbste)'s [fork](https://github.com/urbste/ORB_SLAM3) of [OBR_SLAM3](https://github.com/UZ-SLAMLab/ORB_SLAM3).
* We used [Steffen Urban](https://github.com/urbste)'s [OpenImuCameraCalibrator](https://github.com/urbste/OpenImuCameraCalibrator/) for camera and IMU calibration.
* The HEB gripper's shell and core mechanism are adapted from the original UMI design at https://cad.onshape.com/documents/a8a98201374f5cc9c6538790
