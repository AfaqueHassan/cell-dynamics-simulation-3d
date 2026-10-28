# 🧪 Cell Dynamics Simulation (CDS) Diblock Copolymer 3D Dashboard
> **19-Point & 55-Point Stencil Cylindrical Mesh Discretization Suite**

An advanced, interactive 3D Web Application built using **Three.js**, **GLSL Shaders**, **Tailwind CSS**, and **JavaScript** to visualize Cell Dynamics Simulations (CDS) for Diblock Copolymer microphase separation in cylindrical confinement.

---

## 🌟 Key Features

* **Dual Stencil Engine (19-Point vs 55-Point):**
  * Seamlessly switch between **19-Point Stencil** and high-precision **55-Point Stencil** cylindrical Laplacian operators ($\nabla^2 u$).
  * Real-time update of mathematical weighting factors ($w$), spatial discretizations, and numerical convergence dynamics.

* **6-in-1 Complete Thesis Figure Visualizer:**
  * **Fig 14:** Lamellae Forming System (Neutral Surfaces)
  * **Fig 16:** Cylindrical Forming System (Neutral Pores)
  * **Fig 18:** Spherical Forming System (Neutral Confinement)
  * **Fig 22:** Cylindrical Perforated Wall System
  * **Fig 23:** Cylindrical Helical System (Attractive Boundary)
  * **Fig 24:** Spherical Beads System (Attractive Surface)

* **12 Standard Projection Angles (a to l):**
  * Immediate camera repositioning for Front, Back, Top, Bottom, Right, Left, Diagonal, Off-Diagonal, Off-Front, Off-Back, Top-Bottom, and Off-Bottom views.

* **Interactive CDS Parameter Control:**
  * Real-time sliders & inputs for Nonlinear term ($A$), Diffusion ($D$), Long-range parameter ($B$), Order Parameter ($\tau$), Block Fraction ($f$), Volume Ratios ($u, v$), Height ($h$), and Interior Radius ($r_a$).

* **Scientific Visualization Tools:**
  * Real-time 2D Cross-Section (XY-Plane) preview.
  * Live console execution log & step counter ($t = 1,000,000$ steps).
  * Direct export of simulation output in **VTK Format** for ParaView analysis.

---

## 📐 Mathematical Formulation

### 1. Weighting Factor ($w$)
* **19-Point Stencil:**
  $$w = \frac{6 r^2 (\Delta r)^2 (\Delta\theta)^2 (\Delta z)^2}{4(r^2 (\Delta\theta)^2 (\Delta z)^2 + (\Delta r)^2 (\Delta z)^2 + r^2 (\Delta r)^2 (\Delta\theta)^2)}$$

* **55-Point Stencil:**
  $$w = \frac{1800 r^2 (\Delta r)^2 (\Delta\theta)^2 (\Delta z)^2}{980 r^2 (\Delta\theta)^2 (\Delta z)^2 + (\Delta r)^2 (\Delta z)^2 + r^2 (\Delta r)^2 (\Delta\theta)^2}$$

### 2. Time Evolution Equation
$$\Delta\psi = D \nabla^2 [-A \tanh(\psi) + \psi] - B(\psi - f) + \eta$$

---

## 🚀 How to Run Locally

Click on link:
  https://afaquehassan.github.io/cell-dynamics-simulation-3d/
