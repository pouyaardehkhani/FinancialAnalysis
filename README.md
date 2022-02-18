# FinancialAnalysis ![license](https://img.shields.io/github/license/pouyaardehkhani/FinancialAnalysis.svg) ![releases](https://img.shields.io/github/release/pouyaardehkhani/FinancialAnalysis.svg)
This notebook provides some skills to perform financial analysis on economical data.

**NOTE : Details are provided in the notebook**

# Skills that are covered in the notebook
1. **Plotting stock data by both matplotlib and plotly**
2. **Calculating stocks daily return**
3. **Finding correlation between daily returns**
4. **Portfolio Assets Allocation and Statistical Data Analysis**
    
    ## Portfolio Assets Allocation
    &emsp; For those who do not know what **Portfolio Assets Allocation** is:
    A portfolio is a collection of financial investments(assets) such as stocks, fixed income securities (bonds), cash, mutual funds and Exchange Traded Funds (ETFs).
    ### Types of assets(only 3 of them covered)
    #### 1. EQUITIES (STOCKS):
    &emsp; A stock simply represents an ownership of a certain percentage of a company. A stock gives the owner the right to some shares in a given company depending on how much stock (shares) they own. Stocks are traded on stock exchanges such as New York Stock Exchange (NYSE) and regular individuals can buy them via online brokerage firms. Stocks are generally liquid as compared to real estate which could take a much longer time to sell.
    #### 2. FIXED INCOME SECURITIES (BONDS):
     &emsp; Abond is a fixed income that are generally issued by governments or corporations and represents a loan made by an investor to the borrower. Bonds pay the investor a fixed stated interest rate. Bonds are used by companies and Governments to raise money to fund future projects. Bonds that are less risky such as U.S. Government Bonds pay less interest compared to high risk bonds. Bond coupons represent a semi-annual interest payments to the bond holder.
    #### 3. EXCHANGE TRADED FUNDS (ETFs):
    &emsp; ETFs are a type of security that includes a group of securities and possibly track an index such as the S&P500. ETFs are like mutual funds however they are marketable securities and are being traded on exchanges similar to any other stock. ETFs can include a collection of stocks, bonds, and commodities. ETFs have generally low management fees and offer a tool for risk diversification. Vanguard S&P 500 ETF (VOO): https://investor.vanguard.com/etf/profile/performance/voo
    ### Assets Allocation
    &emsp; Asset allocation is an investment strategy that is used to allocate client's assets based on their risk tolerance, target returns and investment time span. The goal of portfolio managers is to maximize returns and reduce risks.
    
    **common advice that financial advisors generally recommend to retired seniors when it comes to asset allocations**
    
    &emsp; The conventional wisdom is to subtract client's age from 100 to calculate the % of portolio that should be allocated to stocks 
    For Example: If you're 30 years old, you should have 70% allocated to stocks 
    If you are 75 years old, you should invest 25% in stocks (old retired seniors generally recommend a more stable low risk portfolio).
    
5. **PORTFOLIO STATISTICAL METRICS**
    #### Daily Returns
    &emsp; **Stock daily return is a calculation of how much investors have gained or lost per day.**
    
    &emsp; <img src="https://render.githubusercontent.com/render/math?math=Stock\,Daily\,Return = \frac{Closing\,Stock\,Price_t \,- \,Closing\,Stock \,Price_{t-1}}{Closing\,Stock\,Price_{t-1}}">
    
    #### Cummulative Return
    &emsp; **Cumulative return is a measure of the aggregate amount that the stock gained or lost over a period of time.**
    
    &emsp; <img src="https://render.githubusercontent.com/render/math?math=Stock\,Cummulative\,Return = \frac{Current\,Price\,Of\,Stock \,- \,Original Price\,Of\,Stock}{Original\,Price\,Of\,Stock}">
    
    #### Standard Deviation (Risk/Volatility)
    &emsp; **The standard deviation is a measurement of the dispersion away from the mean. The more spread the data is, the higher the standard deviation. Volatile stocks have high standard deviation and therefore standard deviation represent the risk associated with the security.**
    
    &emsp; <img src="https://render.githubusercontent.com/render/math?math=Standard\,Deviation = \sqrt{\frac{\sum_{i=1}^n \,(x_i\,-\,\bar{x})^2}{n - 1}}">
    
    &emsp; where: 

    &emsp; * x = Value of data with the index i 
    
    &emsp; * x = mean value 
    
    &emsp; * n = total number of data points in the data set
    
    #### Sharpe Ratio
    &emsp; **Sharpe ratio is used by investors to calculate the return of an investment compared to its risk.**
    
    &emsp; Sharpe ratio is calculated as follows:
    
    &emsp; <img src="https://render.githubusercontent.com/render/math?math=Sharpe\,Ratio = \frac{R_p \,- \,R_f}{\sigma_p}">
    
    &emsp; **Sharpe ratio is simply a calculation of the average return earned in excess of the risk free rate (U.S. government bonds) per unit of risk (volatility). Note that <img src="https://render.githubusercontent.com/render/math?math=R_f">, is the risk-free rate of return which is the return on an investment with zero risk, meaning it's the return investors could expect for taking no risk. As Sharpe ratio increases, risk-adjusted return increases and security becomes more desired by investors.**
    
