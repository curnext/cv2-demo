# Computer Vision Techniques Demo

A comprehensive demonstration of various computer vision algorithms implemented using OpenCV and Python. This project processes a video stream to showcase filtering, edge detection, object tracking, and custom segmentation pipelines.

## Demo Preview

### Processed Output
<video src="output_demo_example.mp4" controls width="100%"></video>

[Download Output Video](output_demo_example.mp4)

### Original Input
<video src="input_video.mp4" controls width="100%"></video>

[Download Input Video](input_video.mp4)

---

## Overview

This repository contains a Jupyter Notebook (`computer_vision_demos.ipynb`) that progressively applies different computer vision techniques to a video feed.

### Key Techniques Demonstrated:

1.  **Basic Image Processing**:
    *   Grayscale conversion
    *   Start/Stop processing control

2.  **Filtering & Noise Reduction**:
    *   **Gaussian Blur**: Smoothing images to reduce noise.
    *   **Bilateral Filter**: smoothing while preserving edges.

3.  **Edge Detection**:
    *   **Sobel Operator**: Detecting vertical and horizontal edges.
    *   **Canny Edge Detector**: Robust multi-stage edge detection.

4.  **Object Detection**:
    *   **Color-Based Segmentation**: Isolating objects based on HSV/BGR color distances.
    *   **Hough Circle Transform**: Detecting circular objects in the frame.
    *   **Template Matching**: Finding a reference image within the video frame.

5.  **Advanced Tracking Pipeline**:
    *   Combining color segmentation, morphological operations (Opening/Closing), contour detection, and ellipse fitting to track moving objects.
    *   Trajectory smoothing using convolution.
    *   Visual effects (Hue shifting on tracked objects).

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
2.  Open the notebook:
    ```bash
    jupyter notebook computer_vision_demos.ipynb
    ```
3.  Run the cells sequentially to process `input_video.mp4` and generate `output_demo.mp4`.

## Project Structure

*   `computer_vision_demos.ipynb`: Main source code and documentation.
*   `input_video.mp4`: Source video for testing.
*   `output_demo.mp4`: Generated result showing all effects.
*   `tracking_template.png`: Template image used for template matching demo.

## License

This project is for educational purposes.
