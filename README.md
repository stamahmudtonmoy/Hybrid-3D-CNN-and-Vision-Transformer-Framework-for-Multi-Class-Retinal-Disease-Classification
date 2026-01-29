# Hybrid 3D-CNN and Vision Transformer Framework for Multi-Class Retinal Disease Classification
## 📌 Overview

This project presents a Hybrid Deep Learning framework combining 3D Convolutional Neural Networks (3D-CNN) and Vision Transformers (ViT) for multi-class retinal disease classification using medical imaging data. The proposed approach aims to improve feature extraction, spatial understanding, and classification performance by leveraging both convolutional and transformer-based architectures.

The work was developed as part of an academic research project and presented at IEEE BECITHCON 2025.

## 🎯 Objectives

* Design a hybrid architecture integrating 3D-CNN and Vision Transformer
* Classify multiple retinal diseases from medical image datasets
* Improve classification accuracy by combining local feature learning and global contextual attention
* Evaluate performance using standard classification metrics

## 🧠 Model Architecture

* InceptionV3
* EfficientNETB0
* ResNET18
* VGG16
* ViT
* Swin
* Hybrid 3D-CNN + ViT

This hybrid design allows the model to balance fine-grained local patterns with global feature representation.

## 📂 Dataset & Preprocessing

* Medical retinal image dataset (preprocessed for model compatibility)
* Image resizing and normalization
* Data augmentation to reduce overfitting
* Train-test split for evaluation

⚠️ Dataset files are not included in this repository due to privacy and size constraints.

## ⚙️ Technologies Used

* Python
* PyTorch
* NumPy
* Pandas
* Scikit-learn
* Matplotlib
* Vision Transformer (ViT)
* 3D Convolutional Neural Networks

## 📊 Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

The hybrid model demonstrates improved performance compared to standalone CNN-based approaches.

## 📈 Results

* Achieved competitive classification accuracy for multiple retinal disease classes
* Improved feature learning through hybrid architecture
* Demonstrated effectiveness of transformer-based attention in medical imaging tasks

## 📄 Research Publication

This work was presented at:

### IEEE BECITHCON 2025
Hybrid 3D-CNN and Vision Transformer Framework for Multi-Class Retinal Disease Classification

## 🚀 Future Improvements

* Deploy model using MLOps pipelines
* Experiment with larger datasets
* Hyperparameter tuning
* Real-time inference optimization
* Cloud-based deployment

## 📬 Author

* Soleman Hossain
* S T A Mahmud Tonmoy
* Sihab Mahmud
* M Shamimul Haque Mondal Shimul

## 📝 Disclaimer

This repository is intended for academic and research purposes only. Clinical usage requires extensive validation and regulatory approval.
