# High-Precision CNC Linear Servo Drive ⚙️

![Build Status](https://img.shields.io/badge/Status-Completed-success)
![CAD](https://img.shields.io/badge/CAD-SolidWorks-blue)
![Engineering](https://img.shields.io/badge/Domain-Mechatronics%20%26%20Automation-orange)

## Overview
This repository contains the complete mechanical and mechatronic design of a heavy-duty, high-precision linear ball screw servo drive system for a CNC machine. The project includes 3D CAD models, GD&T compliant manufacturing drawings, and full mathematical sizing documentation based on industrial catalogs.

![Hero Image Placeholder](https://github.com/Zsoli28/High-Precision-CNC-Linear-Servo-Drive/blob/main/full.png?raw=true)

## 💡 Key Engineering Highlights
Rather than a basic mechanical assembly, this project focuses on real-world industrial reliability and automation principles:

* **Optimized Homing & Soft Limits:** To reduce wiring complexity in the cable drag chain, the system uses a single traveling limit switch (Balluff BNS001K). Homing logic and directional memory (State Tracking) are utilized to establish the machine zero, while the opposite end relies on software limits (Soft Limits) and mechanical hard stops with torque-limit monitoring.
* **Master-Slave Guideway Architecture:** To prevent hyperstatic binding due to microscopic manufacturing inaccuracies, the linear rails are designed with a Master-Slave configuration. The Master rail provides strict lateral alignment via clamping plates, while the Slave rail allows micro-lateral compliance.
* **GD&T Manufacturing Standards:** All custom components (bed, table, motor mount) are dimensioned using strict Geometric Dimensioning and Tolerancing (GD&T) standards, including precise fits (e.g., H7/g6, H7/j6) for bearing housings and the ball nut.

## 📊 Technical Specifications
The system was mathematically sized for an 8500-hour operational lifespan under the following parameters:

| Parameter | Value |
| :--- | :--- |
| **Stroke (Travel)** | 720 mm |
| **Max Feed Force** | 5.2 kN |
| **Rapid Traverse Speed** | 1.1 m/s |
| **Max Operating Speed** | 0.7 m/s |
| **Servo Motor** | Panasonic MSME204G1 (2000W) |
| **Ball Screw** | Bosch Rexroth FEM-E-B 40x20x6 |
| **Linear Guides** | Bosch Rexroth R205A (Size 35) |
| **Coupling** | TRASCO-ES 28/38 |

## 📁 Repository Structure
```text
📦 CNC-Linear-Servo-Drive
 ┣ 📂 CAD_Models
 ┃ ┣ 📜 CNC_Assembly.step        # Full assembly for universal CAD viewing
 ┃ ┗ 📜 Native_SolidWorks_Files/ # Original .sldprt and .sldasm files
 ┣ 📂 Documentation
 ┃ ┣ 📜 2D_Manufacturing_Drawing.pdf  # A0/A1 Assembly drawing with GD&T
 ┃ ┗ 📜 Engineering_Calculations.pdf  # 17-page mathematical sizing & component selection
 ┗ 📜 README.md
