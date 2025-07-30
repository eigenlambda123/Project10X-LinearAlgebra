# **Column & Null Space Explorer**

## Overview

This project is an interactive tool for exploring **column space** and **null space** of matrices — two fundamental subspaces in linear algebra (Chapter 3 of Strang’s book).

It allows you to compute bases, validate the **Rank-Nullity Theorem**, and visualize the geometry of subspaces in 2D and 3D. The entire toolset is implemented in **pure Python** using `numpy` and `matplotlib`, and designed as part of the **Project10X – Linear Algebra** series.

---

## Functionalities

### 1. **Compute Column Space Basis**

* Find a basis for the **column space** of matrix \$A\$ using column pivoting via elimination.
* Input: Matrix \$A\$
* Output: List of linearly independent column vectors spanning the column space.
* Function: `get_column_space_basis(A)`

---

### 2. **Compute Null Space Basis**

* Extract a basis for the **null space** of matrix \$A\$ by solving \$Ax = 0\$ using Gaussian elimination and backsolving.
* Input: Matrix \$A\$
* Output: List of vectors that span the null space (kernel) of \$A\$.
* Function: `get_null_space_basis(A)`

---

### 3. **Visualize Subspaces**

* For 2×2 and 3×3 matrices:

  * Visualize the **column space** as a span of vectors (in 2D or 3D)
  * Visualize the **null space** as a line/plane of solutions to \$Ax = 0\$
* Uses: `matplotlib` and `mpl_toolkits.mplot3d` for clean subspace rendering.
* Function: `visualize_subspaces(A)`

---

### 4. **Check Rank-Nullity Theorem**

* Validate the core relation:

  $$
  \text{rank}(A) + \text{nullity}(A) = \text{number of columns of } A
  $$

* Prints the rank, nullity, and verifies that the relation holds.

* Function: `check_rank_nullity(A)`

---

### 5. **Main CLI Interface**

* A simple command-line interface for testing all core features interactively.
* Built for notebooks or terminal sessions.
* Function: `main_menu()`

---

## Implementation Details

* Modular design using plain functions and `numpy` arrays.
* All matrix operations handled with row-reduction, elimination, and dot products.
* Designed to support experimentation, learning, and geometric intuition.

### Dependencies

* `numpy`
* `matplotlib`
