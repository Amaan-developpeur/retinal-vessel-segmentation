# Retinal Vessel Segmentation with EfficientNetB4 + U-Net

This project focuses on segmenting retinal blood vessels from fundus images using a deep learning pipeline built with U-Net and EfficientNetB4 as the encoder. It is trained on the [Kaggle Retinal Vessel Segmentation dataset](https://www.kaggle.com/datasets/ipythonx/vessel-dataset) and aims to explore medical image segmentation with limited data.

---

## 🚀 Overview

Accurate segmentation of retinal blood vessels is a critical step in diagnosing diseases such as Diabetic Retinopathy and Glaucoma. This project serves as a hands-on application of deep learning for biomedical image segmentation and offers a solid baseline using a modern encoder-decoder structure.

---

## 🧠 Model Architecture

- **Encoder:** EfficientNetB4 (pretrained on ImageNet)
- **Decoder:** U-Net-style upsampling blocks
- **Framework:** [segmentation_models](https://github.com/qubvel/segmentation_models) using TensorFlow backend
- **Loss Function:** Binary cross-entropy
- **Metrics:** Accuracy, IoU score

---

## 📊 Results Summary

- **Validation Accuracy:** 95.57%
- **Validation Loss:** 0.3514  
- **Validation IoU Score:** 0.5421

The model showed high pixel-wise accuracy and moderate IoU performance despite the small dataset size. This reflects the difficulty of segmenting thin and complex vessel structures, but the results are promising given the resource constraints.

---

## 🖼️ Sample Prediction

Visual results include predicted vessel masks overlaid on original fundus images, indicating the model's ability to detect major vessel structures with reasonable precision.



## Install Dependencies
pip install -r requirements.txt

