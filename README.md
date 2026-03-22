# Hybrid 3D-CNN and Vision Transformer Framework for Multi-Class Retinal Disease Classification
## 📌 Overview

This project presents a Hybrid Deep Learning framework combining 3D Convolutional Neural Networks (3D-CNN) and Vision Transformers (ViT) for multi-class retinal disease classification using medical imaging data. The proposed approach aims to improve feature extraction, spatial understanding, and classification performance by leveraging both convolutional and transformer-based architectures.

The model leverages:
* CNNs → Local spatial feature extraction
* Transformers → Global contextual understanding
* 3D volumetric representation → Depth-aware retinal analysis

📍 The work was developed as part of an academic research project and presented at IEEE BECITHCON 2025.

## 🎯 Key Objectives

* ✅ Designed a dual-branch hybrid architecture (3D-CNN + ViT)
* ✅ Introduced a pseudo-3D volume generation technique from 2D OCT images
* ✅ Achieved state-of-the-art performance within project scope
* ✅ Applied Explainable AI (EigenCAM) for model interpretability
* ✅ Conducted an ablation study to validate architectural improvements

## 🧠 Model Architecture

* InceptionV3
* EfficientNETB0
* ResNET18
* VGG16
* ViT
* Swin
* Hybrid 3D-CNN + ViT
  
🔹 Hybrid Design
* 3D-CNN Branch
  * Input: 4 stacked slices (original + augmented variants)
  * Captures depth & volumetric features
* Vision Transformer Branch
  * Input: 2D OCT image patches
  * Captures global dependencies via self-attention
* Fusion Layer
  * Feature concatenation → Fully connected classifier

This hybrid design allows the model to balance fine-grained local patterns with global feature representation.

## 📊 Dataset & Preprocessing

* Dataset: Retinal OCT Image Classification – C8
* Total Images: 24,000
* Classes (8):
  * AMD, CNV, DME, Drusen, MH, DR, CSR, Normal
    
## 📂 Data Split
* Training: 18,400
* Validation: 2,800
* Test: 2,800

⚠️ Dataset files are not included in this repository due to privacy and size constraints.

## ⚙️ Preprocessing Pipeline
* Image resizing:
  * CNN models: 299×299
  * ViT: 224×224 / 384×384
  * 3D-CNN: 128×128
* Normalization: [-1, 1]
* Data augmentation:
  * Random flip
  * Rotation (±15°)
  * Random crop
  * Color jitter
    
## 🔥 Novel Step
* Converted 2D images → Pseudo-3D volumes
* Stacked augmented variants to simulate depth

## 🧪 Models Evaluated
* InceptionV3
* EfficientNetB0
* ResNet18
* VGG16
* Vision Transformer (ViT)
* Swin Transformer
* Hybrid 3D-CNN + ViT (Proposed Model)
  
## 📈 Results
🔥 Performance Comparison
## 📈 Results

| Model                 | Accuracy | Precision | Recall | F1-score |
|----------------------|----------|----------|--------|----------|
| InceptionV3          | 75.07%   | 75.84%   | 75.07% | 75.09%   |
| EfficientNetB0       | 82.18%   | 82.47%   | 82.18% | 82.10%   |
| ResNet18             | 83.04%   | 83.20%   | 83.04% | 82.93%   |
| VGG16                | 80.86%   | 81.13%   | 80.86% | 80.63%   |
| ViT                  | 87.89%   | 88.05%   | 87.89% | 87.84%   |
| Swin                 | 82.29%   | 82.51%   | 82.29% | 82.19%   |
| **Hybrid (Proposed)**| **91.68%** | **91.87%** | **91.68%** | **91.67%** |

📌 The proposed hybrid model outperforms all baseline architectures.

## 🔬 Ablation Study

| Variant        | F1 Score | Accuracy |
|----------------|----------|----------|
| Baseline ViT   | 0.8784   | 87.89%   |
| + Augmentation | 0.8589   | 85.96%   |
| **Full Model** | **0.9167** | **91.68%** |

👉 Confirms that hybrid + augmentation + attention significantly improves performance.

## 🧠 Explainability (XAI)
* Applied EigenCAM
* Visualized:
  * Critical retinal regions influencing predictions
* Improves model transparency for medical AI

## ⚙️ Technologies Used

* Python
* PyTorch
* NumPy
* Pandas
* Scikit-learn
* Matplotlib

## 🛠️ Setup & Usage

```bash
# Clone repository
git clone https://github.com/stamahmudtonmoy/Hybrid-3D-CNN-and-Vision-Transformer-Framework-for-Multi-Class-Retinal-Disease-Classification.git

# Navigate to project
cd Hybrid-3D-CNN-and-Vision-Transformer-Framework-for-Multi-Class-Retinal-Disease-Classification

# Install dependencies
pip install -r requirements.txt

# Start notebook
jupyter notebook 
```

## 📁 Project Structure

```
project/
 └── group_assignment.ipynb
```

## 📄 Research Publication

This work was presented at:

### IEEE BECITHCON 2025
Hybrid 3D-CNN and Vision Transformer Framework for Multi-Class Retinal Disease Classification

## 👨‍💻 My Contributions (S T A Mahmud Tonmoy)
* Designed Hybrid 3D-CNN + ViT architecture
* Implemented data preprocessing & augmentation pipeline
* Developed training & evaluation pipeline in PyTorch
* Performed model comparison & ablation study
* Integrated Explainable AI (EigenCAM)

## 🚀 Future Improvements

* Deploy model using MLOps pipelines
* Experiment with larger datasets
* Hyperparameter tuning
* Real-time inference optimization
* Cloud-based deployment
* Multi-modal learning (image + patient data)
* Bangladesh-specific medical dataset integration

## 📬 Author

* Soleman Hossain
* S T A Mahmud Tonmoy
* Sihab Mahmud
* M Shamimul Haque Mondal Shimul

## 📝 Disclaimer

This repository is intended for academic and research purposes only. Clinical usage requires extensive validation and regulatory approval.
