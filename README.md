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

    ticker = 'ETF5IT.JO'
    start = "2023-01-01"
    end = "2025-01-01"
    df = yf.download(tickers= ticker,start=start, end=end)
  
    Output
        /tmp/ipython-input-433252377.py:9: FutureWarning: YF.download() has changed argument auto_adjust default to True
          df = yf.download(tickers= ticker,start=start, end=end)
        [*********************100%***********************]  1 of 1 completed

# Returns

<img width="1024" height="316" alt="download (3)" src="https://github.com/user-attachments/assets/99c9e674-759c-41e3-a172-92cad2137a92" />

# Volatility

<img width="1187" height="290" alt="download (6)" src="https://github.com/user-attachments/assets/f040c4c2-679f-49d8-9617-babbbe8f7825" />

# Hypothesis Test on Returns
The Shapiro-Wilk test is a statistical test that checks if a sample of data comes from a normally distributed population








