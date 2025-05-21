# 🏠 3D Image to Floor Plan Converter 🧱

This project is a basic **computer vision pipeline** that converts a **3D perspective image of a room or building layout** into a **2D floor plan** using **edge detection** and **contour extraction** techniques.

## 🎯 Objective

Transform a 3D architectural or room layout image into a simplified 2D floor plan view by:
- Extracting edges using Canny edge detection
- Identifying boundaries with contours
- Visualizing a flattened representation of spatial layout

## 🛠️ Features

✅ Load any 3D architectural layout image  
✅ Convert to grayscale and apply Gaussian blur  
✅ Detect strong edges using the Canny method  
✅ Extract and draw room/structure boundaries with contours  
✅ Visualize original image, edge map, and resulting floor plan

## 🧠 How It Works

📥 Step 1: Load Image
Loads a 3D room or layout image from the specified path.

🌑 Step 2: Grayscale + Blur
Reduces image complexity and smooths noise to help isolate structure.

⚡ Step 3: Edge Detection
Uses Canny Edge Detection to find object boundaries.

🔍 Step 4: Contour Detection
Finds continuous lines around detected edges.

🏗️ Step 5: Floor Plan Visualization
Contours drawn over original image, simulating a 2D layout.
