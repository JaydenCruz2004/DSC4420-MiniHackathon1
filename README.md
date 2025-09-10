# CNN Hyperparameter Sweeps with Weights & Biases

## 👥 Team
- **Simeon Betapudi**, **Jayden Cruz**, **Evan Dant**
- **Jayden**  
- **Evan**  

This project explores the use of **Weights & Biases (W&B) sweeps** to optimize hyperparameters in a Convolutional Neural Network (CNN) trained on the **CIFAR-10 dataset**.  
Instead of manually tuning hyperparameters, we automated the process to find the most efficient configuration that achieves **at least 75% accuracy** within limited training (5 epochs).  

---

## 🚀 Idea
We wanted to answer:  
*“What is the fastest and most computationally efficient way to reach 75% accuracy with as few parameters as possible?”*  

---

## 🎯 Motivation
- Manual hyperparameter tuning is slow and inefficient.  
- With only **5 training epochs**, we needed the **best parameters early**.  
- W&B sweeps provide a systematic and reproducible way to explore hyperparameters.  
- We used **Leaky ReLU** to avoid dead neurons and improve training stability.  

---

## 📊 Dataset: CIFAR-10
- 60,000 color images (32x32 pixels)  
- 10 classes (airplane, car, bird, cat, deer, dog, frog, horse, ship, truck)  
- Standard benchmark for image classification tasks  

---

## ⚙️ Methodology
1. **Model**: Convolutional Neural Network (CNN)  
2. **Sweeps**: Implemented using W&B grid search  
3. **Hyperparameters explored**:
   - `base_channels`: [32, 64]  
   - `channel_mult`: [2, 3]  
   - `n_conv_layers`: [4, 5]  
   - `kernel_size`: [3, 5]  
   - `stride`: [1, 2, 3]  
4. **Activation Function**: Leaky ReLU  

---


## ✅ Conclusions
- Sweeps saved significant time vs manual tuning.  
- Leaky ReLU helped maintain stable learning.  
- Future improvements:
  - Try more architectures (ResNet, VGG).  
  - Explore more hyperparameters (learning rate, optimizer types).  

---

## 📚 References & Resources
- [Professor’s CNN Lesson – GitHub Notebook](https://github.com/drscotthawley/DLAIE/blob/main/Lessons/06_ConvNets.ipynb)  
- [W&B Sweeps Documentation](https://docs.wandb.ai/guides/sweeps/)  

