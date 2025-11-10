# 1. Exploratory analysis

# Closing Prices.
<img width="996" height="316" alt="download (8)" src="https://github.com/user-attachments/assets/f8caaba9-d92b-455d-a58c-44bfc6e2007e" />

# Returns.

<img width="1024" height="316" alt="download (3)" src="https://github.com/user-attachments/assets/99c9e674-759c-41e3-a172-92cad2137a92" />

# Volatility.

<img width="1187" height="290" alt="download (6)" src="https://github.com/user-attachments/assets/f040c4c2-679f-49d8-9617-babbbe8f7825" />

# Geometric Brownian Motion

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

Depending upon the number of simulated paths, the converge estimation to the actual price.


# Estamating old Price

<img width="997" height="316" alt="download (7)" src="https://github.com/user-attachments/assets/41bd253f-df90-414d-9eef-e917fcad88cb" />

<img width="996" height="316" alt="image" src="https://github.com/user-attachments/assets/7c9fcab5-fb20-412d-9180-0c1191e3f4c2" />

Taking an average of the thousand sample paths, we observe an average percentage error of -3.397625 with a scaled volatility factor of 2.5, suggest that the model on average over-estimates the price: 

# Estimating New Price
<img width="1005" height="316" alt="image" src="https://github.com/user-attachments/assets/51fb6ed7-f97e-460e-8ce4-cab9f190aae7" />
Taking another sample path over the next 5 years, where each step is an averaged approximation and assuming constant volatility.





