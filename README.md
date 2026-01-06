# Data-Driven $p$-Norms for Estimating Transmission Loss Coefficients in Power Systems

This repository contains the implementation and data for the paper *"Data-Driven $p$-Norms for Estimating Transmission Loss Coefficients in Power Systems"*.

## 🔍 Overview
We introduce a novel convex, data-driven methodology for estimating transmission loss coefficients (\(B\)-coefficients) in power systems. A key contribution is the incorporation of stochastic demand behavior, which significantly improves estimation accuracy. The proposed model is formulated as a semidefinite programming (SDP) problem using general \(p\)-norm objective functions, ensuring physical consistency through convex constraints.

## ✨ Key Features
- **Data-driven estimation** of \(B_{20}\) (quadratic), \(B_{10}\) (linear), and \(B_{00}\) (constant) loss coefficients from system measurements.
- **Stochastic modeling** of demand using uniform and Gaussian distributions to mimic real-world variability.
- **Convex SDP formulation** with \(p\)-norm objectives (\(p = 1, 2, 3, \infty\)) that guarantees global optimality and numerical stability.
- **Physical constraints** including positive semidefinite \(B_{20}\), nonnegative diagonals, and bounded constant loss term.
- **Validation on standard test systems**: IEEE 14-, 39-, 57-, and 118-bus networks.

## 📊 Results
Numerical evaluations show average estimation errors between \(-6\%\) and \(5\%\) across different test scenarios, demonstrating the robustness and accuracy of the proposed methodology.

## 🛠️ Implementation
- **Language & Tools**: MATLAB R2025b, MATPOWER 8.1
- **Optimization**: YALMIP with MOSEK solver
- **Systems**: Tested on IEEE 14-, 39-, 57-, and 118-bus networks
- **Data**: Includes training datasets (satisfying \(m > N_g(N_g+3)/2\)) and separate validation sets (1000 random operating points per system)

## 📝 Citation
If you use this code or data in your research, please cite the corresponding paper.
