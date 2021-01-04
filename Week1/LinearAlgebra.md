# Linear Algebra - Matrix Operations

## Matrix vs Vector

- Matrix, a 2D array of arrays

  - Dimension of Matrix = (# of row) x (# of columns)

- Vector, a matrix with only one column and many rows

## Matrix Addition and Subtraction

- Add and subtracting are element-wise, so you simply add or subtract each corresponding element
- Both elements have to have the **same dimension**

$$
\begin{bmatrix}
1 & 0 \\
2 & 5 \\
3 & 1
\end{bmatrix}
+
\begin{bmatrix}
4 & 0.5 \\
2 & 5 \\
0 & 1
\end{bmatrix}
=
\begin{bmatrix}
5 & 0.5 \\
4 & 10 \\
3 & 2
\end{bmatrix}
$$

## Scalar Multiplication and Division

- Scalar Value, a real number
  
- In Scalar Multiplication and Division, you simply apply the operation to each element in the matrix by the scalar value.

- Scalar Multiplication is a commutative

$$
3 \times
\begin{bmatrix}
1 & 0 \\
2 & 5 \\
3 & 1
\end{bmatrix}
=
\begin{bmatrix}
3 & 0 \\
6 & 15 \\
9 & 3
\end{bmatrix}
=
\begin{bmatrix}
1 & 0 \\
2 & 5 \\
3 & 1
\end{bmatrix}
\times 3
$$

$$
3 \div
\begin{bmatrix}
4 & 0 \\
6 & 3 \\
\end{bmatrix}
=
\begin{bmatrix}
1 & 0 \\
\frac{3}{2} & \frac{3}{4} \\
\end{bmatrix}
$$

## Matrix-Vector Multiplication

- Product of a $(m\times n)$ matrix and  $(n\times 1)$ vector should be a vector with $(m\times 1)$ dimension

- The **number of columns of the matrix** must equal the **number of rows of the vector**

## Matrix-Matrix Multiplication

- Given $M_a\times M_b$, representing two matrixes
  1. Break the columns in a $M_b$ down into vectors
  2. Perform Matrix-Vector Multiplication on $M_a$ with each column in $M_b$.
  3. Combine the product vectors to form answer matrix

- Matrix-Matrix multiplying is not commutative
- Matrix-Matrix multiplying is associative

## Identity Matrix

- $I$, denotes a Identity Matrix

- A square matrix that has a value of $1$ on the diagonal and $0$ everywhere else

- For any matrix $A$...
  - $A \times I = I \times A = A$
  
$$
\begin{bmatrix}
  1
\end{bmatrix}

\begin{bmatrix}
  1 & 0 \\
  0 & 1 \\
\end{bmatrix}

\begin{bmatrix}
  1 & 0 & 0 \\
  0 & 1 & 0 \\
  0 & 0 & 1 \\
\end{bmatrix}

\begin{bmatrix}
  1 & 0 & 0 & 0 \\
  0 & 1 & 0 & 0 \\
  0 & 0 & 1 & 0 \\
  0 & 0 & 0 & 1 \\
\end{bmatrix}
$$  

## Inverse

- Only a square matrix can have a inverse matrix

- Singular or Degenerate, a matrix that does not have a inverse

- Typically use Matlab or python function to find the inverse of a matrix
  - inv(int) in Matlab

## Transposition

- $A^T$, denotes a matrix $A$ that has been transposed

- Given matrix $A$ with dimensions $m \times n$, then $A^T$ will have dimensions $n \times m$

$$
A =
\begin{bmatrix}
  1 & 2 & 0 \\
  3 & 5 & 9 \\
\end{bmatrix}
\rightarrow
A^T =
\begin{bmatrix}
  1 & 3 \\
  2 & 5 \\
  0 & 9 \\
\end{bmatrix}
$$
