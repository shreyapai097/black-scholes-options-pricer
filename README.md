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
d_1=\frac{\ln{S/K} + (r + \frac{\sigma^2}{2})T}{\sigma\sqrt{T}}
\]

\[
d_2=d_1 - (\sigma\sqrt{T})
\]

Call Price:

\[
C=S\,N(d_1) - K\,e^{-rT}\,N(d_2)
\]

\[
P=K\,e^{-rT}\,N(-d_2) - S\,N(-d_1)
\]





