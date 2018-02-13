# Model-Bankruptcy-data-with-regularized-logistic-regression
## Objective
With the attributes from income statements and balance sheets, predict whether firms fail. Randomly take 60% of the data for training, and use the rest of the oberservations for testing the algorithm. First fit a logistic regression without regularization, second map attributes to a higher dimensional space and fit a regularized logistic regression.


## R scripts and data
1. `bankruptcy.csv`: the bankruptcy data set.
  - Size
    - Sales
  - Profit
    - ROCE: profit before tax=capital employed (%)
    - FFTL: funds flow (earnings before interest, tax & depreciation)=total liabilities
3) Gearing
a. GEAR: (current liabilities + long-term debt)=total assets
b. CLTA: current liabilities=total assets
4) Liquidity
a. CACL: current assets=current liabilities
b. QACL: (current assets – stock)=current liabilities
c. WCTA: (current assets – current liabilities)=total assets
5) LAG: number of days between account year end and the date the annual report and accounts were filed at company registry.
6) AGE: number of years the company has been operating since incorporation date.
7) CHAUD: coded 1 if changed auditor in previous three years, 0 otherwise
8) BIG6: coded 1 if company auditor is a Big6 auditor, 0 otherwise

2. `bankrupt.R`: the main R script.
