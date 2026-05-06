# Sketch to System: Automating UML Classification

## 🌐 Interactive Presentation
**View the fully rendered MATLAB outputs and methodology directly in the browser via Kaggle:** [Click Here for the Interactive Kaggle Notebook](https://www.kaggle.com/code/chamendra/automating-uml-classification-transfer-learning)

---

## 📌 Project Overview
As an IT professional transitioning into AI and Data Science, I developed this project to automate the classification of raw software sketches into 6 specific UML diagram classes. By leveraging Deep Learning and Computer Vision, this repository bridges the gap between hand-drawn software architecture and digitized system design. 

## 📊 Dataset & Preprocessing
* **Source:** MDPI Ground Truth Dataset
* **Volume:** 2,626 perfectly scrubbed and categorized images.
* **The `gray2rgb` Challenge:** Standard sketches are single-channel grayscale, but the chosen transfer learning architectures require three-channel RGB inputs. I successfully implemented a `gray2rgb` conversion pipeline to standardize the dataset to `224x224x3` dimensions, satisfying the network requirements while preserving essential geometric edge clarity.

## 🔬 Methodology & Comparative Analysis
The core of this project is a rigorous comparative analysis of three prominent Transfer Learning architectures implemented natively via **MATLAB Live Scripts**:

1. **ResNet-50 (The Baseline):** Achieved an accuracy of ~85%, serving as the primary benchmark for deep residual learning on structured geometric patterns.
2. **VGG16 (The Heavyweight):** Evaluated to observe the trade-offs between dense architecture and computational cost on sparse sketch data.
3. **MobileNetV2 (The Lightweight):** Evaluated to test viability for edge-deployment and rapid, low-resource inference.

## 📂 Repository Contents
* `*.mlx`: The core MATLAB Live Script containing the raw methodology and execution.
* `*.html`: The exported visual output of the script, including code, charts, and metric results.

---
*Author: Chamendra De Silva*
