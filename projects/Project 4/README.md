# **Matrix Operation Simulator**

## Overview

This project is an interactive tool for performing and experimenting with **fundamental matrix operations** — essential building blocks of linear algebra.
It covers arithmetic, transformations, and utility operations, all implemented in **pure Python** with `numpy`.
Part of the **Project10X – Linear Algebra** series, it’s designed for both **learning** and **quick experimentation**.

---

## Functionalities

### 1. **Matrix Addition**

* Perform element-wise addition between two matrices of the same size.
* Input: Matrices `A`, `B`
* Output: `A + B`
* Function: `add_matrices(A, B)`

---

### 2. **Scalar Multiplication**

* Multiply every entry in a matrix by a given scalar.
* Input: Matrix `A`, scalar `k`
* Output: `k * A`
* Function: `scale_matrix(A, k)`

---

### 3. **Matrix Multiplication**

* Multiply two matrices using the standard dot product rule.
* Input: Matrices `A`, `B` (compatible dimensions)
* Output: `A × B`
* Function: `multiply_matrices(A, B)`

---

### 4. **Identity Matrix Generator**

* Create an identity matrix of size `n × n`.
* Input: Integer `n`
* Output: Identity matrix `Iₙ`
* Function: `identity_matrix(n)`

---

### 5. **Matrix Inverse**

* Compute the inverse of a square, non-singular matrix.
* Input: Matrix `A`
* Output: `A⁻¹`
* Function: `inverse_matrix(A)`

---

### 6. **Matrix Power**

* Raise a square matrix to an integer power (positive, zero, or negative if invertible).
* Input: Matrix `A`, integer `p`
* Output: `Aᵖ`
* Function: `matrix_power(A, p)`

---

### 7. **Matrix Transpose**

* Swap the rows and columns of a matrix.
* Input: Matrix `A`
* Output: `Aᵀ`
* Function: `transpose_matrix(A)`

---

### 8. **Row Permutation**

* Swap two specific rows in a matrix.
* Input: Matrix `A`, `row1`, `row2`
* Output: Matrix with `row1` and `row2` swapped.
* Function: `permute_rows(A, row1, row2)`

---

### 9. **Main CLI Interface**

* Interactive terminal menu to access all operations.
* Allows repeated experiments without restarting.
* Function: `main_menu()`

---

## Implementation Details

* **Modular function-based design** — each operation is independent.
* Built entirely with **NumPy** for speed and reliability.
* Focused on **educational clarity** with readable, well-commented code.

### Dependencies

* `numpy`
