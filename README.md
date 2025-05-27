# Retinal Vessel Segmentation with EfficientNetB4 + U-Net

This project focuses on segmenting retinal blood vessels from fundus images using a deep learning approach. I used a U-Net architecture with EfficientNetB4 as the encoder backbone, trained and evaluated on the [Retinal Vessel Segmentation dataset](https://www.kaggle.com/datasets/ipythonx/vessel-dataset) from Kaggle.

## 🧠 Motivation
Accurate vessel segmentation plays a vital role in automated diagnosis of retinal diseases like Diabetic Retinopathy and Glaucoma. This project allowed me to explore modern segmentation frameworks and apply them in a real-world medical imaging task, despite having access to limited data.

## 🧪 Model Architecture
- **Backbone:** EfficientNetB4 (pretrained on ImageNet)
- **Segmentation Head:** U-Net decoder
- **Framework:** [segmentation_models](https://github.com/qubvel/segmentation_models) with TensorFlow backend

## 📊 Performance Summary
- **Validation Accuracy:** ~95.57%
- **Validation Loss:** ~0.3514
- **Validation IoU (Intersection over Union):** ~0.5421

Despite the dataset's limited size, the model demonstrated strong generalization and decent segmentation performance, especially given the complexity of detecting fine vessel boundaries.

## ⚙️ Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/retinal-vessel-segmentation.git
cd retinal-vessel-segmentation
