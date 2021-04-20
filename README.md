# Option Price Prediction (machine learning)

For this project you will be examining European call option pricing data on the S&P 500. Recall, a European call option gives the holder the right (but not the obligation) to purchase an asset at a given time for a given price. Valuing such an option is tricky because it depends on the future value of the underlying asset.
The Black-Scholes option pricing formula provides an approach for valuing such options. Let K denote the strike price, i.e., the price one must pay to purchase the asset, and 𝜏 (tau) the time until expiration of the option. Suppose that the asset in question is currently trading at S, and has “volitility” (i.e., risk or standard deviation) of σ. Finally, suppose that the annual risk-free interest rate is r. 

The 1997 Nobel Prize in Economics was awarded for the Black-Scholes formula because it works remarkably well in practice. However, in this project we are going to attempt to build statistical/ML models to perform the same task. Often times such models are able to outperform Black-Scholes.
You will find two data sets on Blackboard: option_train.csv and option_test_wolabel.csv. The training data set has information on 1,680 separate options. In particular, for each option we have recorded
• Value (C): Current option value
• S: Current asset value
• K: Strike price of option
• r: Annual interest rate
• tau: Time to maturity (in years)
• BS: The Black-Scholes formula was applied to this data (using some 𝜎) to get C_pred.
and If an option has C_pred – C > 0, i.e., the prediction over estimated the option value, we associate that option by (Over); otherwise, we associate that option with (Under).
