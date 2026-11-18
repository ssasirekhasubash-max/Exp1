# Experiment 1: Exploring NumPy and Pandas

## Aim

To understand the use of NumPy and Pandas for performing basic data
manipulation and analysis in Python.

## Algorithm

1.  Import the NumPy library for matrix and numerical operations.
2.  Define a two-dimensional square matrix `A` and a vector `b`.
3.  Compute the transpose of matrix `A` to interchange rows and columns.
4.  Calculate the inverse of matrix `A` using `np.linalg.inv(A)` (ensure
    `A` is non-singular).
5.  Solve the linear equation `A × x = b` using `np.linalg.solve(A, b)`.
6.  Perform eigen decomposition to find eigenvalues and eigenvectors
    using `np.linalg.eig(A)`.
7.  Display the results for the matrix, transpose, inverse, solution
    vector, and eigenvalues.
8.  End the program.

## Formulas / Theory

-   **Transpose:** `Aᵀ` --- interchange rows and columns.
-   **Inverse:** `A⁻¹ = adj(A) / |A|`, provided `det(A) ≠ 0`.
-   **Linear system:** `A × x = b  ⇒  x = A⁻¹b`.
-   **Eigen decomposition:** `A v = λ v`, where `λ` is an eigenvalue and
    `v` is an eigenvector.

## Coding
import numpy as np
import pandas as pd

# Create a matrix and vector
A = np.array([[2, 1], [1, 3]])
b = np.array([5, 6])

# Transpose
transpose = np.transpose(A)

# Inverse
inverse = np.linalg.inv(A)

# Solve linear equations
solution = np.linalg.solve(A, b)

# Eigenvalues and eigenvectors
eigenvalues, eigenvectors = np.linalg.eig(A)

# Display results
print("Original Matrix:\n", A)
print("Transpose:\n", transpose)
print("Inverse:\n", inverse)
print("Solution:\n", solution)
print("Eigenvalues:\n", eigenvalues)
print("Eigenvectors:\n", eigenvectors)

## Output
Original Matrix:
 [[2 1]
 [1 3]]
Transpose:
 [[2 1]
 [1 3]]
Inverse:
 [[ 0.6 -0.2]
 [-0.2  0.4]]
Solution:
 [1.8 1.4]
Eigenvalues:
 [1.38196601 3.61803399]
Eigenvectors:
 [[-0.85065081 -0.52573111]
 [ 0.52573111 -0.85065081]]

## Result
Thus, NumPy and Pandas libraries were studied for basic data manipulation and analysis. Matrix transpose, inverse, linear equation solving, and eigenvalue calculations were successfully performed using Python.
