# Project1_Fintech_SydUni
## Team: MGM - Mike Rae, Grace Ho, Michael Yip

# OLD LADY BUFFET

REQUIRED (DELETE ONCE DONE): "Create a README.md in your repo with a write-up summarizing your major findings. 
This should include a heading for each question you asked of your data and under each heading a short description of what you found and any relevant plots.

# Core hypothesis
## That Warren Buffet's suggested ETFs were not the best choice for Mrs Buffet's eventual inheritance.
### In 2013, Warren Buffett stated that he advised trustees to manage the money he will leave to his wife by allocating
### 10% in short-term government bonds and 90% in a very low-cost S&P 500 index fund (suggesting Vanguard’s.)
### Warren said he believed the long-term results from this policy will be superior to those attained by most investors.
### We want to test Warren's suggestion against other options and criteria to determine if it is the best recommendation for Mrs Buffet.

# Key Questions to answer:
## What are the appropriate asset classes for Mrs Buffet's inheritance?
We considered asset classes including: direct shares / bonds / FX holdings, cryptocurrencies, real estate, collectables.  
But these were discounted based on our subjective criteria, and we concluded ETFs are an appropriate asset class for Mrs Buffet due to her knowledge and life stage.

## How do we select the specific assets within the appropriate asset(s) class?
Within the ETF universe, we used a funnel to output the top ETFs over different timeframes.

## What other factors do we need to consider for our final recommendation to Mrs Buffet?  
We also considered ESC (Environmental, Social, and (Corporate) Governance) ratings, risk & volatilty vs return, and time horizon based on Mrs Buffet's age.

## Analysis also factoring in:
### What is the global distribution of ETFs?
### What are the top 9 performing ETF's?
### What was the daily returns distribution?
### How did the cumulative returns compare?
### What correlations are in the top 2 ETF's?
### How risky are the tops ETF's?
### How did the Sharpe Ratio's look?
### What companies are most green? *note partial data

# Data Sources used:
 - ETFdb.com for listings of ETFs from around the world which are traded in the USA.
 - yFinance for daily ETF close prices over the past decade.
 - RapidAPI for ESG data points

# Data exploration & clean up process:
Daily close price data for 561 ETFs over a decade was obtained.  They had to be broken up into 30 smaller data requests and pulled into Jupyter Lab.
The cumulative returns were reviewed based on 4 time horizons: 1, 3, 5 and 10 year returns.  The top 20 ETFs for each of these time horizons were extracted, resulting in 51 ETFs.
The top 20 ETFs from each timeframe were given a score based on their rank, and an overall ranking obtained over the 4 time horizons.
From this process, a list of top 9 ETFs across all timeframes were selected.
The data was then amended so the top 9 ETFs were reviewed using a consistent start date (7.5 years history), so they could be consistently compared based on cumulative returns, standard deviation, sharpe ratio.

# Conclusions. This should include a numerical summary (i.e., what data did your analysis yield), as well as visualizations of that summary (plots of the final analysis data).
1. SOXL and TQQQ had the best returns however are 3x leveraged so high risk...
2. The Vanguard fund VSBSX has the highest Sharpe Ratio and lowest standard deviation (and overall risk) although very low returns...
3. MGM Consulting’s recommendation for Mrs Buffett would be the 3rd and 4th ranked ETF’s (SMH and ARKK) with good average returns and a good std dev and Sharpe Ratio.

STILL NEED TO DO
Include images/ dashboard and 

 Discuss the implications of your findings. This is where you get to have an open-ended discussion about what your findings mean.


 Tell a good story! Storytelling through data analysis is no different than in literature. Find your narrative and use your analysis and visualization skills to highlight conflict and resolution in your data.
