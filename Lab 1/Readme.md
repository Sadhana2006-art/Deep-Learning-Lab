# Experiment 1: Single Layer Perceptron for Binary Classification

## Objective

This experiment implements a **Single Layer Perceptron** from scratch to perform binary classification on the **Banknote Authentication Dataset**. The objective is to understand the working of an artificial neuron, the perceptron learning algorithm, and the effect of different learning rates on model performance.

---

## Dataset

- **Dataset:** Banknote Authentication Dataset
- **Source:** UCI Machine Learning Repository
- **Instances:** 1372
- **Features:**
  - Variance
  - Skewness
  - Curtosis
  - Entropy
- **Target Classes:**
  - 0 – Authentic Banknote
  - 1 – Forged Banknote

---

## Features Implemented

- Dataset exploration
- Exploratory Data Analysis (EDA)
  - Histograms
  - Correlation Heatmap
  - Scatter Plot
  - Box Plot
- Data preprocessing using MinMaxScaler
- Train-Test Split (80:20)
- Single Layer Perceptron implemented from scratch
- Step Activation Function
- Perceptron Learning Rule
- Model evaluation using:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix
- Training Error vs Epoch
- Weight Evolution
- Bias Evolution
- Learning Rate Comparison (0.001, 0.01, 0.1)

---

## Project Structure

```
Lab 1/
│── Single_Layer_Perceptron.ipynb
│── Experiment_1.tex
│── Experiment_1.pdf
│── Histogram.eps
│── Correlation_Heatmap.eps
│── Scatter_Plot.eps
│── Box_Plot.eps
│── Confusion_Matrix.eps
│── Training_Error_vs_Epoch.eps
│── Weight_Evolution.eps
│── Bias_Evolution.eps
│── Learning_Rate_Comparison.eps
│── README.md
```

---

## Requirements

Install the required Python libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

Or in Google Colab:

```python
!pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/Sadhana2006-art/Deep-Learning-Lab.git
```

2. Navigate to the Lab 1 folder:

```bash
cd Deep-Learning-Lab/Lab\ 1
```

3. Open the notebook:

- **Google Colab:** Upload `Single_Layer_Perceptron.ipynb`
- **Jupyter Notebook:**

```bash
jupyter notebook
```

4. Run all cells sequentially.

The notebook will:
- Load the dataset
- Perform EDA
- Normalize the features
- Train the perceptron
- Evaluate the model
- Generate all required plots
- Save plots in **EPS format (600 dpi)**

---

## Results

The implemented perceptron achieved high classification performance on the Banknote Authentication Dataset.

Performance metrics include:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Additional analyses include:
- Training Error vs Epoch
- Weight Evolution
- Bias Evolution
- Learning Rate Comparison

---

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

---

## Author

**Sadhana Sundaresan**

B.Tech Artificial Intelligence and Data Science
