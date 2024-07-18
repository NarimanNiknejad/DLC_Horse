# Equine Kinematic Gait Analysis Dataset

## Overview
This dataset contains annotated keypoints for equine kinematic gait analysis using stereo videography and deep learning techniques. It was developed as part of the research paper titled "Equine Kinematic Gait Analysis Using Stereo Videography and Deep Learning: Stride Length and Stance Duration Estimation," published in the Journal of the ASABE.

## Video Demonstration

[![Watch the video](https://img.youtube.com/vi/YixcEN6iN8o/0.jpg)](https://youtu.be/YixcEN6iN8o)

## Highlights
- Stereo machine vision and deep learning techniques were investigated for infield equine kinematic gait analysis.
- The proposed pipeline tracks equine body landmarks in 3D space and estimates stride length and stance duration.
- The system can serve as a cost-effective, rapid, and easy-to-use tool for equine locomotion research.

## Dataset Description
The dataset includes stereo videos of different walking horses. A DeepLabCut (DLC) model was trained to detect body landmarks in individual frames. The keypoints include various body parts essential for gait analysis.

### Keypoints
The annotated keypoints are as follows:
- Hoof
- Fetlock
- Knee
- Hock
- Nostril
- Poll
- Wither
- Hip

### Data Collection
- **Camera**: RGB stereo camera (ZED2, STEREOLABS, France)
- **Resolution**: 2208 × 1242 pixels
- **Frame Rate**: 15 frames per second (FPS)
- **Location**: Auburn University Equestrian Center, Auburn, Alabama, USA
- **Date**: July 2021

### Horse Information
- **Breeds**: Warmbloods, Morgans, Quarter Horses, Thoroughbreds
- **Lighting Conditions**: Sunny, cloudy, overcast, backlit
- **Diagnoses**: Some horses diagnosed with lameness

## Pipeline
The data processing pipeline consists of three main modules:
1. **Body Landmark Detection**: Using DLC for detecting body landmarks in 2D frames.
2. **Hoof Gait Phase Detection**: Using Faster R-CNN to detect hoof phases (stance, swing, occluded).
3. **Stereo 3D Reconstruction**: Using a semi-global block matching (SGBM) algorithm to estimate 3D coordinates of the landmarks.

## Citation
Researchers can use this dataset to develop and evaluate their own equine gait analysis systems. When using this dataset, please cite the following paper:

@article{niknejad2023equine,
  title={Equine kinematic gait analysis using stereo videography and deep learning: stride length and stance duration estimation},
  author={Niknejad, Nariman and Caro, Jessica L and Bidese-Puhl, Rafael and Bao, Yin and Staiger, Elizabeth A},
  year={2023},
  publisher={American Society of Agricultural and Biological Engineers}
}


## Introduction to DeepLabCut

DeepLabCut is an open-source toolbox that utilizes deep learning to enable markerless pose estimation of animals (or humans) performing various tasks. It is particularly well-suited for applications in biomechanics, neuroscience, ethology, and behavioral research. DeepLabCut achieves state-of-the-art performance by leveraging deep convolutional neural networks (CNNs) to detect body landmarks in video frames with high accuracy.

## Getting Started with DeepLabCut

To get started with DeepLabCut and use it with the provided custom dataset, follow the steps below:

### Prerequisites

Ensure you have the following software installed:
- Python 3.6 or higher
- TensorFlow (version 1.13 or later)
- DeepLabCut (latest version)
  
[DeepLabCut User Guide](https://deeplabcut.github.io/DeepLabCut/docs/standardDeepLabCut_UserGuide.html)


