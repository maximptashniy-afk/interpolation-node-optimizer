# Approximation Node Optimizer (ANO)

Open-source mathematical computing engine designed for generating, analyzing, and comparing optimal multivariate interpolation configurations across complex multidimensional domains.

The framework evaluates and benchmarks multiple nodal distribution strategies to minimize the **Lebesgue constant** ($\Lambda_n$), effectively mitigating the Runge phenomenon in high-degree polynomial approximations.

---

## 🚀 Key Features

* **Comprehensive Nodal Solvers:** Benchmark and generate diverse algebraic node configurations:
  * *Approximate Fekete Points* (via the Sommariva & Vianello QR-factorization framework with column pivoting).
  * *Discrete Leja Sequences* (via sequential matrix determinant maximization).
  * *Analytical Profiles:* Padua points (for standard squares) and Bos points (for circular domains).
* **Flexible Geometries (1D, 2D, and 3D):** Fully abstracted domain structures with custom boundary tracking and spatial indicators:
  * *2D Manifolds:* Standard Squares, Unit Disks, 3/4 Circular Sectors, Flat and Round Dumbbells, Circular Annuli, and Disjoint Assemblies.
  * *3D Volumetric Spaces:* Spheres, Cylinders, and Solid Tori.
* **Interactive Laboratory:** Dynamic visualization interfaces (`ipywidgets`) enabling real-time manual node manipulation and instant tracking of phase-space operator norm shifts.
* **Academic Automation:** Seamless calculation of exact critical peak coordinates and automatic generation of fully formatted, journal-compliant LaTeX tabular source code blocks.

---

## 🛠️ Tech Stack

* **Core Language:** Python 3.10+
* **Numerical Computations:** NumPy, SciPy (leveraging LAPACK `DGEQP3` preconditioned bindings).
* **Visualization Suite:** Matplotlib (2D isoline contours and 3D topographic surface reliefs).
* **GUI Engine:** IPython Display & ipywidgets Framework.

---

## 📚 Theoretical Foundations

The computing engine integrates the discrete optimization principles established by *A. Sommariva and M. Vianello (2009)* for extractively computing Approximate Fekete Points using numerical linear algebra tools. 

Multivariate polynomial valuation matrices are constructed utilizing total-degree combinations of normalized Chebyshev polynomials mapped onto a strict $[-1.0, 1.0]$ canonical space. The stability pipelines validate nodal asymptotic behaviors under the Bos-Levenberg theorem across both standard and non-convex geometries.

---

## ⚙️ Project Structure & Execution

* `chebyshev_interpolation_engine.ipynb` — Core Google Colab notebook containing the complete framework architecture and validation benchmarks.
* `wykres_wzrostu_*.pdf` — Vector PDF growth tracking curves ($\Lambda_n$ vs. polynomial degree $n$).
* `mapa_lebesgue_*.pdf` — High-definition operator norm contour maps designed for direct academic publication inserts.

### Quick Start:
1. Open the `.ipynb` core engine notebook inside **Google Colab**.
2. Execute the environment initialization cell to purge any legacy file system artifacts.
3. Run the analytical pipelines for your designated geometric domain to extract the LaTeX logs and PDF visualization vectors.

---

## 📄 License

This project is open-source and licensed under the terms of the **MIT License**. See the [LICENSE](LICENSE) file for the full copyright and permission notice.
