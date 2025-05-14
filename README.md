High-Precision Face Detection using MATLAB with GUI
This project implements a high-precision face detection system using MATLAB, developed as part of the Image Processing Course (ECE228) at Zagazig University, Faculty of Engineering, Department of Electronics and Communications Engineering (2024/2025). The system detects human faces in digital images through custom algorithms focusing on skin tone segmentation, shape symmetry, and geometric filtering, integrated with a user-friendly GUI application.
Project Overview
The objective is to accurately detect human faces in images without relying on MATLAB's high-level built-in functions. The algorithm uses:

Gaussian Smoothing to reduce noise.
YCbCr Color Space Conversion for robust skin detection.
Skin Mask Extraction based on Cb/Cr thresholds.
Morphological Operations (e.g., hole filling, small object removal) for mask refinement.
Geometric and Symmetry Analysis to verify face regions using elliptical shape matching, horizontal symmetry, and eccentricity checks.

A MATLAB-based GUI provides an interactive interface with functionalities to load images, start detection, reset the view, and exit the application.
Features

Custom Algorithm: Avoids high-level MATLAB functions for educational purposes.
GUI Application: User-friendly interface for image loading and face detection visualization.
Robust Detection: Handles varying lighting conditions with low false positives.
Modular Design: Clear separation of detection logic and GUI components.

Prerequisites

MATLAB (R2018b or later recommended) with the following toolboxes:
Image Processing Toolbox


A computer with basic hardware (4GB RAM, 1GHz CPU) for running the GUI and processing images.

Installation

Clone the repository:git clone https://github.com/<your-username>/<your-repo-name>.git


Open MATLAB and navigate to the project directory:cd path/to/your/project


Ensure the Image Processing Toolbox is installed. Verify by running:ver



Usage

Launch MATLAB and open the main script (e.g., FaceDetectionApp.m).
Run the script to start the GUI:FaceDetectionApp


Use the GUI buttons:
Load Image: Select an image file (e.g., JPG, PNG).
Start Detection: Process the image and display bounding boxes around detected faces.
Reset: Clear the current image and results.
Exit: Close the application.


View results in the GUI, with detected faces highlighted.

Project Structure

FaceDetectionApp.m: Main script for launching the GUI and core detection logic.
README.md: This file, providing project documentation.
/images: 
/docs: (Optional) Additional documentation, including the project report.
/Application : 

Challenges and Solutions

Noisy Images: Addressed using Gaussian blur for smoothing.
Skin Segmentation: Improved by using YCbCr color space instead of RGB.
False Positives: Reduced with combined symmetry, shape, and eccentricity constraints.
Function Limitation: Implemented using basic MATLAB functions for educational purposes.

Results

Accuracy: High for frontal faces in well-lit conditions.
False Positive Rate: Low due to strict verification criteria.
Performance: Suitable for real-time GUI interaction.

Screenshots

Team
Developed by:

Abdallah Ahmed Abdelwahid
Abdelrahman Mohamed Saad
Ahmed Gamal Mahmoud Salem
Ahmed Osama Soliman
Ezzat Mohamed Abdelmohsen Mohamed
Mohamed Abdo El-Sayed Attallah
Nada Mohamed Naguib
Shahd Ahmed Goda

Supervised by: Dr. Azhar Ahmed Hamdi
License
This project is licensed under the MIT License. See the LICENSE file for details.
Acknowledgments

Zagazig University, Faculty of Engineering
Dr. Azhar Ahmed Hamdi for guidance and support
