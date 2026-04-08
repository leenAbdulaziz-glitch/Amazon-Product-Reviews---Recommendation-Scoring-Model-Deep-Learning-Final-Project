# Amazon Product Reviews — Recommendation Scoring Model (Deep Learning)

## Project Overview

This project builds a **Deep Learning-based recommendation scoring model** using Amazon product review data.
The goal is to predict whether a product should be **recommended or not** based on user reviews and related features.

Instead of using traditional machine learning only, this project applies an **Artificial Neural Network (ANN)** with advanced regularization techniques to improve generalization and performance.

---

##  Objectives

* Build a **binary classification model** for recommendation prediction
* Improve model performance using **deep learning techniques**
* Prevent overfitting using **regularization methods**
* Evaluate the model using multiple performance metrics

---

##  Model Architecture (ANN)

The model is a **3-layer fully connected neural network**:

* Layer 1: 128 neurons
* Layer 2: 64 neurons
* Layer 3: 32 neurons
* Output Layer: 1 neuron (Sigmoid activation)

###  Key Techniques Used:

* **ReLU Activation**
* **He Initialization**
* **Batch Normalization**
* **Dropout**
* **L2 Regularization (Weight Decay)**

---

##  Regularization Techniques

To improve generalization and avoid overfitting:

* **L2 Regularization**

  * Penalizes large weights
  * Keeps the model simple and stable

* **Dropout**

  * Randomly disables neurons during training
  * Forces the model to learn robust patterns

* **Batch Normalization**

  * Normalizes layer outputs
  * Speeds up training and improves stability

---

##  Training Strategy

The model uses advanced callbacks to optimize training:

###  Early Stopping

* Monitors validation AUC
* Stops training if no improvement for 10 epochs
* Restores best model weights

###  Reduce Learning Rate

* Reduces learning rate when validation loss plateaus
* Helps fine-tune the model

###  Model Checkpoint

* Saves the best model based on validation AUC

---

##  Evaluation Metrics

The model is evaluated using:

* **Accuracy**
* **AUC (Area Under Curve)**
* **Precision**
* **Recall**

These metrics provide a comprehensive understanding of model performance, especially for imbalanced data.

---

##  Project Structure

```
├── data/
├── notebooks/
├── models/
│   └── best_model.keras
├── src/
├── README.md
```

---



##  Results

* High validation AUC (≈ 0.98+)
* Strong generalization due to regularization
* Stable training using adaptive learning strategies

---

##  Key Insights

* Deep learning significantly improves recommendation scoring
* Regularization is critical for preventing overfitting
* AUC is more reliable than accuracy for this problem

---

##  Future Improvements

* Integrate **NLP models (e.g., BERT)** for text reviews
* Use **ensemble models** (ML + DL)
* Deploy as an **API or web application**
* Add real-time recommendation system

---

##  Author

**Leen Almufleh**
Computer Science Student | AI & Machine Learning Enthusiast

---

##  Project Type

Final Project — Deep Learning & Recommendation Systems
