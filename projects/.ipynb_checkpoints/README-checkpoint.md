# Vector Visualizer

A 2D interactive tool for visualizing vector operations in linear algebra, including vector addition, scalar multiplication, linear combinations, and span. This project is part of the **Project10X–Linear** learning series and was built to develop geometric intuition behind symbolic operations.

## Overview

Traditional linear algebra focuses on symbolic manipulation, but often lacks geometric intuition. This project was created to bridge that gap. By visualizing vector behavior and how they generate lines or planes through linear combinations, users can gain a deeper understanding of vector spaces, independence, and basis.

The visualizer uses Python, Matplotlib, and Jupyter widgets to provide an interactive experience that helps learners connect algebraic operations with visual outcomes.

## Features and Functionalities

* **2D Vector Plotting**
  Display vectors from the origin on a Cartesian plane.

* **Vector Addition Visualization**
  Illustrate head-to-tail addition to show resultant vectors.

* **Scalar Multiplication**
  Scale vectors by any real number and observe stretching or compression.

* **Interactive Linear Combination**
  Use sliders to adjust scalars `a` and `b` for the combination `a*v + b*w`, showing the resulting vector in real time.

## Tools and Technologies

* Python 3
* Matplotlib (for plotting)
* ipywidgets (for interactivity in Jupyter)
* NumPy (for vector calculations)

## How to Use

1. Clone the repository or download the notebook file.
2. Open it in a Jupyter environment.
3. Define two 2D vectors `v` and `w`.
4. Use the `interactive_linear_combination()` method to explore vector combinations.
5. Use the `span_demo([v, w])` function to visualize the area spanned by `v` and `w`.

## Educational Use Cases

* Understand how vectors behave under addition and scaling.
* See how two vectors can generate a subspace (line or plane).
* Explore the effect of different scalar coefficients on linear combinations.
* Support learning around linear independence, span, and geometric intuition in vector spaces.

## Potential Extensions

* 3D vector visualization and Calculations
* Span Demonstration
* Basis change visualization
* Matrix transformation demos
* Step-by-step animations or guided tutorials