6. **Portfolio Optimization using Monte Carlo Simulations**
7. **Plotting MARKOWITZ EFFICIENT FRONTIER**
8. **CAPITAL ASSET PRICING MODEL (CAPM)**
    ## CAPITAL ASSET PRICING MODEL (CAPM)
    For those who do not know what **CAPITAL ASSET PRICING MODEL (CAPM)** is:
    
    &emsp; **Capital Assets Pricing Model (CAPM) is one of the most important models in Finance. CAPM is a model that describes the relationship between the expected return and risk of securities. CAPM indicates that the expected return on a security is equal to the risk-free return plus a risk premium.**
    #### RISK FREE ASSET (<img src="https://render.githubusercontent.com/render/math?math=r_f">)
    &emsp; **CAPM assumes that there exist a risk free asset with zero standard deviation.
The risk free asset return is denoted as <img src="https://render.githubusercontent.com/render/math?math=r_f">.
Investors who are extremely risk averse would prefer to buy the risk free asset to protect their money and earn a low return <img src="https://render.githubusercontent.com/render/math?math=r_f">.
If investors are interested in gaining more return, they have to bear more risk compared to the risk free asset.**
A risk free asset could be a U.S. government 10 year Treasury bill. This is technically a risk free asset since it's backed by the US Government.
    #### MARKET PORTFOLIO (<img src="https://render.githubusercontent.com/render/math?math=r_m">)
    &emsp; **Market portfolio includes all securities in the market. A good representation of the market portfolio is the S&P500 (Standard & Poor's 500 Index).
The market overall return is denoted as <img src="https://render.githubusercontent.com/render/math?math=r_m">.
The S&P500 is a market-capitalization-weighted index of the 500 largest U.S. publicly traded companies.
The index is viewed as a gauge of large-cap U.S. equities.**
    #### WHAT IS BETA?
    &emsp; **Beta represents the slope of the line regression line(market return vs. stock return). Beta is a measure of the volatility or systematic risk of a security or portfolio compared to the entire market (S&P500). Beta is used in the CAPM and describes the relationship between systematic risk and expected return for assets. Tech stocks generally have higher betas than S&P500 but they also have excess returns.**
     * Beta=1.0: this indicates that its price activity is strongly correlated with the market.
     * Beta<1(defensive): indicates that the security is theoretically less volatile than the market (Ex:Utility and consumer goods (P&G). If the stock is included, this will make the portfolio less risky compared to the same portfolio without the stock.
     * Beta>1 (aggressive): indicates that the security's priceis more volatile than the market. For instance, Tesla stock beta is 1.26 indicating that it's 26% more volatile than the market. It will do better if the economy is booming and worse in cases of recession.
     #### CAPM FORMULA
     &emsp; <img src="https://render.githubusercontent.com/render/math?math=r_i = r_f \,+ \,B_i(r_m\,-\,r_f)">
     
     &emsp; Where:
     * <img src="https://render.githubusercontent.com/render/math?math=r_i"> EXPECTED RETURN OF A SECURITY
     * <img src="https://render.githubusercontent.com/render/math?math=r_f"> RISK FREE RATE OF RETURN
     * <img src="https://render.githubusercontent.com/render/math?math=B_i"> BETA BETWEEN THE STOCK AND THE MARKET
     * <img src="https://render.githubusercontent.com/render/math?math=(r_m\,-\,r_f)"> RISK PREMIUM (INCENTIVE FOR INVESTING IN A RISKY SECURITY)
     
9. **Trading Using Moving Average**
10. **create buy (1) and sell (-1) signal**
11. **Stock Price Predictions Using regression / LSTM**
12. **Bank Customers Segmentation**
13. **AUTOENCODERS (PERFORM DIMENSIONALITY REDUCTION USING AUTOENCODERS)**
14. **Stocks Sentiment Analysis Using AI**

     **We live in a world where we are constantly bombarded with social media feeds, tweets, and news articles. This huge data could be leveraged to predict people sentiment towards a particular company or stock. Natural language processing (NLP) works by converting words (text) into numbers. These numbers are then used to train an Al/ML model to make predictions. AI/ML-based sentiment analysis models, can be used to understand the sentiment from public tweets, which could be used as a factor while making a buy/sell decision of securities.**
     
15. **Text Data Cleaning(remove PUNCTUATIONS and STOPWORDS)**
16. **Plot WORDCLOUD**
17. **TOKENIZING AND PADDING**
    #### TOKENIZER
     **Tokenizer allows us to vectorize text corpus. Tokenization works by turning each text into a sequence of integers.**
18. **EMBEDDING LAYER**

     **Embedding layers learn low-dimensional continuous representation of discrete input variables.**
