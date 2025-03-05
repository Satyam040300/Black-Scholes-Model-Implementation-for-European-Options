# Black-Scholes Model Implementation for European Options

This project implements the **Black-Scholes Model** for pricing European **call** and **put options**. The Black-Scholes model is a mathematical model used for pricing options, and it is widely used in financial markets. This project calculates the price of options based on the current stock price, strike price, time to maturity, volatility, and the risk-free interest rate.

## Project Overview

The Black-Scholes model provides a theoretical estimate for the price of European-style options by using **log-normal distribution** assumptions and the **risk-neutral pricing theory**. The model incorporates the following key variables:
- **S₀**: Initial stock price
- **K**: Strike price
- **T**: Time to maturity (in years)
- **r**: Risk-free interest rate
- **σ**: Volatility (standard deviation of stock returns)

This project demonstrates how to calculate the **call** and **put** option prices using Python, and it also provides insight into the sensitivity of option prices to these inputs.

## Files

- `Satyam_Black_Scholes_Call_and_Put_Option_Pricing.ipynb`: Contains the implementation of the Black-Scholes model for **call** and **put** options.
- `requirements.txt`: Lists the required Python libraries (`scipy`, `math`).

## Usage

You can calculate the **call** and **put** option prices by calling the functions in the `Satyam_Black_Scholes_Call_and_Put_Option_Pricing.ipynb` file with the following parameters:


S0 = 100    # Initial stock price

K = 100     # Strike price

T = 1       # Time to maturity (in years)

r = 0.05    # Risk-free interest rate

sigma = 0.2 # Volatility (20%)

# Calculate the Call and Put prices
call_price = black_scholes_call(S0, K, T, r, sigma)

put_price = black_scholes_put(S0, K, T, r, sigma)


print(f"Call Option Price: {call_price}")

print(f"Put Option Price: {put_price}")

Call Option Price: 10.450583572185565

Put Option Price: 5.573526022256971

## Project Insights

This implementation provides a straightforward approach to calculating option prices and allows you to observe how option prices change with varying inputs.
The project demonstrates quantitative finance concepts such as risk-neutral pricing and volatility impact.
The model assumes European options, which can only be exercised at expiration.

## Skills Learned
Options Pricing using the Black-Scholes model

Python Programming for financial modeling

Quantitative Finance and Mathematical Finance

Probability & Statistics for financial data analysis

## Future Work
This project can be extended by:

Implementing the Greeks (Delta, Gamma, Vega, Theta, and Rho) to analyze option sensitivities.

Incorporating Monte Carlo simulations for option pricing to explore alternative methods.

Building a more interactive tool for real-time option pricing based on live stock data.



