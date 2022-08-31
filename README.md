## Report

> This project is about how you can create your portfolio on Python based on stock returns of over companies. Inputs that I used from yahoofinance to get companies 
> real stock prices. My portflio consisted of 4 real company stocks: 
- General Electronics
- JPMorgan Chase &amp; Co.
- Microsoft Corporation
- Citigroup Inc.
 
> The tool shows returns and risks by finding variance of returns. Returns from portfolio according
> to companies were equal weights, each of them 25%. Moreover my idea was, to show the stock price
> change visually by using python plotting function. Project informs user about portfolio profitability and
> riskiness over any time period by writing start and end data. For financial approach, to find risk of
> portfolio I found daily mean and then annual mean. Using data which I imported, I found portfolio
> simple returns, co-variance, daily returns, variance(risk), and correlation among stocks. Standard
> deviation and volatility of population, volatility actually shows our risk. This project strictly will helpful
> investments.

Now I am going to explain what I have done.

1. First, we need to import our library used within this project:
- Datetime-to get a date
- pandas_datareader-to get stock prices
- pandas-for analyses
- NumPy-for high-level mathematical functions, 
- matplotlib.pyplot-graphing from pandas.plotting import register_matplotlib_converters,
- register_matplotlib_converters()-for register –for errors, 
- fivethirtyeight.com - site I use graphs styles as the same.

2. Get stock symbols and my stocks for portfolio: 
- GE-General Electronics, 
- JPM-JPMorgan Chase &amp; Co.,
- MSFT-Microsoft Corporation, 
- C-Citigroup Inc. and print them

3. To get a start date and end date for the portfolio. I begin from the 1st of January to see full-year data.
The end date is the current date as a form of YYYY-MM-DD.

4. To calculate the number of stocks in the portfolio and print it.

5. To create a function for import stock adjusted prices from 01.01.2015 until now as data and print it.
6. To create a function to see visually price change as a graph.

7. To find simple daily returns by using the percentage change function for the data.
8. To find a correlation (Correlation is a mathematical term used to find a change in one variable leads to change in another variable and changes between -1 and 1. 1 is positive corr , if one variable increases another variable increase. Negative corr (-1) - one increases - another decrease.) and print it
9. Find the covariance matrix for daily simple returns which means how stocks move together and print it.
10. In this step, I calculated variance or other words risk. (Variance is used in finance to find risk. It used to find spread between prices. If Variance is high it means high risk, higher return, and higher volatility and if a variance is low then low risk, lower return, and lower volatility.)
11. To find a standard deviation or square-root of the variance is called volatility. In our case, less risky asset in our data is Microsoft (0.017317) and higher risk asset is General Electronics(0.021942) (as explained 10.)
12. To create a graph for daily simple returns and volatility.
13. And this step I found expected returns by finding the mean of daily simple returns. As we see again higher performance for expected returns showed by Microsoft (0.001213) and the lowest by General Electronics (-0.000630).
14. By using expected returns according to weights of companies( each of the 25%) I found daily expected portfolio return (0.00030603649528441643)
15. To find annual return we need to multiply daily returns to annual trading days(253) which is in our portfolio annual return is 0.07742723330695736. It means our investment gives about 7.74% annual return.
16. Create a function to find cumulative returns by numpy.cumprod() function and print it
17.To create a graph for cumulative daily simple returns Result

> As we see from the cumulative returns bar chart&#39;s highest performance made by Microsoft over our portfolio. If we invested Microsoft on 01.01.2015 and sold it in > 2020 we could make gain in our investment. On the other hand, the lowest performance made by General Electronics.
