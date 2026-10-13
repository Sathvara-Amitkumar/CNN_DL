### 🚀 Simple Project Overview: Digit Classification & Transfer Learning

I built and compared three types of computer brain models (Neural Networks) to recognize handwritten digits (0-9) using the **MNIST** dataset. I also tested **Transfer Learning** to see how a pre-trained model can recognize real-world objects.

---

### 💡 Easy Explanations of the Models

#### 1. 🧠 Perceptron (Accuracy: 91.97%)
* **What it is:** The simplest kind of neural network. Think of it like a single decision-maker looking at all the pixels at once.
* **How it works:** It takes every pixel, multiplies it by a weight, adds them up, and makes a guess. 
* **Limit:** It is too simple because it can only learn straight-line patterns. It cannot understand complex shapes.

#### 2. 🎛️ ANN - Artificial Neural Network (Accuracy: 97.62%)
* **What it is:** A network with extra layers of "smart helpers" (hidden layers) between the input pixels and the final output.
* **How it works:** The pixels go through these hidden layers. This allows the model to combine simple lines to understand more complex shapes (like curves and loops).
* **Limit:** It treats the image as a flat list of numbers, so it easily forgets how pixels next to each other relate in 2D space.

#### 3. 🌀 CNN - Convolutional Neural Network (Accuracy: 99.10%) 🏆
* **What it is:** A network designed specifically for images.
* **How it works:** It uses "filters" that slide across the image to scan for small features like corners, edges, and shapes (just like human eyes do). 
* **Why it wins:** It understands the 2D layout of images, leading to nearly perfect accuracy.

#### 4. 🔄 Transfer Learning (ResNet50)
* **What it is:** Instead of training a model from scratch, we use a giant model (ResNet50) that was already trained on millions of everyday pictures by experts.
* **How it works:** We borrow its pre-built "knowledge" to instantly classify new objects. In this project, it successfully recognized a custom rabbit image (`wood_rabbit`) without any extra training!

---

### 🔑 Summary Table

| Model | Type | Test Accuracy | Best For |
|---|---|---|---|
| **Perceptron** | Single Layer | **91.97%** | Basic binary patterns |
| **ANN** | Multi-Layer | **97.62%** | General tabular data |
| **CNN** | Convolutional | **99.10%** 🏆 | Images & Computer Vision |
| **ResNet50** | Transfer Learning | **N/A (Pretrained)** | Quick, high-power classification |
