# Optical Flow and Feature Tracking with OpenCV

This project implements feature detection and optical flow tracking in C++ using OpenCV. It detects strong corners in grayscale frames and tracks their motion across consecutive frames with the Lucas-Kanade method.

## Project Structure

- `main.cpp` — main source code
- `CMakeLists.txt` — build configuration
- `data/` — input images or related data
- `videos/` — sample videos for testing
- `results/` — output visualizations and processed results
- `build/` — build directory for compiled binaries

## Usage

1. Build the project using CMake:
   ```bash
   mkdir build && cd build
   cmake ..
   make
2. Run the executable (optionally with a video file):

  ```bash
  Copy
  Edit
  ./optical_flow_tracking [path_to_video]
  If no video is specified, the program will attempt to use the default webcam.
