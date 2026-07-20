# Black-Scholes Options Pricer

A Python implementation of the **Black-Scholes Options Pricing Model** for European options. This project calculates theoretical call and put option prices, analyzes option sensitivities (Greeks), estimates implied volatility, compares Black-Scholes prices with Monte Carlo simulation, and provides several visualizations for understanding option behavior.

---

## Features

- Black_scholes pricing for European call and put options
- Interactive user input with input validation
- Break-even price evaluation
- Sensitivity analysis for:
  - Volatility
  - Stock price
  - Time to expiry
- Option payoff and profit diagrams
- Greeks calculation:
  - Delta
  - Theta
  - Rho
  - Vega
  - Gamma
- Greeks visualization
- Implied volatility estimation using the Newton-Raphson method
- Monte Carlo simulation for option pricing
- Comparison between Black-Scholes and Monte Carlo

---

## Black-Scholes Model

\[
d_1=\frac{\ln(S/K)+(r+\frac{\sigma^2}{2})T}{\sigma\sqrt{T}}
\]

\[
d_2=d_1-\sigma\sqrt{T}
\]

Call Price:

\[
C=S\,N(d_1)-Ke^{-rT}N(d_2)
\]

Put Price:

\[
P=Ke^{-rT}N(-d_2)-SN(-d_1)
\]

---

## Project Structure

```

|
├── User input and validation
├── Black-Scholes pricing
├── Break-even analysis
├── Sensitivity analysis
├── Option payoff diagrams
├── Greeks calculation
├── Greeks visualization
├── Implied volatility estimation
└── Monte Carlo simulation

```
---

## Requirements

Install the required libraries

```bash
pip install pandas numpy matplotlib scipy
```
---

## Inputs

The notebook requires:

- Spot price (S)
- Strike price (K)
- Time to expiry (T)
- Risk-free interest rate (r)
- Volatility (sigma)

---

## Outputs

The notebook computes:

- Call option price
- Put option price
- Break-even prices
- Options Greeks
- Implied volatility
- Monte Carlo option prices

It also generates plots for:

- Volatility vs Option Price
- Stock Price vs Option Price
- Time to Expiry vs Option Price
- Option Payoff & Profit
- Delta
- Theta
- Rho
- Vega
- Gamma

---

## Monte Carlo Simulation

The project estimates option prices by simulating thousands of possible future stock prices under the risk-neutral measure and discounts the expected payoff back to the present. The results are compared with the analytical Black-Scholes solution.

---

## Technologies Used

- Python
- NumPy
- Pandas
- SciPy
- Matplotlib
- Jupyter Notebook

---

## Future Improvements

- Support for American options
- Binomial Tree pricing model
- Real-time market data integration
- Interactive dashboard using Streamlit
- Additional Greeks (Charms, Vanna, Vomma)
- Volatility surface visualizations

---

## Disclaimer

This project is intended for educational purposes and demonstrates option pricing concepts using the Black-Scholes framework. It is not intended for investment or trading decisions.











