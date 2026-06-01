# Approximation Node Optimizer (ANO)

Open-source computing engine and research tools for generating, analyzing, and visualizing optimal interpolation and quadrature nodes (Approximate Fekete Points and Leja Sequences) on complex 2D/3D geometries.

## 🚀 Features

* **Advanced Node Generation:** Implements discrete Fekete points via QR factorization with column pivoting (Sommariva & Vianello framework) and Leja sequences using orthogonal projections (Luu's method).
* **Flexible Geometries:** Support for custom domains, including standard intervals/squares, complex non-convex 2D shapes (`SectorDisk`), and 3D manifolds (spheres, cylinders, tori).
* **Interactive UI:** Built-in interactive visualization tools (`ipywidgets`) to manipulate nodes and analyze Lebesgue constants in real time.
* **Academic Integration:** Automations for recording experiment data and exporting formatted LaTeX tables directly.

## 🛠️ Tech Stack

* **Core Engine:** Python 3.10+
* **Libraries:** NumPy, SciPy (LAPACK `DGEQP3` bindings), Matplotlib, ipywidgets

## 📚 Theoretical Background

This project is based on the discrete optimization framework proposed by A. Sommariva and M. Vianello (2009) for computing approximate Fekete points using numerical linear algebra tools, combined with iterative refinement techniques for multidimensional domains and Bos-Levenberg asymptotic theorem.
