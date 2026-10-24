# 📈 Black–Scholes Option Pricing Model (Python)

This project implements the **Black–Scholes option pricing model** in Python to calculate theoretical prices of European Call and Put options.
It also computes volatility from real stock data and visualizes option behavior using plots.

The notebook fetches live financial data using Yahoo Finance and applies core mathematical finance concepts in a practical way.

---

## 🚀 Features

✅ Fetches real stock data using `yfinance`
✅ Calculates **log returns**
✅ Computes **annualized volatility**
✅ Implements the **Black–Scholes formula for Call & Put options**
✅ Plots option prices and stock movement
✅ Uses `scipy` for probability distributions
✅ Designed for learning and experimentation

---
## 📘 Black–Scholes Formula

### 📈 Call Option

<p align="center">
<b>C = S N(d₁) − K e<sup>−rt</sup> N(d₂)</b>
</p>

### 📉 Put Option

<p align="center">
<b>P = K e<sup>−rt</sup> N(−d₂) − S N(−d₁)</b>
</p>

### 📐 Definitions

<p align="center">
<b>d₁ = [ ln(S/K) + (r + σ² / 2)t ] / ( σ√t )</b>
</p>

<p align="center">
<b>d₂ = d₁ − σ√t</b>
</p>


---

## 📂 Project Structure

```
Black-Scholes/
│
├── Black_scholes.ipynb     # Main notebook
├── README.md              # Documentation
```

---

## 📦 Requirements

Install dependencies using:

```bash
pip install numpy pandas matplotlib yfinance scipy
```

---

## ▶️ How to Run

1. Download or clone the repository:

```bash
git clone https://github.com/Hrushi1812/Option-Pricing-model.git
```

2. Open the notebook:

```bash
jupyter notebook Black_scholes.ipynb
```

3. Run each cell step-by-step.

---

## 📊 Important Functions in the Notebook

### 🔹 Annual Volatility

```python
def annual_vol(df):
```

Calculates volatility using log returns.

---

### 🔹 Black–Scholes Call Price

```python
def call_option_price(S, K, r, t, sigma):
```

Calculates European Call option price.

---

### 🔹 Black–Scholes Put Price

```python
def put_option_price(S, K, r, t, sigma):
```

Calculates European Put option price.

---

## 🎯 Why Log Returns Instead of Normal Returns?

Log returns are preferred because:

* Time additive
* More stable variance
* Handles compounding naturally
* Better for modeling price behavior mathematically

---

## 🧠 Learning Outcomes

By completing this notebook, you will understand:

* Option pricing fundamentals
* Volatility estimation
* Risk-free rate impact
* Application of probability distributions
* How theory meets real data

---

## ⚠️ Limitations of Black–Scholes

While powerful, the model assumes:

* Constant volatility
* No dividends
* Efficient markets
* European options only

Real markets may deviate significantly.

---

## 🙌 Acknowledgement

Built using:

* `scipy`
* `pandas`
* `yfinance`
* `matplotlib`

---

## 👨‍💻 Author

**HrushiKesh Peddi**
Undergraduate Student
FinTech & Quant Finance Enthusiast

---

## 📬 Suggestions?

Open an issue or contact if you'd like:

✔ Greeks added
✔ Monte Carlo simulation
✔ Implied volatility calculator
✔ Interactive dashboard
✔ Strategy builder
