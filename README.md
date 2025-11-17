# Pneumonia-and-Tuberculosis-Detection-using-Chest-X-Rays
This project implements a deep learning–based multi-class image classification system to detect Tuberculosis (TB) and Pneumonia from chest X-ray images. It compares the performance of various convolutional neural network architectures  ResNet50, InceptionV3, MobileVNetV2 and a Custom CNN.


⚙️ Key Features

📂 Dataset Integration: Combines and preprocesses public chest X-ray datasets from Kaggle for TB and Pneumonia detection.

🧩 Transfer Learning: Uses pre-trained ResNet50 and InceptionV3 (ImageNet weights) for feature extraction and fine-tuning.

🧠 Custom CNN Model: Designed and trained from scratch for comparative evaluation.

🚫 Overfitting Control: Utilizes Dropout, EarlyStopping, and GlobalAveragePooling for regularization.

📊 Performance Visualization: Plots training vs. validation accuracy/loss and summarizes model performance metrics.

🏆 Model Comparison: Evaluates all architectures to identify the best-performing model based on validation accuracy and loss.

🧪 Technical Workflow

Data Preparation:

Loads and augments X-ray images using ImageDataGenerator

Performs normalization, resizing, and batching

Model Development:

ResNet50: Deep residual CNN with skip connections

InceptionV3: Multi-branch CNN capturing multi-scale features

Custom CNN: 3-block convolutional architecture with max pooling and dropout

Training Setup:

Optimizer: Adam (lr=0.0001)

Loss: Categorical Crossentropy

Metrics: Accuracy

Callbacks: EarlyStopping (patience=5, restore best weights)

Evaluation & Comparison:

Epoch-wise visualization of validation curves

Comparative DataFrame summarizing all models

Identification of best model (ResNet50)

🩺 Dataset Sources

🫁 Pneumonia Chest X-ray Dataset (Kaggle)

🧬 Tuberculosis Chest X-ray Dataset (Kaggle)
