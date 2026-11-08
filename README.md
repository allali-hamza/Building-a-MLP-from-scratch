# Building a MLP from Scratch

This project implements a simple Multi-Layer Perceptron (MLP) with one hidden
layer. The complete work is in `MLP.ipynb`.

## Content

The notebook includes:

- A manual linear classifier for the `make_moons` dataset.
- A comparison with logistic regression.
- A two-layer MLP built with Python lists.
- Sigmoid, softmax, cross-entropy loss and backpropagation.
- Training on the scikit-learn digits dataset.
- A training/validation split and hyperparameter comparison.
- An overfitting example.
- A NumPy version of the MLP and a speed comparison with the list version.

## Installation

Install the required packages:

```bash
pip install -r requirements.txt
```

Open the notebook:

```bash
jupyter notebook MLP.ipynb
```

Run all cells from top to bottom.

If the first cell reports an error for `sklearn`, install `scikit-learn`:

```bash
pip install scikit-learn
```

## Results

On the two-moons dataset, logistic regression obtains about **85% accuracy**.
The MLP reaches about **96% accuracy** after 200 epochs because it can learn a
curved decision boundary.

For the digits dataset, the notebook tests nine configurations. The best one
uses **20 hidden neurons** and a learning rate of **0.001**, with about
**90.8% validation accuracy**.

In the final bonus, the Python-list and NumPy versions obtain the same
validation accuracy. The NumPy version is about **65 times faster**.

## Files

| File | Description |
| --- | --- |
| `MLP.ipynb` | Completed MLP project notebook. |
| `requirements.txt` | Python dependencies. |
