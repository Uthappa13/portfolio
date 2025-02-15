---
name: Parameterized Defogging Network for Object Detection in Adverse Weather Conditions
tools: [Python, PyTorch, YOLOv5]
image: /portfolio/images/adverse1.png
description: This project focuses on enhancing object detection in autonomous driving systems under challenging weather conditions like fog.
---

# Parameterized Defogging Network for Object Detection in Adverse Weather Conditions

## Project Overview
This project focuses on enhancing object detection in autonomous driving systems under challenging weather conditions like fog. Adverse weather significantly degrades image quality, affecting the performance of real-time detection.
To address this, the project introduces a Convolutional Neural Network-based Parameter Predictor (CNN-PP) that estimates optimal parameters for a Differentiable Image Processing (DIP) module. The DIP module enhances images by applying defogging, contrast adjustment, gamma correction, and sharpening before passing them to the YOLO-based object detection model. The proposed solution improves detection accuracy and efficiency, making autonomous navigation more reliable in complex environments.

## Tech Stack
- **Python** for programming language
- **PyTroch** for Deep Learning Framework
- **YOLOv5** Object Detection Model
- **Matplotlib** for image visualization


## Methodology
- **Model Architecture**
    The system consists of three main components:
    - **CNN-Based Parameter Predictor (CNN-PP)**
        - Learns optimal parameters for image enhancement.
        - Uses convolutional layers with Leaky ReLU activation to extract hierarchical image features.
    - **Differentiable Image Processing (DIP) Module**
        - Applies six differentiable filters based on CNN-PP outputs.
    - **Detection Network (YOLOv5)**
        - Processes the enhanced images to detect objects in foggy environments.
        - Uses CSPDarknet53 backbone for feature extraction and Path Aggregation Network (PANet) for multi-scale feature fusion.
- **Training Process**
    - The CNN-PP and DIP modules are trained together using an end-to-end hybrid training approach.
    - The dataset consists of 367 images, with ⅔ being foggy images, resized to 256×256 pixels.
    - The DIP-enhanced images are then passed through YOLOv5 for final detection.
- **Performance Evaluation**
    - Compared YOLOv5 with and without the DIP module to measure detection improvement.
    - Evaluated using mAP50, and mAP50-95 metrics.


## Results
- Significant improvement in object detection accuracy on foggy images.
- Metric scores:
    - mAP50 = 0.738
    - mAP50-95 = 0.50

## Project Snippets

- **Model Architecture**
    ![Model Architecture](/portfolio/images/adverse1.png)<br>

- **Image before and after Defogging**
    ![Bearing Health](/portfolio/images/adverse2.png)<br>

- **Object Detection Results**
    ![Bearing Fault](/portfolio/images/adverse3.png)<br>


## Detailed code on Github

<div class="left">
{% include elements/button.html link="https://github.com/Uthappa13/Defogging_network" text="Code on Github" %}
</div>