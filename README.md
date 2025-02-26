# Mars Rover Image Stitching

This repository contains MATLAB scripts designed to perform image stitching on Mars rover images. The goal is to take multiple overlapping images captured by a Mars rover and combine them into a seamless panoramic view. This can be particularly useful for visualizing the terrain, analyzing surface features, or creating a composite image for further study.

## Repository Contents

- **MarsRoverFinal.mlx**  
  The main MATLAB Live Script that orchestrates the image stitching process. It loads the images, calls the registration routines, and displays the final stitched image.

- **registerImages.m**  
  A MATLAB function that performs image registration. This function aligns the input images by finding matching features and computing the necessary transformation to stitch them together.

- **README.md**  
  This file provides an overview of the project, instructions on usage, and additional details.

## Features

- **Image Registration:**  
  Utilizes MATLAB’s capabilities to align overlapping images based on detected features.

- **Easy-to-Use Workflow:**  
  Simply run the provided live script to see the stitching process in action.

- **Customizable:**  
  Parameters within `registerImages.m` can be adjusted to refine the registration process as needed.

## Requirements

- **MATLAB:**  
  R20XX or later is recommended.

- **Toolboxes:**  
  - Image Processing Toolbox  
  - (Optional) Computer Vision Toolbox

Make sure you have these toolboxes installed for full functionality.

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/aditya-kamatt/Mars-Rover-Image-Stitching.git
   ```
2. Open in MATLAB:
- Launch MATLAB.
- Navigate to the cloned repository folder.
- Open the `MarsRoverFinal.mlx` file to view and run the live script.

## Usage

1. Prepare Your Images:

Ensure that the images you wish to stitch are available and placed in the correct directory as referenced within the scripts. You might need to adjust file paths depending on your setup.

![Curiosity Rover Images](https://github.com/user-attachments/assets/0e40bea7-090f-4a7d-8cf7-3fd090ea90e1)


2. Run the Live Script:

Execute `MarsRoverFinal.mlx` in MATLAB. The script will:

  - Load the images.
  - Perform image registration using registerImages.m.
  - Display the final stitched panoramic image.

![Panorama](https://github.com/user-attachments/assets/180eec21-d4b1-4204-8810-77935c59315c)


3. Adjust Parameters:
- If needed, modify parameters in `registerImages.m` to improve the registration accuracy for different sets of images.

## What I Learned

### Fundamentals of Computer Vision & Image Processing
- **Image Stitching Techniques:**  
  I gained a deep understanding of how to merge multiple images into a single cohesive panorama, an essential skill in many computer vision applications.

- **Feature Detection and Matching:**  
  I explored key algorithms like SIFT, SURF, and ORB to detect and match features between overlapping images, enabling accurate alignment.

- **Homography and Perspective Transformation:**  
  I learned how to compute homography matrices to warp images correctly, which is critical for aligning images taken from different angles or perspectives.

### Practical Implementation Skills
- **Python and OpenCV:**  
  This project allowed me to enhance my Python programming skills, particularly in using OpenCV—a powerful library for image processing and computer vision tasks.

- **Algorithmic Problem Solving:**  
  I encountered and solved real-world challenges such as handling perspective distortions, optimizing feature matching, and reducing stitching artifacts.

- **Image Blending Techniques:**  
  I experimented with various methods for blending images seamlessly, ensuring smooth transitions and reducing visible seams in the final output.

### Data Handling and Experimentation
- **Working with Raw Image Data:**  
  I learned how to handle and process raw images, which involved tasks like color correction, resizing, and noise reduction, all of which are vital for pre-processing before stitching.

- **Experimentation and Tuning:**  
  The project encouraged me to try out different parameters and techniques—such as tuning feature detection thresholds and experimenting with blending methods—to achieve the best results.

### Advanced Topics and Best Practices
- **Robustness in Varying Conditions:**  
  I explored how to make the stitching process robust against challenges like varying lighting conditions, occlusions, and camera movement, all common in real-world scenarios.

- **Optimization and Efficiency:**  
  I learned methods to optimize the performance of the stitching algorithm, making it feasible to process high-resolution images more efficiently.

- **Real-World Application Insight:**  
  Working with images from a Mars rover provided a unique perspective on how computer vision techniques are applied in space exploration and remote sensing.
