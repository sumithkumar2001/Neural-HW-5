Sumith Kumar Kotagiri (700759479)

You're absolutely right — and thank you for your patience.

There are **two separate codebases** in your project:

1. **A GAN implementation** using PyTorch to generate MNIST digits.
2. **A data poisoning simulation** using a Naive Bayes text classifier (with scikit-learn and seaborn).

I'll create a clear and separate README section for **each** of these projects in a single unified `README.md` file.

---

## ✅ Full README.md

````markdown
# 🧠 Machine Learning Demos: GAN and Data Poisoning

This repository showcases two machine learning concepts:

1. **Generative Adversarial Network (GAN)**: Trained on the MNIST dataset using PyTorch to generate handwritten digits.
2. **Data Poisoning Simulation**: A sentiment classifier shows the effects of adversarially manipulated labels on text classification performance.

---

## 1️⃣ GAN: MNIST Digit Generator

### 📌 Description
A basic GAN model that consists of:
- A **Generator** that creates images from random noise.
- A **Discriminator** that classifies images as real or fake.
The model is trained adversarially so that both networks improve over time.

### 📦 Features
- Simple PyTorch-based implementation
- Saves generated image samples at epoch 0, 50, and 100
- Plots loss trends over training

### 🚀 Requirements
```bash
pip install torch torchvision matplotlib numpy
````

### ▶️ Run the code

```bash
python basic_gan_mnist.py
```

### 📁 Output

* `samples/epoch_0.png`, `epoch_50.png`, `epoch_100.png` — image grids of fake digits
* `loss_plot.png` — line chart of Generator vs Discriminator loss over time

---

## 2️⃣ Data Poisoning in Text Classification

### 📌 Description

This experiment simulates a **data poisoning attack** on a sentiment classifier using scikit-learn. A Naive Bayes model is trained to classify text sentiment, and then labels for a specific subset (e.g., mentions of "UC Berkeley") are flipped to poison the data.

### 📦 Features

* Baseline and poisoned model comparison
* Confusion matrix visualization before and after poisoning
* Uses `CountVectorizer`, `MultinomialNB`, and `seaborn` for plotting

### 🚀 Requirements

```bash
pip install scikit-learn matplotlib seaborn nltk
```

### ▶️ Run the code

```bash
python data_poisoning_simulation.py
```

### 📁 Output

* Confusion matrix before and after poisoning
* Accuracy metrics shown in matrix titles

---

## 📬 Contact

For questions or improvements, feel free to open an issue or pull request.

---

## 📄 License

This project is for educational and research purposes only.

```

---

Would you like this README content saved as a downloadable `README.md` file or added directly to your repo structure?
```
