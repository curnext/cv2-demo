# Computer Vision Techniques Demo

This repository contains a collection of computer vision algorithms implemented as part of a **Computer Vision Course Assignment**. The project demonstrates various image processing techniques using OpenCV and Python, including filtering, edge detection, object detection, and a custom object tracking pipeline.

**Note:** This codebase is provided as a personal archive of course work.

## Demo Preview

### Processed Output
[▶️ View Output Video (output_demo_example.mp4)](output_demo_example.mp4)

### Original Input
[▶️ View Input Video (input_video.mp4)](input_video.mp4)

---

## Overview

The core of this project is the Jupyter Notebook `computer_vision_demos.ipynb`, which processes a video stream (`input_video.mp4`) frame-by-frame to visualize different CV concepts.

### Key Techniques Demonstrated

1.  **Basic Image Processing**
    *   Grayscale conversion and basic channel manipulation.

2.  **Filtering & Noise Reduction**
    *   **Gaussian Blur**: Smoothing images to reduce high-frequency noise.
    *   **Bilateral Filter**: smoothing images while preserving edge sharpness.

3.  **Edge Detection**
    *   **Sobel Operator**: Computing image gradients to detect vertical and horizontal edges.
    *   **Canny Edge Detector**: A multi-stage algorithm for robust edge detection.

4.  **Object Detection**
    *   **Color-Based Segmentation**: Isolating objects based on specific color ranges (HSV/BGR).
    *   **Hough Circle Transform**: Detecting circular shapes in the frame.
    *   **Template Matching**: Locating a specific template image within a larger video frame.

5.  **Advanced Custom Tracking Pipeline**
    *   A comprehensive pipeline combining **Color Segmentation**, **Morphological Operations** (Opening/Closing), **Contour Detection**, and **Ellipse Fitting**.
    *   Includes **Trajectory Smoothing** using temporal convolution.
    *   Demonstrates visual effects like **dynamic hue shifting** on tracked objects.

## Getting Started

### Prerequisites

*   Python 3.8+
*   Jupyter Notebook
*   OpenCV (`opencv-python`)
*   NumPy

### Installation

```bash
pip install opencv-python numpy jupyter
```

### Usage

1.  Clone this repository.
2.  Launch the notebook:
    ```bash
    jupyter notebook computer_vision_demos.ipynb
    ```
3.  Execute the cells sequentially to process `input_video.mp4`.
4.  The script will generate a new `output_demo.mp4` file with all visual effects applied.

## Project Structure

*   `computer_vision_demos.ipynb`: Main source code and documentation.
*   `input_video.mp4`: Raw input video for testing.
*   `output_demo_example.mp4`: Example of the processed output video.
*   `tracking_template.png`: Template image used for the template matching demo.

