# **Lane Detection** 

<img src="laneLines_thirdPass.jpg" width="480" alt="Combined Image" />

This project is a lane detection system using computer vision techniques. It aims to identify and draw lane lines on the road in images and videos.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Pipeline Overview](#pipeline-overview)
- [Results](#results)
- [Requirements](#requirements)
- [Contributing](#contributing)
- [Contact](#contact)

## Introduction

Lane detection is a crucial aspect of autonomous vehicles and advanced driver-assistance systems (ADAS). This project utilizes Python, OpenCV, and several computer vision techniques, including color selection, region of interest selection, grayscaling, Gaussian smoothing, Canny edge detection, and Hough transform line detection, to identify and draw lane lines on the road in images and videos.

## Installation

To run the lane detection system, follow these steps:

1. Clone this repository to your local machine:

```bash
git clone https://github.com/yourusername/Lane-Detection-Project.git
```

2. Install the required packages. You can use the provided `requirements.txt` file:

```bash
pip install -r requirements.txt
```

3. Run the lane detection script:

```bash
python lane_detection.py
```

Note: Make sure you have Python installed on your machine and properly set up the environment.

## Usage

The lane detection system can process images and videos. To use the system:

1. Place your images in the `test_images` directory.
2. Place your videos in the `test_videos/input` directory.
3. Run the lane detection script as mentioned in the Installation section.

The processed images and videos will be saved in the `test_images` and `test_videos/output` directories, respectively.

## Features

The lane detection system offers the following features:

- Identifies lane lines in images and videos.
- Draws the lane lines on the images and videos.
- Provides a simple and efficient lane tracking mechanism.
- Utilizes region of interest selection to focus only on the relevant part of the image.
- Implements color selection for white and yellow lane lines.

## Pipeline Overview

The lane detection pipeline consists of the following steps:

1. Color selection: Identify white and yellow lane lines using HSV color space.
2. Region of interest selection: Focus on the relevant region where lane lines are expected.
3. Grayscaling: Convert the image to grayscale for Canny edge detection.
4. Gaussian smoothing: Apply Gaussian blur to reduce noise in the image.
5. Canny edge detection: Detect edges in the image.
6. Hough transform: Detect lines in the edge-detected image.
7. Lane line filtering: Identify and filter lane line segments.
8. Lane line fitting: Fit lane lines using linear regression.
9. Lane line stability check: Check the stability of lane lines using a buffer.
10. Draw lane lines: Draw the identified lane lines on the original image.

## Results

The lane detection system provides accurate and stable lane detection on images and videos. It successfully identifies and draws lane lines on various road surfaces and lighting conditions.

## Requirements

The lane detection system has the following requirements:

- Python 3.x
- OpenCV
- Matplotlib
- NumPy

The required packages are listed in the `requirements.txt` file for easy installation.

## Contributing

Contributions to this project are welcome! If you find any issues or have suggestions for improvements, please feel free to create an issue or submit a pull request.

## Contact

For any questions or inquiries, please contact [pdoshi7@vt.edu](mailto:pdoshi7@vt.edu).

---
