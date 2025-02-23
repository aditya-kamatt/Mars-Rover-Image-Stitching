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

## Results

- Feature Detection & Matching:
Learnt how to detect key features in individual images and match them across overlapping regions.

- Image Registration Techniques:
Understood how to compute and apply geometric transformations (e.g., affine or perspective transformations) to align multiple images into a seamless panorama.

- Algorithm Optimization:
Experimented with different parameters in the registration process to improve alignment accuracy, reduce misalignment artifacts, and optimize the stitching process.

- MATLAB Scripting & Workflow Automation:
Gained proficiency in using MATLAB, particularly its live script environment, to build, execute, and visualize an entire image processing pipeline.

- Handling Real-World Data Challenges:
Explored challenges such as variations in lighting, perspective distortions, and noise in Mars rover imagery, and learnt techniques to mitigate these issues.

- Visualization & Analysis:
Developed skills in visualizing intermediate steps (e.g., feature matches, transformation overlays) as well as the final stitched image, which can be valuable for both debugging and presenting results.

- Application in Remote Sensing & Robotics:
Demonstrated how image stitching is applied in practical scenarios like planetary exploration, terrain mapping, and enhancing the visual context for autonomous navigation.
