# PricePredictor
Using Random Forest Models, PricePredictor isolates relevant trading signals to generate recommendations

### Team Members: Greg Buiter, Kai Ning Liu, Jimmy Tarika, Justin Gouin 
### Submission Due Date: June 19, 2021

Overview: 
Our model analyzes cryptocurrency data, specifically Bitcoin (BTC), and provides buy and sell recommendations; however, if one were to make asset-specific 
changes to the data intake structure, our model is generalizable for any asset.

To create our recommendations, we first generate trading signals from the following four distinct quantitative indicators: 50 and 200 day moving averages, 
bollinger bands, volume weighted average price (vwap), and relative strength index (rsi). 

We input these signals and the original, raw indicators into a Random Forest (RF) model to assess which of these variables are most significant in predicting 
an increase or a decrease in the price of BTC. Our model proved to be generally predictive, and so we selected the top 3 predictive signals (although in
future iterations we may do better to select only 2) for another RF model. This time, the RF model was used to generate specific buy and sell recommendations by 
regressing together these three signal variables. 

We then backtest the model, and visualize the recommendations and outcomes. 
