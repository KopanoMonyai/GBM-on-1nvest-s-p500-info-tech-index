# 1. Exploratory analysis

# 1.1) Visualising Closing Prices.
<img width="996" height="316" alt="download (8)" src="https://github.com/user-attachments/assets/f8caaba9-d92b-455d-a58c-44bfc6e2007e" />

# 1.2) Returns.

<img width="1024" height="316" alt="download (3)" src="https://github.com/user-attachments/assets/99c9e674-759c-41e3-a172-92cad2137a92" />

# 1.3) Volatility.

<img width="1187" height="290" alt="download (6)" src="https://github.com/user-attachments/assets/f040c4c2-679f-49d8-9617-babbbe8f7825" />

# 2) Geometric Brownian Motion

The Geometric Brownian Motion (GBM) is a continuous-time stochastic process in which the logarithm of the randomly varying quantity follows a Brownian motion (also called a Wiener process) with drift. This method is used to model stock prices in the Black–Scholes model and is the most widely used model of stock price behavior.

The Geometric Brownian Motion equation is represented as:

<img width="710" height="77" alt="image" src="https://github.com/user-attachments/assets/3fd1383f-429a-4140-8850-6a01e65ccc75" />

Where:

S(t) is the price of a security/portfolio at time t

σ is the volatility of the security’s price

µ is mean return (per unit time)

dS(t) infinitesimal increment in price

dW(t) infinitesimal increment of a standard Brownian Motion/Wiener Process


# Positional Arguments

    ticker = Ticker symbol for the stock
    start = The beginning time period
    end = The end time period
    S0 = Initial stock price
    mu = Expected return (drift)
    sigma = Volatility
    T = Time horizon (years)
    N = Number of time steps (e.g., trading days in a year)
    num_simulations = Number of simulated paths


# Call:

    simulate_gbm(S0, mu, sigma, T, N, num_simulations)
    <img width="997" height="316" alt="download (9)" src="https://github.com/user-attachments/assets/ccad58c6-0006-4411-b872-d71cb44c5c1c" />

Depending upon the number of simulated paths the more accurate the solution


# 1.Estamating New Price
Taking a thousand sample paths with a percentage error of 26.94038245219348
<img width="997" height="316" alt="download (7)" src="https://github.com/user-attachments/assets/41bd253f-df90-414d-9eef-e917fcad88cb" />
taking the average of those sample paths
<img width="996" height="316" alt="image" src="https://github.com/user-attachments/assets/7ed86da4-0c9b-4aee-8809-aadc386de4fe" />






