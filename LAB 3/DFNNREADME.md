# Deep Feed-Forward Neural Network for Multi-Class Classification

## Aim

The aim of this project is to implement a **Deep Feed-Forward Neural Network (DFNN)** from scratch using Python and NumPy for multi-class classification. The model classifies forest areas into different forest cover types using the given input features.

## Dataset Used

**Dataset:** Forest Cover Type (Covertype) Dataset

* Number of samples: **581,012**
* Number of input features: **54**
* Number of classes: **7**
* Classes: Forest Cover Types 1 to 7
* Dataset source: **UCI Machine Learning Repository**

The dataset is divided into **80% training, 10% validation, and 10% testing** using stratified splitting. The features are standardized before training.

## Model

The implemented DFNN has the following architecture:

```text
54 Input Features
       ↓
64 Neurons + ReLU
       ↓
32 Neurons + ReLU
       ↓
16 Neurons + ReLU
       ↓
7 Output Neurons + Softmax
```

The model uses **He initialization, weighted categorical cross-entropy, backpropagation, mini-batch SGD, and early stopping**.

## Results

The trained model is evaluated on the unseen test dataset using:

* Accuracy
* Precision
* Recall
* F1-score
* Macro Precision
* Macro Recall
* Macro F1-score
* Confusion Matrix

The notebook also generates training/validation loss and accuracy graphs, per-class F1 scores, precision-vs-recall comparison, and true-vs-predicted class distribution graphs.

**Note:** The exact numerical results are generated when the notebook is executed and may vary slightly depending on the environment and training run.

## Requirements

```text
Python 3
NumPy
Pandas
Scikit-learn
Matplotlib
Seaborn
ucimlrepo
```

Install the required packages using:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn ucimlrepo
```

## How to Run

Open the Jupyter Notebook:

```text
DFNN_Covertype_Complete_Assignment.ipynb
```

Run all cells from top to bottom. The dataset will be loaded, the DFNN will be trained, and the evaluation results and graphs will be generated automatically.
