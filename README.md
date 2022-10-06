# Efficient Frontier Porfolio Model Card

## Basic Information
 - Personal developing model
 - License: MIT
 - Model date: October, 2022
 - Model implementation material: [Efficient Frontier Excel](https://github.com/Contona1215/Efficient-Frontier-Project/blob/main/EFFICIENT%20FRONTIER-%20Fangyuan_Du.xlsm)

## Intended Use
 - Primary intended uses: This model is an example portfolio in the proportion of stock and fund investment can be selected according to the client's preference and allocated reasonably using $100,000 funds.
 - Primary intended investment selected: APPLE, CVS HEALTH, MICROSOFT, ALPHABET, COSTCO WHOLESALE, AMAZON, STARBUCKS, NETFLIX, NIKE. 
 - Out-of-scope use cases: Any use beyond an educational example is out-of-scope.

## Test Data
 - **Source of test data**: Yahoo Finance
 - **Test data requirements**: At least ten years of monthly stock prices, selecting open price, high price, low price, close price, volume, and adj return.
 - **Number of rows in test data**: 500
 - **State any differences in columns between training and test data**: None

## Model details
 - **Columns used as inputs in the Excel model**: 'AAPL', 'CVS', 'MSFT', 'GOOGL', 'COST', 'AMZN', 'SBUX', 'NFLX', 'NKE'
 - **Type of model**: Efficient Frontier 
 - **Software used to implement the model**: Excel, scikit-learn
 - **Version of the modeling software**: Model version: 1.0(Excel version: 16.65, sklearn version: 1.0.2)

## Quantitative Analysis
- **Metrics used to evaluate the model**:
  - Time Series of Closing Prices
   
   
  
  - Time Series of Rate of Monthly Returns(in%)
  
  - Histograms of Monthly Rate of Returns(in%)
- **The final values of the metrics for all data**:

| **Porfolio** | **Standard Deviation** | **Mean** |
|--------------|:----------------- |:--------------------- |
| **AAPL.return**   | 9.71 | 3.15 | 
| **CVS.return**    | 6.58 | 0.86 | 
| **MSFT.return**   | 6.51 | 1.34 | 
| **GOOGL.return**  | 8.76 | 2.17 | 
| **COST.return**   | 5.31 | 1.25 | 
| **AMZN.return**   | 10.52| 2.77 | 
| **SBUX.return**   | 7.77 | 1.48 | 
| **NFLX.return**   | 15.39| 3.89 | 
| **NKE.return**    | 6.32 | 1.50 |




