# Optical Flow and Feature Tracking with OpenCV

This project implements feature detection and optical flow tracking in C++ using OpenCV. It detects strong corners in grayscale frames and tracks their motion across consecutive frames with the Lucas-Kanade method.

## Project Structure

- `main.cpp` — main source code
- `CMakeLists.txt` — build configuration
- `videos/` — sample videos for testing
- `results/` — output visualizations and processed results
- `build/` — build directory for compiled binaries

## Usage

1. Build the project using CMake:
   ```bash
   mkdir build && cd build
   cmake ..
   make
   ```
2. Run the executable:

  ```bash
  ./optical_flow_tracking [path_to_video]
  ```
If no video is specified, the program will attempt to use the default webcam.

## Importance of Feature Tracking

One important application of tracked features is in algorithms for **camera pose estimation**, such as:

- **Visual Odometry**: Estimating the camera’s motion by analyzing the displacement of tracked features between consecutive frames.
- **Structure from Motion (SfM)**: Reconstructing 3D scene structure and camera motion from multiple images.
- **Simultaneous Localization and Mapping (SLAM)**: Building a map of an unknown environment while simultaneously tracking the camera’s position within it.
- **Augmented Reality (AR)**: Aligning virtual objects with the real world by tracking features in the camera feed.

By reliably detecting and tracking key points, these algorithms can compute how the camera moves through space, enabling a wide range of robotics and computer vision applications.

