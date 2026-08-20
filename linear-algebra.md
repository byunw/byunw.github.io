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

$$
\text{Let } A \text{ be an } m \times n \text{ matrix. The transpose of } A,
\text{ denoted by } A^T, \text{ is the } n \times m \text{ matrix whose columns
are the respective rows of } A.
$$

## Matrix Multiplication

In this section, let's just do matrix multiplication!

$$
\begin{bmatrix}
2 \\
5 \\
-3 \\
-2
\end{bmatrix}
\begin{bmatrix}
-2 & -5 & -4 & -1
\end{bmatrix}
=
\begin{bmatrix}
-4 & -10 & -8 & -2 \\
-10 & -25 & -20 & -5 \\
6 & 15 & 12 & 3 \\
4 & 10 & 8 & 2
\end{bmatrix}
$$

## Matrix Addition
In this section, let's just do matrix addition!

$$
\begin{bmatrix}
1 \\
2
\end{bmatrix}
+
\begin{bmatrix}
3 \\
5
\end{bmatrix}
=
\begin{bmatrix}
4 \\
7
\end{bmatrix}
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

