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


# Call:

    ticker = 'AMD'
    start = "2023-01-01"
    end = "2025-01-01"
    df = yf.download(tickers= ticker,start=start, end=end)
    
    Output
        tmp/ipython-input-496447581.py:1: FutureWarning: YF.download() has changed argument auto_adjust default to True
        df = yf.download(tickers='AMD',start= "1980-01-01")
        [*********************100%***********************]  1 of 1 completed.



