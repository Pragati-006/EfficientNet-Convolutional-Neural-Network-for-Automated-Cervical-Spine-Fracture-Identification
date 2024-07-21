# EfficientNet-Convolutional-Neural-Network-for-Automated-Cervical-Spine-Fracture-Identification

Project Overview

![Thoracic-Spine](https://github.com/user-attachments/assets/c95d4ad8-7694-440a-a5bd-8ece0c7d4074)

The cervical spine, located in the neck and consisting of seven vertebrae (C1 to C7), is essential for supporting the head and facilitating neck movements. Fractures in this region can result from various incidents, including car accidents, sports injuries, or trauma. Such injuries pose significant challenges, often leading to severe complications if not promptly diagnosed.

Traditional methods for diagnosing cervical spine fractures involve manual analysis by healthcare professionals, which can be time-consuming and subjective. This project addresses this challenge by utilizing deep learning techniques to automate fracture detection, aiming to make the diagnostic process faster, more accurate, and less reliant on manual methods.

Dataset

The dataset used in this project is provided by the Radiological Society of North America (RSNA), the American Society of Neuroradiology (ASNR), and the American Society of Spine Radiology (ASSR). It includes CSV files and directories with scan slices and segmentations. The dataset is balanced, with a focus on standardizing image sizes and augmenting data to prepare it for deep learning model training.

kaggle competitions download -c rsna-2022-cervical-spine-fracture-detection
https://www.kaggle.com/competitions/rsna-2022-cervical-spine-fracture-detection/data

Objectives

Automated Fracture Detection: Develop an EfficientNet-based system to automatically identify cervical spine fractures from X-ray images.
Metadata Integration: Enhance the accuracy of fracture detection by incorporating metadata from X-ray images.
Model Optimization: Refine the model using learning rate scheduling and custom loss functions to achieve high accuracy, precision, recall, and F1 scores.
Improved Diagnostic Efficiency: Provide healthcare practitioners with a tool to speed up diagnosis and treatment, improving patient outcomes and reducing the workload on medical professionals.
Methods

Model Architecture: Utilized EfficientNet for image feature extraction, combined with a metadata processing network.
Data Processing: Employed custom data augmentation techniques and designed specific loss functions for fracture and vertebrae detection.
Optimization: Implemented AdamW optimizer with Cosine Annealing Warmup Restarts scheduling for efficient training.

Results

The EfficientNet-based models have demonstrated high accuracy in detecting cervical spine fractures, with strong performance metrics such as accuracy, precision, recall, and F1 score. This automated system holds significant promise for enhancing diagnostic workflows and improving patient care in medical settings.

Vertebrae Detection
![train_model drawio](https://github.com/user-attachments/assets/667bd3dd-549d-4e5c-a3b1-c182d8e86816)

Fracture Detection
![Model drawio](https://github.com/user-attachments/assets/b20d7cb4-79dd-4168-97a8-f74c9e4d3f8a)

Significance

This project contributes to the advancement of medical image analysis by integrating deep learning with metadata, providing a more accurate and reliable tool for diagnosing vertebral fractures. It represents a step forward in leveraging AI for improved healthcare outcomes.
Getting Started

To get started with the project, clone this repository and follow the instructions in the Installation section to set up the environment.
Installation

Clone the repository:
    git clone https://github.com/yourusername/vertebrae-fracture-detection.git


Usage

Run the training script to train the model:
    python train.py

Evaluate the model using:
    python evaluate.py
