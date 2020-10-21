# Project 1
Phil Abraham

Felipe Ayala

Eve Griggs

Eren Turkmenonglu

## BlackRock Investments Presents:
# Beating the SP500, A Million Dollar Selection Process

BlackRock Investments is comprised of learners and stock market enthusiasts. In this project we worked to create a simple yet sophisticated portfolio that could potentially beat the overall stock market.
We selected large-cap to mega-cap stocks in order to follow a low market correlation to a high beta strategy.
We built our portfolio with a systematic stock selection approach and forecasted future returns by running a Monte Carlo Simulation as well as comparing the performance of our portfolio and the benchmark based on 5 years of historical data.

# Key components for selecting a Portfolio which will outperform the SP500
To create our portfolio which will be compared against the S&P500, each team member has selected some stocks, 28 stocks in total. Then we evaluated them based on their beta and market correlation to keep the most suitable stocks with our portfolio strategy. We kept the stocks yielding the highest outcome of the division of stocks' beta to their market correlation in order to achieve high-beta & low-market correlation stocks.

## Is it possible to outperform the SP500?
Based on our 5 years of historical data, the stocks that our team picked outperformed the S&P 500.
We looked at the following comparisons to determine our portfolio performance against the SPY;


>>SPY historical vs BLK historical Portfolio

>>SPY Sharpe vs BLK Portfolio Sharpe

>>SPY 5YR MC Sim vs BLK Portfolio  5YR MC Sim

## What does the selection process look like to create the portfolio?
Stock Picking Strategies:

Eve: Technology sector reflecting consumer and industry trends. 

Felipe: Large Cap Stocks / consistent history of dividend yield and growth.

Phil: Large Cap and Mega Cap / Financial Services, Consumer Defensive, Tech, Consumer Cyclical. P/E, Beta, Working Capital and EV/EBITDA

Eren: Enterprise Software, Technology, Entertainment, Pharmaceutical. Comparison analysis with peers using fundamental analysis, stocks that are operating in more than a single industry.

### BLK Final Portfolio Composition:

### Select final Stock portfolio by using a High Beta low Correlation Strategy

### Final Portfolio Composition: 40% SPY and 60% BLK Portfolio. 

## How do our applied metrics determine if the portfolio beats the SP500?
Our goal was to compare historical metrics and run a Monte Carlo Simulation to determine the probability of outperforming the stock market. Below are the selected metrics:

>> 5 yr - Historical Returns

>> Sharpe Ratios

>> 5 yr - MC Simulation: 

# Understanding the Data: An elaboration on our applied metrics

## Initial portfolio resulted in 28 stocks selected based on team members' decisions. The selected Portfolio (BLK) is reduced from 28 to 15 stocks by running the following data exploration

We calculated the daily return of stocks based on 5 years of historical data (approx 11-2015:11-2020) in order to find their betas and market correlation. 

We used ffn library (https://pypi.org/project/ffn/) to plot histograms of daily returns;
![raw portfolio returns](./Images/Daily_Returns_of_each_individual_Stock.png)


![histograms raw portfolio x sp500](./Images/histogramshistorical.png)

Calculating the covariance and variance for the Initial Portfolio and SP500: 

![covariance image](./Images/covariance.png)

![covariance code](./Images/covarianceCode.png)

Calculating beta of raw portfolio stocks, sorting from lowest to highest in order to pick high beta stocks;
![beta](./Images/beta.png)

Calculating correlation of raw portfolio to S&P500;
### correlation_of_portfolio = daily_returns.corr()

### correlation_of_portfolio

![correlation](./Images/fnnBetaRaw.png)

![correlation table](./Images/correlationtable.png)


# Final portfolio selection: Low correlation to SP500 and High Beta metric from initial portfolio
Using the lowest market correlation and highest beta from our initial 28 stock portfolio, we selected 15 stocks. However, as an executive decision, we replaced 2 stocks. We removed PSX and SBUX, and added PFE and COST form our raw portfolio. We wanted to capitalize on Costco’s future growth and reduce all exposure to the Oil Industry Sector.
Finally, we picked the 15 stocks below;
AMT, ORCL, PPG, COST, MSFT, UNH, TROW, BLK, NVDA, FB, BABA, CRM, PFE, NFLX, SQ. 
These stocks constituted the 60% of our final portfolio by allocating 4% to each stock.
And the 40% left was invested in S&P 500. 
![portfolio selection](./Images/portfolioselection.png)

![portfolio strategy](./Images/portfoliostrategy.png)

### Final BLK Portfolio composition = (40% SPY + 60% BLK Portfolio) Totaling 16 holdings. 

# Data Results and Findings

## 5 Year MC Simulation Expected Return BLK Port vs SPY

![MC sim SP500](./CSVs/MonteCarlo_5yrs_SPY_simulation.png)

![MC sim ](./Images/MCsimulationBLK.png)

There is a 95% chance that an initial investment of $10,000 in BKL strategy, will end within the range of $ 19,024.21  and $ 42,326.91. This represents 90.24% to 323.26% return in a 5 year period. 
There is a 95% chance Expected Return of a $10,000 initial portfolio investing in SPY will end within the range of $ 7,019.96  and $ 38255.93. This represents -29.81% to 282.55% return in a 5 year period. 
Based on the results of MC simulation, our portfolio is on average more likely to perform better than the S&P 500 for the next 5 years. 
## Sharpe Ratio

![sharpe ratio](./Images/sharperatioBLK_SP500.png)

>>The sharpe ratio comparisons are favorable for the BLK portfolio, based upon a good ratio above 1, and the SP500 ratio below 1 as sub-optimal.

# The goal of our project was to answer the question: Can we beat the market?
*We used data from open sources as well as API’s to collect the data*. 

*Techniques and applied data manipulation to include Juypter notebooks, pandas and Python to clean and interpret the data and we used FFN to help understand the data*.

*Through analysis and interpretation we determined a portfolio that we felt best offered us a chance to outperform the S&P500* .

 ***Based on historical data and future predictions we determined that it is possible to use the portfolio we created to outperform the market***.{*DISCLAIMER}



* DISCLAIMER: This portfolio was created for the purposes of this project and should not be the sole method of determining stock selections nor should it be viewed as  strong investment method. This portfolio while containing financial analysis worked primarily to highlight the teams coding abilities and not necessarily their ability to pick stocks or guarantee any type of return. The team takes no responsibility or liability if an individual attempts to use this portfolio in order to replicate returns. The team also makes no guarantee that the returns predicted can come true. The team as a collective is not an investment advisor or serve in a advising capacity and should not be viewed as such.
Please speak to a registered Investment professional before making any financial decisions
The team has no affiliation with BlackRock Investment Management Company nor do we represent their views. The team name was predetermined and the team used it solely in a identifying capacity.
Past results DO NOT guarantee future returns.

