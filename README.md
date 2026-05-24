# 🤖 CIFAR-10 Image Classification using CNN (TensorFlow Implementation)

![Python](https://img.shields.io/badge/Python-3.12-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange)
![Dataset](https://img.shields.io/badge/Dataset-CIFAR10-yellow)
![Status](https://img.shields.io/badge/Status-Completed-green)

---

## 📌 Project Overview
This project presents a Convolutional Neural Network (CNN) implementation for image classification on the CIFAR-10 dataset using TensorFlow/Keras.

The goal is to analyze model performance, training behavior, and classification limitations through practical experimentation and evaluation.

---

## 🎯 Objectives
- Implement CNN using TensorFlow/Keras
- Train model on CIFAR-10 dataset
- Analyze training and validation performance
- Perform error analysis using confusion matrix
- Evaluate class-wise accuracy

---

## 📊 Dataset
**CIFAR-10**
- 60,000 color images (32×32)
- 10 classes
- 50,000 training images
- 10,000 testing images

### Classes:
Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck

---

## ⚡ How to Run

### 1. Clone Repository
```bash
git clone https://github.com/your-username/Image-Identification.git
cd Image-Identification
```

2. Install Dependencies
```bash
pip install tensorflow matplotlib numpy scikit-learn seaborn
```

3. Run the Notebook / Script
```bash
python main.py
```

---

## 🧠 Model Architecture

- Conv2D (32 filters, 3×3) + ReLU
- MaxPooling2D
- Conv2D (64 filters, 3×3) + ReLU
- MaxPooling2D
- Conv2D (128 filters, 3×3) + ReLU
- Flatten
- Dense (128 units, ReLU)
- Output Layer (Softmax - 10 classes)

Total Parameters: 356,810

---

## 🧪 Training Configuration

- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Batch Size: 64
- Epochs: 10

---

## 📈 Training Results

| Epoch | Train Accuracy | Validation Accuracy |
|------|----------------|---------------------|
| 1    | 44.30%         | 56.22%              |
| 5    | 73.25%         | 69.89%              |
| 10   | 83.72%         | 71.06%              |

---

## 📊 Final Performance
- **Test Accuracy:** 71.06%  
- **Test Loss:** 0.8857  

---

## 📉 Training Analysis
- Rapid learning in early epochs  
- Validation accuracy plateaus after epoch 7  
- Overfitting observed in later epochs  

---

## 🔍 Error Analysis

### Confusion Patterns:
- Cat ↔ Dog  
- Deer ↔ Horse  
- Automobile ↔ Truck  

👉 **Reason:** Similar visual patterns in low-resolution images  

---

## 📊 Class-wise Accuracy

| Class       | Accuracy |
|------------|---------|
| Airplane   | 66.4%   |
| Automobile | 88.3%   |
| Bird       | 70.6%   |
| Cat        | 55.8%   |
| Deer       | 62.4%   |
| Dog        | 64.2%   |
| Frog       | 74.6%   |
| Horse      | 67.2%   |
| Ship       | 88.9%   |
| Truck      | 72.2%   |

---

## 📊 Visualizations
- Training vs Validation Accuracy Curve  
- Training vs Validation Loss Curve  
- Confusion Matrix  

---

## 💾 Model Saving

```python
model.save("model.h5")
```

---

## ⚙️ Limitations
- No data augmentation  
- No dropout regularization  
- No batch normalization  
- Limited depth CNN  
- Overfitting in later epochs  

---

## 🚀 Future Improvements
- Add Dropout and Batch Normalization  
- Apply Data Augmentation  
- Use deeper architectures (ResNet, VGG)  
- Hyperparameter tuning  
- Transfer Learning  

---

## 🧠 Key Learnings
- CNNs effectively learn spatial hierarchies  
- Overfitting is a major issue in small CNNs  
- Regularization improves generalization  
- Confusion matrix is critical for error analysis  

---

## 🛠️ Tech Stack
- Python 3.12  
- TensorFlow (Keras API)  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## 🙋‍♂️ Author

**Satyam Singh Patel**  
https://github.com/satyamsinghpatel476
