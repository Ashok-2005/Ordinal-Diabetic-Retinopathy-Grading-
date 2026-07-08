# 🩺 Multi-Channel Dense Attention Network with Tri-Objective Optimization for Ordinal Diabetic Retinopathy Grading

A deep learning framework for **ordinal diabetic retinopathy (DR) grading** using retinal fundus images. The proposed framework integrates a **Multi-Channel Dense Attention Network**, a **CORN-based ordinal regression head**, and a **custom Hybrid Tri-Objective Loss Function** to improve disease severity prediction on the **APTOS 2019 Blindness Detection** dataset.

This work was carried out during my **Summer Research Internship** at the **Biomedical Signal and Image Processing (BSIP) Laboratory, National Institute of Technology (NIT) Rourkela** and forms the basis of an **IEEE conference paper**.

---

# 📌 Overview

Diabetic Retinopathy (DR) is one of the leading causes of preventable blindness worldwide. Automated grading of retinal fundus images can assist ophthalmologists in early diagnosis and treatment planning.

Unlike conventional multi-class classification, this project formulates diabetic retinopathy grading as an **ordinal regression problem**, preserving the ordered relationship between disease severity levels.

The proposed framework combines a **multi-channel retinal image representation**, **DenseNet121 with attention**, a **CORN ordinal regression head**, and a **custom Hybrid Tri-Objective Loss Function** to improve grading performance while effectively handling severe class imbalance.

---

# 🎯 Objectives

- Develop an automated diabetic retinopathy grading system.
- Formulate diabetic retinopathy grading as an ordinal regression task.
- Design a Multi-Channel Dense Attention Network.
- Improve ordinal prediction using a CORN-based regression head.
- Develop a custom Hybrid Tri-Objective Loss Function.
- Address class imbalance using Weighted Random Sampling.
- Improve generalization using Albumentations-based augmentation.
- Evaluate the framework using standard medical imaging metrics.

---

# ✨ Features

- Ordinal Diabetic Retinopathy Grading
- Multi-Channel Image Representation
- DenseNet121 Backbone
- Attention-based Feature Learning
- CORN Ordinal Regression Head
- Custom Hybrid Tri-Objective Loss Function
- Weighted Random Sampling
- Albumentations Data Augmentation
- Automatic Mixed Precision (AMP)
- PyTorch Implementation

---

# 🛠️ Technologies Used

- Python
- PyTorch
- Torchvision
- Albumentations
- OpenCV
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Kaggle

---

# 📂 Dataset

**APTOS 2019 Blindness Detection Dataset**

Source:
- Kaggle

The dataset contains retinal fundus images categorized into five diabetic retinopathy severity levels.

| Grade | Severity |
|--------|----------|
| 0 | No DR |
| 1 | Mild |
| 2 | Moderate |
| 3 | Severe |
| 4 | Proliferative DR |

---

# 🔄 Data Preprocessing

The preprocessing pipeline includes:

- Image resizing
- CLAHE enhancement
- RGB + CLAHE Enhanced Green Channel fusion
- Four-channel image generation
- Pixel normalization
- Albumentations data augmentation
- Weighted Random Sampling

---

# 🧠 Proposed Architecture

The proposed framework consists of the following components:

- Multi-Channel Retinal Image Representation
- DenseNet121 Backbone
- Attention Module
- Global Average Pooling (GAP)
- Fully Connected Layer
- CORN Ordinal Regression Head
- Custom Hybrid Tri-Objective Loss Function

### Workflow

```text
Retinal Fundus Image
          │
          ▼
Image Preprocessing
(RGB + CLAHE Green Channel)
          │
          ▼
4-Channel Input
          │
          ▼
DenseNet121 Backbone
          │
          ▼
Attention Module
          │
          ▼
Global Average Pooling
          │
          ▼
Fully Connected Layer
          │
          ▼
CORN Ordinal Regression Head
          │
          ▼
Hybrid Tri-Objective Loss
          │
          ▼
Backpropagation
          │
          ▼
Predicted DR Grade
```

---

# ⚙️ Training Strategy

The proposed model incorporates:

- Transfer Learning using ImageNet-pretrained DenseNet121
- Multi-Channel Input Representation
- CORN Ordinal Regression
- Custom Hybrid Tri-Objective Loss Function
- AdamW Optimizer
- Weighted Random Sampling
- Albumentations Data Augmentation
- Learning Rate Scheduler
- Early Stopping
- Automatic Mixed Precision (AMP)

---

# 📊 Evaluation Metrics

Model performance is evaluated using:

- Quadratic Weighted Kappa (QWK)
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

# 📈 Results

The proposed framework demonstrates:

- Effective ordinal diabetic retinopathy grading.
- Robust learning through CORN ordinal regression.
- Improved performance on imbalanced retinal datasets.
- Better feature extraction using DenseNet121 with attention.
- Enhanced optimization through the custom Hybrid Tri-Objective Loss Function.

---

# 📌 Key Contributions

- Proposed a **Multi-Channel Dense Attention Network** for ordinal diabetic retinopathy grading.
- Designed a **4-channel retinal image representation** by combining RGB channels with a CLAHE-enhanced green channel.
- Integrated a **CORN-based ordinal regression head** to model the ordered nature of diabetic retinopathy severity.
- Developed a **custom Hybrid Tri-Objective Loss Function** to jointly optimize ordinal learning and classification performance.
- Addressed class imbalance using **Weighted Random Sampling** and **Albumentations-based data augmentation**.
- Evaluated the framework using **Quadratic Weighted Kappa (QWK), Accuracy, Precision, Recall, and F1-score**.

---

# 🔮 Future Work

- Validate the framework on larger multi-center retinal datasets.
- Explore Vision Transformer (ViT) and Swin Transformer architectures.
- Investigate self-supervised pretraining for retinal image analysis.
- Extend the framework to other retinal diseases.
- Deploy the model for real-time clinical decision support.

---

# 👨‍💻 Authors

- **Uppalapati Venkata Ashok Adithya**
- **Swayangjyoti**
- **Saisrija**

Summer Research Intern  
Biomedical Signal and Image Processing (BSIP) Laboratory  
National Institute of Technology (NIT) Rourkela

---

# 📚 References

- APTOS 2019 Blindness Detection Dataset
- DenseNet121
- CORN: Conditional Ordinal Regression for Neural Networks
- PyTorch Documentation
- Albumentations Documentation
