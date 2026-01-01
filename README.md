# Wi-Fi Radiation Pattern Analysis Using Smartphones

This repository contains the implementation and analysis code focused on studying **Wi-Fi radiation patterns** using **smartphones** and **graphical heatmap visualization**. The project demonstrates a low-cost, accessible alternative to traditional RF measurement tools by leveraging smartphone sensors and Python-based data visualization.

---

## Project Overview

Wi-Fi signals exhibit variations in strength due to distance, obstacles, interference, and population density. In this project, I analyzed how these factors influence Wi-Fi performance by collecting real-world measurements using smartphones and visualizing the results as **heatmaps over a floor plan**.

The approach replaces expensive spectrum analyzers with readily available mobile devices, making Wi-Fi analysis scalable and accessible.

---

## Objectives

- Measure Wi-Fi signal strength (RSSI), internet speed, and upload speed across a defined indoor space  
- Compare signal behavior in **empty vs populated environments**  
- Generate spatial heatmaps to visualize Wi-Fi radiation and performance patterns  
- Evaluate the effectiveness of smartphones as RF measurement tools  

---

## Methodology

### Data Collection
- Environment: Indoor academic building floor
- Tools:
  - Smartphones
  - Apps: **NetSpot**, **Fast.com**
- Parameters recorded:
  - RSSI (Received Signal Strength Indicator)
  - Internet download speed
  - Upload speed
- Measurements taken at predefined grid points mapped to floor coordinates

### Experimental Conditions
- **Baseline (empty space)**
- **Populated space (human interference introduced)**

---

## Data Processing & Visualization

Collected data is stored in CSV format and processed using Python. Heatmaps are generated and overlaid on a floor plan to visually represent signal distribution.

### Visualization Pipeline
1. Load CSV data
2. Pivot data into a 2D grid
3. Interpolate and smooth values using Gaussian filtering
4. Generate heatmaps using Seaborn
5. Overlay heatmaps onto the floor plan using OpenCV

---

## Key Technologies Used

- **Python**
- **Pandas** – data handling
- **Matplotlib & Seaborn** – heatmap visualization
- **SciPy** – interpolation and smoothing
- **OpenCV** – image overlay and blending


