# 🤖 CIFAR-10 Image Classification using CNN (TensorFlow Implementation)

![Python](https://img.shields.io/badge/Python-3.12-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange)
![Dataset](https://img.shields.io/badge/Dataset-CIFAR10-yellow)
![Status](https://img.shields.io/badge/Status-Completed-green)

---

## 📌 Project Overview
This project implements a Convolutional Neural Network (CNN) using TensorFlow/Keras to classify CIFAR-10 images, achieving 71.06% test accuracy, with detailed analysis of model behavior and limitations.

The goal is to analyze model performance, training behavior, and classification limitations through practical experimentation and evaluation.

---

## 🎥 Demo / Output

### 🔹 Model Accuracy
<img width="737" height="585" alt="Screenshot 2026-05-24 234649" src="https://github.com/user-attachments/assets/8faca707-6f17-4c82-8284-0aa140d2f74d" />


### 🔹 Model Loss
<img width="723" height="583" alt="Screenshot 2026-05-24 234927" src="https://github.com/user-attachments/assets/b2640665-2186-4884-9f78-da47e558c49f" />


### 🔹 Sample Prediction
<img width="496" height="548" alt="Screenshot 2026-05-24 234714" src="https://github.com/user-attachments/assets/1a858cd9-71e8-4792-a542-7fae6bf78b5a" />


### 🔹 Confusion Matrix
<img width="977" height="868" alt="Screenshot 2026-05-24 235632" src="https://github.com/user-attachments/assets/bf273ac4-87c2-4ced-8e0b-a5b4b91b5338" />


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

### 2. Install Dependencies
```bash
pip install tensorflow matplotlib numpy scikit-learn seaborn
```

### 3. Run the Notebook / Script
```bash
python main.py
```

---

## 📁 Project Structure

├── main.py
├── model.py
├── outputs/
├── README.md

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

```markdown
**Total Parameters:** 356,810
```

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
