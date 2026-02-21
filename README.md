# Comparative Study of Deep Learning Architectures on CIFAR-10 Using PyTorch

## 📌 Project Overview

This project implements and compares three deep learning architectures on the CIFAR-10 dataset using PyTorch:

- SimpleNN (Fully Connected Neural Network)
- Modified AlexNet
- TinyVGG

The models are trained under the same conditions to ensure a fair comparison based on:

- Test Accuracy
- Training Time
- Model Complexity (Number of Parameters)
- Convergence Behavior
- Generalization Performance

---

## 📂 Dataset

Dataset Used: CIFAR-10  
- 60,000 32x32 color images  
- 10 classes  
- 50,000 training images  
- 10,000 testing images  

Classes:
airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck

---

## 🧠 Models Implemented

### 1️⃣ SimpleNN
- Fully connected feedforward network
- Baseline model
- Fast training
- Lower accuracy compared to CNN models

### 2️⃣ AlexNet (Modified)
- Deep convolutional architecture
- High parameter count
- Best accuracy among all models
- Longer training time

### 3️⃣ TinyVGG
- Lightweight CNN inspired by VGG
- Fewer parameters than AlexNet
- Balanced performance and efficiency

---

## ⚙️ Training Configuration

- Loss Function: CrossEntropyLoss
- Optimizer: Adam
- Learning Rate: 0.001
- Epochs: 10
- Batch Size: 128
- Device: CUDA (if available)

---

## 📊 Results Summary

| Model     | Accuracy | Training Time | Parameters |
|-----------|----------|---------------|------------|
| SimpleNN  | ~54%     | ~123 sec      | ~1.7M      |
| AlexNet   | ~78%     | ~244 sec      | ~35M       |
| TinyVGG   | ~73%     | ~174 sec      | ~0.59M     |

---

## 📈 Key Observations

- CNN-based models outperform fully connected networks for image classification.
- AlexNet achieved the highest accuracy but required more computational resources.
- TinyVGG provides a good balance between performance and efficiency.
- Model complexity directly affects training time and memory usage.

---

## 💾 Saved Models

The trained model weights are saved as:

- SimpleNN.pth
- AlexNet.pth
- TinyVGG.pth

---

## 🛠 Technologies Used

- Python
- PyTorch
- Torchvision
- Matplotlib
- tqdm

---

## 🎯 Conclusion

This project demonstrates that convolutional neural networks significantly outperform simple fully connected networks for image classification tasks. However, deeper models increase computational cost. Efficient architectures like TinyVGG offer a practical compromise between performance and resource usage.
