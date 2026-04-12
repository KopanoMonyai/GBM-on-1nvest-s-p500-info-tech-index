# Geometric Brownian Motion

The Geometric Brownian Motion (GBM) is a continuous-time stochastic process in which the logarithm of the randomly varying quantity follows a Brownian motion (also called a Wiener process) with drift. This method is used to model stock prices in the Black–Scholes model and is the most widely used model of stock price behavior.

The Geometric Brownian Motion equation is represented as:

$\large{S_t = S_0 \ e^{\big(\mu - \frac{\sigma^2}{2}\big) t + \sigma W_t}}$

where:

$S_0$ is the initial value

$\mu$ is a drift coefficient

$\sigma$ is the volatility

$W_t$ is a (standard) Brownian motion.


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

Depending upon the number of simulated paths, the estimation converges to the actual price.

<img width="997" height="316" alt="download (7)" src="https://github.com/user-attachments/assets/41bd253f-df90-414d-9eef-e917fcad88cb" />


# Price Prediction
Taking an average of the thousand sample paths, we observe an average percentage error of 0.00610164 with a scaled volatility factor of 2.5, suggest that the model on average under-estimates the price: 

<img width="996" height="316" alt="download (7)" src="https://github.com/user-attachments/assets/dc82e81a-93fc-4f3e-aad2-39120225c058" />

  
                                        Close	Estimate	Abs Error
        2020-11-12 00:00:00+02:00	11.808510	11.80851	0.000000
        2021-11-12 00:00:00+02:00	16.026600	14.31000	0.107109
        2022-11-12 00:00:00+02:00	14.334960	17.08000	0.191493
        2023-11-12 00:00:00+02:00	21.463999	22.04000	0.026836
        2024-11-12 00:00:00+02:00	30.010000	27.04000	0.098967
        2025-11-12 00:00:00+02:00	36.020000	34.26000	0.048862


# Estimating Of New Prices
Taking another sample path over the next 5 years, where each step is an averaged approximation while assuming constant volatility.

    
                0	Error
    Year		
    2025	36.75	0.006102
    2026	46.20	0.006102
    2027	57.93	0.006102
    2028	72.61	0.006102




