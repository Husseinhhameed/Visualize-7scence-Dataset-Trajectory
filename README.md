# 7Scenes Dataset Trajectory Visualization

This repository contains code for visualizing the trajectories of sequences from the [7Scenes Dataset](https://www.microsoft.com/en-us/research/project/rgb-d-dataset-7-scenes/). The visualization helps in analyzing the camera poses and movement paths across the dataset sequences.


## Project Overview

This project is divided into three major visualization parts:
1. **Single Plot for All Sequences**: All the sequences are plotted together on a single 3D plot to provide an overall visualization of the entire dataset.
2. **Colored Plot for Each Sequence**: All sequences are plotted on the same 3D plot, but each sequence is represented with a different color to distinguish between them.
3. **Separate Plot for Each Sequence**: Each sequence is plotted individually on its own 3D plot to provide a detailed trajectory visualization.

The dataset and poses are preprocessed to align and normalize the pose data before visualization.

## 7Scenes Dataset

The [7Scenes Dataset](https://www.microsoft.com/en-us/research/project/rgb-d-dataset-7-scenes/) is an RGB-D dataset that contains sequences captured using a handheld Kinect RGB-D camera in different indoor environments, such as offices and rooms. The dataset is primarily used for visual localization tasks and camera pose regression.

### Dataset Structure

The dataset consists of seven different scenes, with each scene containing multiple sequences. Each sequence has images and their corresponding camera pose (in `.pose.txt` format) describing the camera's 3D position and orientation.

## Visualization Code

The code provided in this repository allows you to visualize the camera trajectories of the 7Scenes dataset. The following libraries are used:

- `OpenCV`: For reading images.
- `Matplotlib`: For plotting 3D trajectories.
- `transforms3d`: For quaternion calculations.
- `PyTorch`: For managing datasets and data loading.

The main functionalities include:

- Loading and processing the pose data (`load_and_process_poses` function).
- Defining a custom dataset class (`FireDataset`) to load images, depth data, and poses.
- Visualizing the trajectories using three different methods.

### Requirements

The following Python packages are required:
- `transforms3d`
- `opencv-python`
- `matplotlib`
- `torch`
- `torchvision`
- `pickle`


