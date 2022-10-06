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
   
   ![Closing Price] <img src="Closing Price.png" width="100" height="100" />
      - Closing prices help analyze the level of sales and also can help investors decide whether to invest. Although the closing price fluctuates, the      overall trend of the closing price curves is upward. The closing prices are the fundamental data to choose the stock. If the closing price continues to fall, it means that the stock continues to lose money. Therefore, these stocks are a good choice for the portfolio on the macroscopic.
  
  - Time Series of Rate of Monthly Returns(in%)
  
  ![Monthly Return](https://user-images.githubusercontent.com/111463982/194404320-c913b6f8-a481-4fba-9a1a-c2d82bdbece4.png)
     - Based on the rate of monthly returns, as Y-axis as centered, positive volatility means profit and negative volatility means loss.  From the estimated yearly return, all stocks are positive, and investors are able to get profits in the long term.  Intuitively, nine stocks have different situations of positive and negative return peaks. Specifically, Netflix- 43.0%, the highest yearly return in the stock portfolio-owns the highest yearly return and also owns the lowest negative peak, which means high returns come with high risks.  For technological companies, Apple, Microsoft, Alphabet, and Amazon have great monthly return fluctuation and yearly return, and these stocks generally are optimistic in the future to continue to go higher.  During COVID-19, Brick-and-mortar companies, including CVS Health, Costco, Starbucks, and Nike, will be affected more than tech companies, which is reciprocal in the stocks’ performance.
  
  - Histograms of Monthly Rate of Returns(in%)
  
  ![Density Monthly Return](https://user-images.githubusercontent.com/111463982/194404343-5eb00d53-65fc-44a1-b1f4-61d9a00698f4.png)

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




