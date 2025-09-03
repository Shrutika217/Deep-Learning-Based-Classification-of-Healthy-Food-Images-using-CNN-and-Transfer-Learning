# 🍎 Healthy Food Image Classification

A deep learning project comparing CNN, ResNet50, EfficientNetB0, and MobileNetV2 for classifying healthy food images. The project applies transfer learning, handles class imbalance with class weights, and evaluates models using accuracy, loss curves, classification reports, and confusion matrices.

📌 Project Overview

The goal of this project is to build an image classification system that can distinguish between different categories of healthy foods.

1. Implemented a basic CNN as a baseline.
2. Applied transfer learning with ResNet50, EfficientNetB0, and MobileNetV2.
3. Addressed class imbalance using computed class weights.
4. Evaluated models with metrics (accuracy, precision, recall, F1-score) and visualizations (training curves, confusion matrices, prediction samples).

📂 Dataset

Source: [Kaggle Link](https://www.kaggle.com/datasets/raflyramadan/healthy-food/data)

Structure:

healthy_food/
    ├── train/
    │   ├── grilled_chicken_breast/
    │   ├── fruit_salad/
    │   ├── boiled_eggs/
    │   └── ...


🧠 Models Implemented

Basic CNN – Simple convolutional network for baseline.
ResNet50 – Residual connections to handle vanishing gradients.
EfficientNetB0 – Compound scaling for accuracy-efficiency tradeoff.
MobileNetV2 – Lightweight, efficient model using depthwise separable convolutions and inverted bottlenecks.

⚙️ Methodology

1. Image preprocessing: Resizing (224×224), normalization, augmentation.
2. Transfer Learning: Pretrained ImageNet weights, frozen base layers, custom classifier head.
3. Training: 10 epochs, Adam optimizer, categorical cross-entropy loss.
4. Evaluation: Accuracy, precision, recall, F1-score, confusion matrices, training curves.

📊 Results

✅ Performance Summary

Best Model: EfficientNetB0 (slightly ahead of ResNet50).
Most Struggled: Basic CNN (limited representational power).
Common Challenge: Differentiating visually similar foods (e.g., salads vs. egg-based dishes).
Transfer Learning Advantage: All pretrained models outperformed the basic CNN significantly.

🔹 Confusion Matrices

Diagonal numbers represent correctly classified samples per class.
Off-diagonal entries represent misclassifications.
EfficientNetB0 and ResNet50 show stronger diagonals compared to the Basic CNN.

📈 Training Curves

EfficientNetB0 and ResNet50 achieved higher validation accuracy with lower loss.
Basic CNN overfit quickly and plateaued.

📌 Key Learnings

Transfer learning with pretrained models significantly improves performance.
MobileNetV2 is a good balance between speed and accuracy.
Confusion matrices reveal challenges in visually similar categories.

📄 Report

A detailed project report with methodology, experiments, and findings is included in the repository (2448387_CAC2_Report.pdf).

Developed by Shrutika Gupta | Deep Learning Project 
