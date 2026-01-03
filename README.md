# QuantumML

A toy example comparing classical and quantum machine learning kernels for binary classification on XOR data.


## Kernel Functions

Kernel functions map data to higher-dimensional spaces:

$$k(\vec{x}_i, \vec{x}_j) = \langle f(\vec{x}_i), f(\vec{x}_j) \rangle$$


## Quantum Kernels

Quantum kernels use quantum feature maps $\phi(\vec{x})$ to compute fidelity between quantum states:

$$K_{ij} = \left| \langle \phi(\vec{x}_i) | \phi(\vec{x}_j) \rangle \right|^2$$

This allows quantum computers to explore exponentially large feature spaces efficiently.


## What It Does

- **classicTrain.py**: Standard SVM with linear kernel on XOR dataset
- **quantumTrain.py**: SVM with quantum kernel (ZZFeatureMap) on same data

Quantum kernels leverage superposition and entanglement to explore higher-dimensional feature spaces for non-linear classification.