# Instance Segmentation and Pose Estimation
This repo presents the work that I've done in Cobot project, funded by Foxconn Interconnect Technology. Due to the confidentiality, I'm unable to provide source code but show some current progress.

## Introduction to Cobot
The goal of this project is to develop capabilities for autonomous, collaborative robots performing tasks in a manufacturing environment. I'm responsible for developing object detection and pose estimation pipeline for small, relective, symmetric USB type-c components. My main contributions are focusing on:
* Improved the performance of self-developed real data labeling tool
* Generated synthetic datasets to train Mask R-CNN, compared with training with real datasets
* Physical simulation experiment to collect stable poses for objects with arbitrary shapes
* Pose estimation based on Augmented Autorencoder.

## Labeling GUI improvements
* Intergrated interactive interface(sliding widgets etc.)
* Improve refresh rate from 3fps to 25fps by optimizing the rendering logic

<p align="center">
  <img src="https://github.com/yangfei4/Sim2real/blob/main/figures/labeling_GUI.jpg" alt="Labeling tool interface" width="500">
</p>

<p align="center">
  <img src="https://github.com/yangfei4/Sim2real/blob/main/figures/rendering_logic.jpg" alt="rendering logic" width="600">
</p>

* Build lable visulization tool
<p align="center">
  <img src="https://github.com/yangfei4/Sim2real/blob/main/figures/checker.jpg" width="600">
</p>
<p align="center">
  <img src="https://github.com/yangfei4/Sim2real/blob/main/figures/vis_logic.jpg" width="600">
</p>

## Synthetic datasets and Mask R-CNN
* Synthetic data examples

<p align="center">
  <img src="https://github.com/yangfei4/Sim2real/blob/main/figures/sythetic_data.jpg" width="400">
</p>

* Augmented synthetic dataset(onging)
<p align="center">
  <img src="https://github.com/yangfei4/Sim2real/blob/main/figures/synthetic.jpg" width="800">
</p>

* Inference of Mask R-CNN (In progress)


## Physical simulation [Link](https://github.com/yangfei4/BlenderProc2_Cobot)
* Experiment collecting 1000 samples
<p align="center">
  <img src="https://github.com/yangfei4/Sim2real/blob/main/figures/physics_positioning.gif" width="600">
</p>

* Experiment result
<p align="center">
  <img src="https://github.com/yangfei4/Sim2real/blob/main/figures/pose_result.jpg" width="800">
</p>

## Pose estimation
<p align="center">
  <img src="https://github.com/yangfei4/Sim2real/blob/main/figures/pvnet_pipeline.jpg?raw=true" width="800">
</p>

See [this repo](https://github.com/yangfei4/clean-pvnet).
