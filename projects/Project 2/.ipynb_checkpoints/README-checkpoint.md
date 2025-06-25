## Overview

This project is an interactive linear system solver that demonstrates core concepts from Chapter 2 of linear algebra: **representing systems as $Ax = b$**, performing **Gaussian Elimination**, **detecting solution types**, **solving with back substitution**, and **visualizing equations as geometric objects**.

It is implemented in pure Python using `numpy` and `matplotlib`, and structured for Jupyter notebooks as part of the **Project10X – Linear Algebra** series.

---

## Functionalities

### 1. **Gaussian Elimination**

- Reduce a system $Ax = b$ to Row Echelon Form (REF) using step-by-step elimination.
- Input: Matrix `A`, vector `b`.
- Output: Transformed augmented matrix and detailed elimination log.
- Uses: `GaussianEliminator` class with `.eliminate()` and `.print_steps()` methods.

---

### 2. **Solution Type Detection**

- Automatically classify whether the system has:
    - A **unique solution**
    - **Infinite solutions**
    - **No solution**

- Uses rank comparison:  
    $\text{rank}([A|b])$ vs number of unknowns.

- Function: `detect_solution_type(A, b)`

---

### 3. **Back Substitution**

- Solve the system when matrix is in upper-triangular form (from Gaussian elimination).
- Input: Upper-triangular matrix `U`, vector `b`.
- Output: Final solution vector and step-by-step substitution breakdown.
- Function: `back_substitution_with_steps(U, b)`

---

### 4. **2D and 3D Visualization**

- Geometrically visualize each equation:
    - As **lines** in 2D $(for \ 2×2)$
    - As **planes** in 3D $(for \ 3×3)$

- Highlights the solution as the intersection of lines or planes, if it exists.
- Function: `visualize_elimination(A, b)`

---

## Implementation Details

- All features are modular and built around clean, testable functions and classes.
- Main interface: `main_menu()` — CLI for testing and demonstration.
- Primary libraries used: `numpy`, `matplotlib.pyplot`, and `mpl_toolkits.mplot3d`.
