# Pricing European Options: A Comparison Between Black-Scholes and Monte Carlo Method

This repository contains my project for the **Python for Finance** course (MSc in Finance, University of Siena, 2024-2025).  
The goal is to compare two different approaches for pricing **European call and put options**:

- **Black-Scholes Model** (closed-form solution)  
- **Monte Carlo Simulation** (numerical approximation)

---

## 📄 Project Description

Options are derivative instruments that give the right, but not the obligation, to buy (call) or sell (put) an underlying asset at a predetermined price (strike) at maturity.  
In this project:

- The **Black-Scholes model** is implemented as a reference closed-form pricing formula.  
- The **Monte Carlo method** simulates multiple paths of the underlying asset using a **Geometric Brownian Motion (GBM)** to approximate the option value.  
- A **comparison** is made between the two methods in terms of accuracy and convergence.  
- A **sensitivity analysis** on volatility shows how option prices evolve when the underlying risk parameter changes.

---

## 📊 Results

- Black-Scholes and Monte Carlo methods provide **consistent estimates** for both call and put options.  
- The **absolute error** between the two approaches decreases as the number of simulations increases, confirming the convergence of Monte Carlo toward the theoretical value.  
- Sensitivity analysis confirms the expected monotonic relationship between volatility and option prices, with Monte Carlo tracking closely the Black-Scholes results.

---

## ⚙️ Requirements

The code relies on the following Python libraries:

- `numpy`  
- `scipy`  
- `matplotlib`  
- `IPython.display` (for Colab/Notebook output)

You can install them with:

```bash
pip install -r requirements.txt

