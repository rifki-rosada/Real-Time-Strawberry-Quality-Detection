# Real-Time Strawberry Ripeness Detection using YOLO

**Description:** First-author paper and code for IAICT 2025. This project uses state-of-the-art YOLO models to build a highly accurate, real-time strawberry ripeness detection system.
**Official Paper Title:** *"Evaluating YOLO Variants for Real-Time Multi-Object Detection of Strawberry Quality and Ripeness"*
**Conference:** Accepted & Presented at IAICT 2025 (First Author)

---

## 🌟 Overview & Key Achievement

This repository contains the research and implementation of a computer vision system designed to automate strawberry ripeness detection in complex agricultural settings.

After a comparative analysis of three state-of-the-art models, the final **YOLOv11 model** (enhanced with dynamic attention and feature fusion) was identified as the superior solution, achieving a **mean Average Precision (mAP@.50-.95) of 82.0%**.

## 🎯 The Problem

Manual ripeness assessment in strawberry farming is labor-intensive, subjective, and a significant bottleneck in the harvesting process. This can lead to reduced crop yield, increased waste, and inconsistent product quality. The goal of this project was to develop an automated, data-driven solution to this critical agricultural challenge.

## 💡 Our Solution

A three-step framework was developed to identify the optimal model for this task:

1.  **Data Collection:** A robust and diverse dataset of strawberries was compiled. This included images from open-source repositories and original on-site collections at **Ichigo Farm in Ciwidey, West Java, Indonesia**.
2.  **Comparative Analysis:** Three advanced object detection models—YOLOv7, YOLOv8, and YOLOv11—were trained and evaluated on the custom dataset to rigorously compare their performance on key metrics.
3.  **Best Model Selection:** YOLOv11 demonstrated the best overall performance, particularly in recall and robustness, making it the most suitable model for real-world deployment where identifying all ripe fruit is critical.

## 📊 Results

The performance of the three models was benchmarked across several standard object detection metrics:

| Model   | Precision | Recall | mAP@.50 | mAP@.50-.95 |
| :------ | :-------- | :----- | :------ | :---------- |
| YOLOv7  | 0.833     | 0.794  | 0.898   | 0.769       |
| YOLOv8  | **0.883**  | 0.834  | 0.938   | 0.813       |
| **YOLOv11** | 0.874 | **0.855** | **0.942** | **0.820** |

**Conclusion:** YOLOv11 provided the best balance of sensitivity and overall accuracy, making it the top choice for this application.

## 🛠️ Tech Stack

* **Primary Models:** YOLOv7, YOLOv8, YOLOv11
* **Framework:** PyTorch
* **Key Libraries:** Ultralytics, Supervision, Roboflow, OpenCV, Pandas, NumPy, Matplotlib
* **Model Deployment:** ONNX
* **Programming Language:** Python 3.11
* **Development Environment:** Google Colab
* **Hardware:** NVIDIA Tesla T4 GPU with CUDA 12.4

## 🚀 Future Work & Business Impact

The findings from this research serve as a direct proof-of-concept for significant agricultural automation. Future work will focus on:

* Integrating the YOLOv11 model into a physical, automated harvesting system.
* Optimizing the model for deployment on low-power, on-device hardware (edge AI).
* Enhancing the dataset to further improve precision and reduce trade-offs.

This work has direct applications in optimizing crop yield, improving quality control, and increasing the overall efficiency and profitability of modern farming.
