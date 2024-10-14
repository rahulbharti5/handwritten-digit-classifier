# Handwritten-Digit-Classification-Using-ANN

A neural network built from scratch to classify handwritten digits from the MNIST dataset.

- **Technologies Used**: numpy
- **Highlights**:
  - Custom architecture with 3 dense layers
  - Achieved 98% accuracy
  - Confusion matrix and prediction examples

## 1. Model Architecture

![alt text](image.png)

We assume the image data of 28x28 is flatern into 784x1 dimension:

## 2. Forword Propagation

\begin{align*}
\begin{bmatrix}
w*{11} & w*{12} & \cdots & w*{1,783} & w*{1,784} \\
w*{21} & w*{22} & \cdots & w*{2,783} & w*{2,784} \\
\vdots & \vdots & \ddots & \vdots & \vdots \\
w*{15,1} & w*{15,2} & \cdots & w*{15,783} & w*{15,784} \\
w*{16,1} & w*{16,2} & \cdots & w*{16,783} & w*{16,784}
\end{bmatrix}*{16 \times 784}
\odot
\begin{bmatrix}
x_1 \\
x_2 \\
x_3 \\
\vdots \\
x*{783} \\
\end{bmatrix}*{783 \times 1} +
\begin{bmatrix}
b_1 \\
b_2 \\
b_3 \\
\vdots \\
b*{16}
\end{bmatrix}*{16 \times 1}
=
\begin{bmatrix}
z_1 \\
z_2 \\
z_3 \\
\vdots \\
z*{16}
\end{bmatrix}\_{16 \times 1}
\end{align*}
