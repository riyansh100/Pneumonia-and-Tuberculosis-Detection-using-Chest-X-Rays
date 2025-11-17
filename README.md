# Pneumonia-and-Tuberculosis-Detection-using-Chest-X-Rays

This project builds a deep-learning-based medical imaging classifier capable of distinguishing between:

-Normal Chest X-rays
-Pneumonia
-Tuberculosis (TB)

Using different architectures — ResNet50, MobileVNet2, InceptionV3, and a Custom CNN — the project evaluates their performance and identifies the most effective model for multi-class medical diagnosis.

We have also deployed a flask web application where the user can upload a medical chest x-ray image and we can determine the category along with a confidence level.

The work combines transfer learning, regularization, data augmentation, and comparative evaluation to create a robust solution suitable for clinical pre-screening applications.

Project Structure:

├── dl33.ipynb                     # Full training + evaluation notebook
├── README.md                      # Project documentation
├── /data
│   ├── pneumonia/                 # Pneumonia dataset (from Kaggle)
│   ├── tuberculosis/              # TB dataset (from Kaggle)
│   └── combined/                  # Merged dataset (auto-created)
└── /models
    ├── resnet50_best.h5
    ├── inceptionv3_best.h5
    └── custom_cnn_best.h5
    └── mobilevnetv2_best.h5

Datasets:

Pneumonia Chest X-ray Dataset (Kaggle)- https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

Tuberculosis Chest X-ray Dataset (Kaggle)- https://www.kaggle.com/datasets/tawsifurrahman/tuberculosis-tb-chest-xray-dataset

Future Improvements:

-Integrate attention mechanisms (SE blocks, CBAM) to highlight infected lung regions
-Train Vision Transformers (ViT, Swin Transformer) for better global feature reasoning



