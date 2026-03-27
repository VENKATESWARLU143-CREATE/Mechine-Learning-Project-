# 🚦 Reducing Overfitting in Traffic Sign Classification Using Dropout in Neural Networks

## 📌 Project Overview

This project demonstrates how **Dropout**, a regularization technique in deep learning, helps reduce **overfitting** in Convolutional Neural Networks (CNNs).  

The model is trained to classify traffic signs using the **German Traffic Sign Recognition Benchmark (GTSRB)** dataset. Two models are implemented and compared:

1. Baseline CNN (without Dropout)
2. Regularized CNN (with Dropout)

The goal is to analyze how Dropout improves generalization and stabilizes model performance.

---

## 🎯 Objectives

- Build a Convolutional Neural Network for traffic sign classification
- Demonstrate overfitting in a baseline model
- Apply Dropout to reduce overfitting
- Compare model performance using loss metrics
- Analyze kernel weight distributions
- Evaluate generalization capability

---

## 🧠 Key Concept: Overfitting

Overfitting occurs when a model learns patterns specific to training data but performs poorly on new data.

### Symptoms of Overfitting

- High training accuracy
- Low test accuracy
- Large gap between training and test loss

Dropout helps solve this problem by randomly disabling neurons during training, forcing the network to learn more robust features.

---

## 🗂 Dataset

### German Traffic Sign Recognition Benchmark (GTSRB)

The dataset contains real-world traffic sign images used for classification tasks.

### Dataset Features

- 50,000+ images
- 43 traffic sign classes
- Real-world variations:
  - Lighting
  - Angles
  - Background noise
  - Occlusions

---

## 🏗 Model Architecture

Both models use the same structure except for the Dropout layer.

### CNN Architecture

Input Image  
→ Convolution Layer  
→ ReLU Activation  
→ Max Pooling  
→ Convolution Layer  
→ ReLU Activation  
→ Max Pooling  
→ Fully Connected Layer  
→ Output Layer  

### With Dropout Model

A Dropout layer is added before the final classification layer.
Dropout(p=0.5)

---

## ⚙️ Training Configuration

| Parameter | Value |
|-----------|------|
| Framework | PyTorch |
| Loss Function | CrossEntropyLoss |
| Optimizer | Adam |
| Batch Size | 64 |
| Epochs | 5 |
| Dropout Rate | 0.5 |

---

## 📊 Results

### Model Without Dropout

- Faster training
- Lower training loss
- Higher overfitting
- Poor generalization

### Model With Dropout

- Slightly slower training
- More stable test loss
- Reduced overfitting
- Better generalization

---

## 📈 Observations

### Without Dropout

- Wider distribution of weights
- More extreme values
- Over-specialization

### With Dropout

- More balanced weight distribution
- Lower variance
- Improved stability

---

---

## 🛠 Installation

Clone the repository:


git clone https://github.com/your-username/Machine-Learning-Project.git


Navigate into the project:


cd Machine-Learning-Project


Install dependencies:


pip install -r requirements.txt


---

## ▶️ How to Run

Run the Jupyter Notebook:


jupyter notebook Untitled11.ipynb


Or run the Python script:


python model.py


---

## 📦 Requirements


python >= 3.8
torch
torchvision
numpy
matplotlib
scikit-learn

---

## 📉 Why Dropout Works

Dropout improves model performance by:

- Preventing neuron co-adaptation
- Encouraging redundancy in learning
- Acting as regularization
- Simulating ensemble learning
- Reducing overfitting

---

## ⚖️ Trade-offs

| Advantage | Disadvantage |
|----------|-------------|
| Better generalization | Slower training |
| Reduced overfitting | Slightly higher training loss |
| More stable weights | Increased computation time |

---

## 🧪 Applications

This project is relevant to:

- Autonomous vehicles
- Traffic sign recognition
- Computer vision
- Image classification
- Deep learning research
- Safety-critical AI systems

---

## 🔒 Ethical Considerations

Machine learning systems used in transportation must be reliable and safe.

Poor model performance can lead to:

- Misclassification
- Unsafe decisions
- System failures

Using techniques like Dropout improves robustness and reduces risk.

---

## 📚 References

- Dropout: A Simple Way to Prevent Neural Networks from Overfitting
- PyTorch Documentation
- German Traffic Sign Recognition Benchmark Dataset

---

## 👨‍💻 Author

**Bandi Venkateswarlu**  
Student ID: 24172884  

---

## 📜 License

This project is for academic and educational purposes.

