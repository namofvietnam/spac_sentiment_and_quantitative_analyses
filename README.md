# Evaluating SPAC as An Asset Class Using Sentiment Analysis and Quantitative Analyses
This project evaluated the risk-return profile of SPACs (Special Purpose Acquisition Companies), after the hype on SPAC in 2021 had passed, and data on performances of SPAC and de-SPACed companies (those that went public through a SPAC scheme) had been more abundantly recorded. 

## Methodology
The project included the following techniques in Python:
- Scraping titles, abstracts, and contents of Wall Street Journal (WSJ) articles about SPAC using _Selenium_
- Sentiment analysis and visualizing the sentiment distribution of the articles
- Collecting data on performances of de-SPACed companies from Spactrack.io
- Visualizing the return distribution of de-SPACed companies using _diverging color histogram_
- Querying performances of S&P 500, SPCX (SPAC ETF), DSPC (de-SPACed ETF) with _yfinance_ package
- Plotting relative returns of SPY, SPCX, and DSPC to evaluate how a dollar would have performed if put in each of these asset classes

## File Run-down
The repository contains the following files:
### Data:
- final_WSJ_News.xlsx : scraped headlines, subheadings, body contents, timestamps of WSJ articles that mentioned SPAC
- DeSPACed.xlsx
- DeSPACed.csv
(Both contains the same data of companies that went public through SPAC. Data was collected from Spactrack.io)
### Jupyter Notebook files:
- Sentiment Analysis of SPAC Articles.ipynb
  - Filtering related articles
  - Sentiment analysis with TextBlob
  - Diverging color histogram of articles' sentiment distribution
- Quantitative Analyses of SPAC and deSPACed.ipynb 
  - Diverging color histogram to illustrate distribution of deSPACed companies' returns since inception
  - Collecting securities data with yfinance
  - Normalizing returns to one dollar
  - Plotting returns of SPY, SPCX, DSPC
  


