# Experiment 2: Implementation of a Multi-Layer Perceptron (MLP) for Multi-Class Image Classification

This project implements a **Multi-Layer Perceptron (MLP)** using **TensorFlow/Keras** for multi-class image classification on the **Fashion-MNIST** dataset. The experiment includes data preprocessing, model training, evaluation, and automated hyperparameter optimization using **RandomizedSearchCV** with the **SciKeras** wrapper.

---
## Objective

The objective of this experiment is to implement a Multi-Layer Perceptron (MLP) using TensorFlow/Keras for multi-class image classification on the Fashion-MNIST dataset. The experiment covers image preprocessing, model construction, training, evaluation, and automated hyperparameter optimization using RandomizedSearchCV with the SciKeras wrapper.

---

## Dataset

**Fashion-MNIST**

- Training Images: 60,000
- Testing Images: 10,000
- Number of Classes: 10
- Image Size: 28 × 28 pixels

Classes:
- T-shirt/Top
- Trouser
- Pullover
- Dress
- Coat
- Sandal
- Shirt
- Sneaker
- Bag
- Ankle Boot

---

## Features

- Load and explore the Fashion-MNIST dataset
- Display sample images and class distribution
- Image preprocessing (flattening, normalization, one-hot encoding)
- Build a baseline MLP model
- Train and evaluate the baseline model
- Perform automated hyperparameter optimization using RandomizedSearchCV
- Retrain the optimized model
- Compare baseline and optimized models
- Generate performance plots and confusion matrix

---

## Project Structure

```
Lab 2/
│── Multilayer_Perceptron.ipynb     # Main Jupyter Notebook
│── Experiment_2.tex                # LaTeX Report
│── Experiment_2.pdf                # Compiled Report
│── README.md
│── *.eps                           # Generated plots
```

---

## Requirements

Install Python **3.11 or later**.

Install the required libraries:

```bash
pip install tensorflow keras scikit-learn scikeras numpy matplotlib pandas
```

If you are using **Google Colab**, most libraries are pre-installed. Install SciKeras using:

```bash
pip install scikeras
```

---

## How to Run

### Clone the Repository

```bash
git clone https://github.com/Sadhana2006-art/Deep-Learning-Lab.git
```

Move into the project folder:

```bash
cd Deep-Learning-Lab/Lab\ 2
```

---

### Open the Notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

or

```bash
jupyter lab
```

Open

```
Multilayer_Perceptron.ipynb
```

If using **Google Colab**:

1. Open Google Colab.
2. Upload `Multilayer_Perceptron.ipynb`.
3. Run all cells sequentially.

---

## Workflow

Run the notebook from top to bottom.

The notebook performs the following tasks:

1. Import required libraries
2. Load the Fashion-MNIST dataset
3. Display sample images
4. Plot class distribution
5. Flatten the images
6. Normalize pixel values
7. Convert labels to one-hot encoding
8. Build the baseline MLP
9. Train the model
10. Evaluate the model
11. Generate evaluation metrics
12. Perform RandomizedSearchCV hyperparameter optimization
13. Retrain the optimized model
14. Compare baseline and optimized models
15. Generate all required plots

---

## Model Architecture

```
Input Layer (784)

↓

Dense (128, ReLU)

↓

Dense (64, ReLU)

↓

Output Layer (10, Softmax)
```

The optimized model architecture is selected automatically during hyperparameter optimization.

---

## Hyperparameter Search Space

| Hyperparameter | Values |
|---------------|--------|
| Hidden Layers | 1, 2, 3 |
| Hidden Neurons | 32, 64, 128, 256 |
| Learning Rate | 0.1, 0.01, 0.001 |
| Optimizer | SGD, Adam, RMSProp |
| Activation Function | ReLU, Tanh, Sigmoid |
| Batch Size | 16, 32, 64, 128 |
| Epochs | 10, 20, 30 |
| Dropout | 0.0, 0.2, 0.5 |

---

## Results

The notebook reports:

- Accuracy
- Precision
- Recall
- F1-score
- Classification Report
- Confusion Matrix
- Training Time
- Best Hyperparameters
- Cross-Validation Accuracy
- Testing Accuracy

---

## Generated Outputs

The notebook generates the following figures:

- Sample Images
- Class Distribution
- Training Accuracy vs Epoch
- Validation Accuracy vs Epoch
- Training Loss vs Epoch
- Validation Loss vs Epoch
- Confusion Matrix
- Hyperparameter Search Results
- Baseline vs Optimized Accuracy Comparison

---

## Best Hyperparameters Obtained

| Parameter | Value |
|-----------|-------|
| Hidden Layers | 1 |
| Hidden Neurons | 128 |
| Optimizer | SGD |
| Learning Rate | 0.1 |
| Activation | Tanh |
| Batch Size | 32 |
| Epochs | 30 |
| Dropout | 0.0 |
| Cross Validation Accuracy | 88.63% |

---

## References

- TensorFlow Documentation
- Keras Documentation
- SciKeras Documentation
- Fashion-MNIST Dataset
- Deep Learning by Goodfellow, Bengio and Courville

---

## Author

**Sadhana Sundaresan**

B.Tech Artificial Intelligence & Data Science

Shiv Nadar University Chennai
