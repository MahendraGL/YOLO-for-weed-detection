# Automated Weed Detection on Edge Devices (Master's Thesis)

![Project Status](https://img.shields.io/badge/Status-Thesis_Completed-success)
![Hardware](https://img.shields.io/badge/Hardware-Raspberry_Pi-red)
![Focus](https://img.shields.io/badge/Focus-Edge_AI_%26_Computer_Vision-blue)

## 📄 Overview
This repository serves as an archive for my Master's Thesis: **"Automated Weed Detection in Crops using Computer Vision."**

The project explores the feasibility of deploying deep learning models on resource-constrained edge devices for precision agriculture. Specifically, it compares four variations of the YOLO (You Only Look Once) architecture to find the optimal balance between inference speed (FPS) and detection accuracy (mAP) on a Raspberry Pi.

> **Note:** The complete training code is archived locally. This repository hosts the thesis documentation, experimental results, and architectural breakdown.

## 📥 Thesis Document
You can read the full detailed analysis, methodology, and mathematical background in the thesis document attached below:

[**📄 Click here to view the Full Master's Thesis (PDF)**](./MTP_Report.pdf)

## 🎯 Objectives
* **Dataset:** Collection and annotation of custom crop/weed datasets.
* **Model Comparison:** Benchmarking YOLO v5, v6, v7, and v8.
* **Quantization/Optimization:** Converting models (e.g., ONNX, TFLite) for ARM-based processors.
* **Deployment:** Real-time inference testing on Raspberry Pi.

## 📊 Key Results & Performance
The models were evaluated based on Mean Average Precision (mAP@0.5) and Frames Per Second (FPS) on the Raspberry Pi.

| Model Version | Precision | Recall | mAP@0.5 | Pi Inference (FPS) |
|:-------------:|:---------:|:------:|:-------:|:------------------:|
| YOLO v5s      | ...       | ...    | ...     | ...                |
| YOLO v6n      | ...       | ...    | ...     | ...                |
| YOLO v7-tiny  | ...       | ...    | ...     | ...                |
| YOLO v8n      | ...       | ...    | ...     | ...                |

**Conclusion:** The experiment demonstrated that **[YOLO v5]** offered the best trade-off, achieving real-time performance suitable for robotic weeding applications.

## 🖼️ Visuals
### 1. Detection Samples
*(Replace this text with a screenshot from your PDF showing the bounding boxes around weeds)*
![Detection Example](./images/results.png)

### 2. Training Metrics
*(Replace this text with a screenshot of your Loss/Accuracy graphs from the PDF)*
![Training Graphs](./images/YOLOv5_1.png)

## 🛠️ Technology Stack
* **Hardware:** Raspberry Pi [4b], RPi Camera Module
* **Software:** Python, PyTorch, OpenCV
* **Deployment:** ONNX Runtime / TFLite
