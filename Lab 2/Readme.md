# Experiment 2: Implementation of a Multi-Layer Perceptron (MLP) for Multi-Class Image Classification

## Objective

The objective of this experiment is to implement a Multi-Layer Perceptron (MLP) using TensorFlow/Keras for multi-class image classification on the Fashion-MNIST dataset. The experiment covers image preprocessing, model construction, training, evaluation, and automated hyperparameter optimization using RandomizedSearchCV with the SciKeras wrapper. As an additional exercise, the Single Layer Perceptron (SLP) learning algorithm is implemented for the XOR gate to demonstrate its inability to converge on a non-linearly separable problem.

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

## Main Experiment

- Load and explore the Fashion-MNIST dataset
- Display sample images and class distribution
- Image preprocessing
  - Flattening
  - Normalization
  - One-hot encoding
- Build a baseline MLP model
- Train and evaluate the baseline model
- Perform automated hyperparameter optimization using RandomizedSearchCV
- Retrain the optimized model
- Compare baseline and optimized models
- Generate performance plots

## Additional Exercise

Implementation of the **Single Layer Perceptron (SLP)** for the **XOR Gate**.

The implementation includes:

- Weight initialization
- Bias initialization
- Step activation function
- Perceptron learning rule
- Weight updates after each misclassification
- Decision boundary after each weight update
- Analysis of the non-convergence behaviour
- Demonstration of why the XOR problem cannot be solved using a Single Layer Perceptron

---

## Project Structure

```
Lab 2/
│── Multilayer_Perceptron.ipynb     # Fashion-MNIST classification and additional XOR experiment
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

## Fashion-MNIST Classification

- Import required libraries
- Load the Fashion-MNIST dataset
- Display sample images
- Plot class distribution
- Flatten the images
- Normalize pixel values
- Convert labels to one-hot encoding
- Build the baseline MLP
- Train the model
- Evaluate the model
- Generate evaluation metrics
- Perform RandomizedSearchCV hyperparameter optimization
- Retrain the optimized model
- Compare baseline and optimized models
- Generate all required plots

## Additional Exercise – XOR using Single Layer Perceptron

- Initialize weights and bias
- Implement the Step Activation Function
- Apply the Perceptron Learning Rule
- Display weights after each update
- Plot the decision boundary after each weight update
- Analyze the oscillating decision boundary
- Demonstrate the non-convergence of the perceptron on the XOR dataset

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

### Additional Exercise

The Single Layer Perceptron fails to converge on the XOR dataset because the classes are **not linearly separable**. The weights continue to change during training, and the decision boundary oscillates without reaching a stable solution, demonstrating the fundamental limitation of the Single Layer Perceptron.

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
- XOR Gate Decision Boundaries

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

1. Goodfellow et al., *Deep Learning*, MIT Press, 2016.
2. Bishop, *Pattern Recognition and Machine Learning*, Springer, 2006.
3. Haykin, *Neural Networks and Learning Machines*, Pearson, 2009.
4. Fashion-MNIST Dataset.
5. TensorFlow/Keras Documentation.

---

## Author

**Sadhana Sundaresan**
