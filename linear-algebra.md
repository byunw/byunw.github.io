On this page, I explain concepts using mathematical notation. 
What I write on this page is the representation of my understanding.

## What is a scalar?

$$
x \in \mathbb{R}
$$

---

## What is a vector?

$$
\mathbf{v} = (v_1, v_2, \dots, v_n)
$$

where

$$
v_i \in \mathbb{R}
$$


## What is a matrix?

$$
A =
\begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mn}
\end{bmatrix}
$$

where

$$
a_{ij} \in \mathbb{R}
$$

## What is dot product?
Let

$$
\mathbf{u}, \mathbf{v} \in \mathbb{R}^n
$$

be two vectors.

The dot product is defined as

$$
\mathbf{u} \cdot \mathbf{v}
=
\sum_{k=1}^{n} u_k v_k
$$


## What is transpose?

Let

$$
A \in \mathbb{R}^{m \times n}
$$

Then the transpose of \( A \) is denoted by

$$
A^T \in \mathbb{R}^{n \times m}
$$

where

$$
(A^T)_{ij} = A_{ji}
$$

## What is matrix multiplication?

Let

$$
A \in \mathbb{R}^{m \times n}
\quad \text{and} \quad
B \in \mathbb{R}^{n \times p}.
$$

The **matrix product** of \(A\) and \(B\) is the matrix

$$
C = AB,
$$

where

$$
C \in \mathbb{R}^{m \times p}.
$$


## What is Eigenvalue and Eigenvector?
Let

$$
A \in \mathbb{R}^{n \times n}
$$

and

$$
\mathbf{v} \neq \mathbf{0}
$$

Then

$$
\lambda \in \mathbb{R}
$$

is called an eigenvalue of A and
$$
\mathbf{v}
$$

is called an eigenvector of A if 

$$
A\mathbf{v} = \lambda \mathbf{v}
$$. 

