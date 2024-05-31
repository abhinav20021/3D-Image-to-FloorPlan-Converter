# 3D-Image-to-FloorPlan-Converter

A Python program to convert 3D images into 2D floor plans using image processing techniques.

# Problem Statement

The goal is to develop a Python program that can convert 3D images into floor plans. This involves extracting meaningful information from the 3D images to generate a 2D representation of the floor layout. The challenge includes handling image processing, edge detection, and contour extraction to produce accurate floor plans.

# Approach

To address this problem, we will use the following approach:

Image Loading: Load the 3D image from the specified path.
Grayscale Conversion: Convert the loaded image to grayscale to simplify processing.
Gaussian Blur: Apply Gaussian blur to the grayscale image to reduce noise and enhance edge detection.
Edge Detection: Use the Canny edge detection algorithm to find edges in the image.
Contour Detection: Find contours in the edge-detected image to outline the shapes present.
Contour Drawing: Draw the detected contours on the original image to visualize the floor plan.
Display Results: Display the original image, edge-detected image, and image with contours side by side for comparison.

# Solution

The solution involves implementing the approach using Python and the OpenCV library for image processing. The program includes the following steps:
Loading the Image: The program loads an image from a specified path. It includes error handling to ensure the image file is found and loaded correctly.
Converting to Grayscale: The loaded image is converted to a grayscale image, which simplifies subsequent processing steps.
Applying Gaussian Blur: A Gaussian blur is applied to the grayscale image to reduce noise and improve the accuracy of edge detection.
Edge Detection: The Canny edge detection algorithm is used to identify edges in the blurred grayscale image.
Finding Contours: Contours are detected in the edge-detected image, outlining the significant shapes.
Drawing Contours: The detected contours are drawn on the original image to visualize the detected shapes.
Displaying Images: The original image, edge-detected image, and image with contours are displayed side by side for comparison.
Modify Image Path: If your images are not named 3d_interior.jpg, update the image_path variable in the process_image function with the correct path to your image file.

# Enhancements
To further improve the solution, consider the following enhancements:
Perspective Correction: Implement techniques to correct perspective distortion in 3D images.
Feature Detection: Use machine learning models to detect and label specific architectural features (walls, doors, windows) to improve floor plan accuracy.
Plan Generation: Generate a vector-based floor plan from the detected contours using libraries like svgwrite for scalable vector graphics.

