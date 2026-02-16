# Monte Carlo Simulation for European Option Pricing  
### Numerical Methods Final Project

This repository contains a Jupyter notebook implementing a Monte Carlo framework for pricing European call and put options under Geometric Brownian Motion (GBM). The project focuses on numerical accuracy, variance reduction, and validation against analytical benchmarks.

## Notebook
**final_project.ipynb**  
A self‑contained notebook including simulation code, visualizations, and validation tests.

## Overview
We model asset prices using GBM and estimate option values by simulating thousands of price paths and discounting terminal payoffs. To improve estimator efficiency, we incorporate antithetic variates and construct confidence intervals to quantify uncertainty. Results are compared against the closed‑form Black–Scholes formula to verify correctness.

## Key Techniques
- Geometric Brownian Motion simulation  
- Monte Carlo pricing for European options  
- Variance reduction (antithetic variates)  
- Confidence intervals and error analysis  
- Analytical Black–Scholes benchmark  
- Convergence and edge‑case checks (σ → 0, T → 0, put–call parity)

## Main Findings
- Monte Carlo estimates converge to Black–Scholes prices with error scaling as $\(1/\sqrt{N}\)$.  
- Antithetic variates significantly reduce variance at no additional computational cost.  
- Edge‑case tests and parity checks confirm numerical correctness and stability.

## 📚 References
Black & Scholes (1973), Brewer–Feng–Kwan (GBM simulation notes), Zariphopoulou (derivative valuation primer)
