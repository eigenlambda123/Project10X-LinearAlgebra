# **Linear System Solver**

## Overview

This project is an interactive solver and visualizer for linear systems of equations, designed to reinforce core concepts from **Chapter 2 of Linear Algebra**:

* Representing systems as \$Ax = b\$
* Performing **Gaussian Elimination**
* **Classifying solution types** (unique, infinite, none)
* **Solving via back substitution**
* **Visualizing equations as geometric objects**

It is implemented in **pure Python** using `numpy` and `matplotlib`, and structured for interactive use in Jupyter notebooks. Part of the **Project10X – Linear Algebra** series.

---

## Functionalities

### 1. **Gaussian Elimination**

* Reduces the system \$Ax = b\$ to **Row Echelon Form (REF)** through forward elimination.
* Input: Matrix \$A\$, vector \$b\$
* Output: Augmented matrix in REF, along with step-by-step logs
* Class: `GaussianEliminator`
  Methods: `.eliminate()`, `.print_steps()`

---

### 2. **Solution Type Detection**

* Automatically detects whether the system has:

  * A **unique solution**
  * **Infinite solutions**
  * **No solution**

* Based on comparing ranks:

  $$\text{rank}([A|b]) \quad \text{vs} \quad \text{number of variables}$$

* Function: `detect_solution_type(A, b)`

---

### 3. **Back Substitution**

* Solves upper-triangular systems after elimination.
* Input: Upper-triangular matrix \$U\$, modified vector \$b\$
* Output: Solution vector \$x\$ and detailed substitution trace
* Function: `back_substitution_with_steps(U, b)`

---

### 4. **2D and 3D Visualization**

* Plots each equation:

  * As **lines** (2×2 systems)
  * As **planes** (3×3 systems)

* Illustrates how solutions emerge from the **intersection** of geometric objects.

* Function: `visualize_elimination(A, b)`

---

## Implementation Details

* Modular design using clean functions and classes
* Command-line driver: `main_menu()` for testing each feature
* Libraries used:

  * `numpy`
  * `matplotlib.pyplot`
  * `mpl_toolkits.mplot3d` (for 3D visuals)