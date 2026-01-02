# IHRCD-Det: High-Resolution Detection Dataset for Reinforced Concrete Surface Defect of Industrial Architectural Heritage

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)

This repository contains the IHRCD-Det dataset, a specialized high-resolution dataset designed for the autonomous detection of reinforced concrete (RC) surface defects in industrial architectural heritage scenarios.
---

## 📌 Overview
Industrial architectural heritage structures (e.g., blast furnaces, silos, chimneys) are subject to extreme environments. **IHRCD-Det** provides a high-resolution solution for identifying complex defects that differ significantly from civilian buildings.

* **Images:** 6,388 high-resolution slices ($1024 \times 1024$ pixels).
* **Original Data:** 578 ultra-high-resolution images ($4096 \times 3072$).
* **Defect Categories:** 8 types (Crack, Spalling, Exposed reinforcement, Rust stain, Chemical corrosion, Hole, Repair mark, Anthropogenic mark).
* **Sources:** Captured from major Chinese industrial heritage sites including Shougang, Wuhan Iron and Steel, etc.
---

## 📸 Visual Samples
![Defect Samples](figures/fig3.png)  
*Figure: Representative visual features of the 8 RC defect categories in IHRCD-Det.*

---

## 📊 Dataset Statistics
The dataset covers 6 types of structural components: **Beams, Slabs, Columns, Walls, Roofs/Trusses, and Equipment Foundations**.

| Damage Type | Defect Name | Key Characteristics |
| :--- | :--- | :--- |
| **Structural Damage** | Crack, Spalling, Exposed reinforcement | Focuses on structural integrity. |
| **Material Degradation** | Rust stain, Chemical corrosion, Hole | Result of physical/chemical erosion. |
| **Human Intervention** | Repair mark, Anthropogenic mark | Traces of usage and historical repair. |

---

## 🚀 Benchmark Results
We evaluated the dataset using 10 state-of-the-art models on an NVIDIA RTX 4090.

| Model | Precision | Recall | mAP@0.5 | mAP@0.5:0.95 | Latency (ms) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **YOLO11-l** | **75.0%** | 60.3% | **69.2%** | **51.4%** | 35.5 |
| **YOLO11-m** | 74.8% | **62.9%** | 67.9% | 49.3% | 28.5 |
| **YOLOv12-n** | 63.5% | 56.8% | 59.3% | 36.3% | 14.0 |
| **Faster R-CNN**| 65.1% | 41.9% | 55.4% | 40.2% | 20.3 |

*Experimental results indicate that YOLO11-l is currently the best choice for industrial heritage monitoring tasks.*

---

## 📥 Download
Full Dataset: [Link to Zenodo/Baidu Netdisk]
