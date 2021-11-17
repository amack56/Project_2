# Agricultural Futures
![Image Credit:Dreamstime.com](images/agricultural_futures.jpeg)
    
## Determined Our Source Data & Environment
- [CME DataMine](https://www.cmegroup.com/market-data/datamine-historical-data.html#)
- Built the project in Jupyter Lab
- [Google Slides presentation](https://docs.google.com/presentation/d/1IZplJYO0P4w_COjAJ48CUtNfo1ynZ99CkwT8p8GHzmg/edit#slide=id.p)

## Project Goals
- Predict hog prices
    - Feed is 95% of the cost
    - Farmers need to determine quantity of corn to purchase
    - What are farmers margins?
    - What is GFM?
    - How does all this correlate?
- Predict and create a profitable algo for trading the hog crush
    - Assess and visualize results

## Loaded In and Cleaned the Data
- HE - lean hogs
- ZC - corn
- ZM - soybean meal
- LE - live cattle
- GF - feeder cattle
- Joined the data into a single dataframe

## Understanding Gross Feeding Margin (GFM)
- The difference between the purchased inputs value and the sold finished hog value is known as the gross feeding margin (GFM).
- GFM t= 2.05 * LH t - WP t-5-(10 * C t-5)-(0.a * SM t-5)
- LH t: Lean Hog at placement,  WP t-5: Weaned Hog 5 months from placement, C t-5: Corn 5 months from placement, SM t-5: Soybean meal 5 months from placement.
- Corn and soybean meal correlate positively with the price of actual hog.

## Data Preparation
- Created a correlation matrix
- Used the window_data function to generate the X and y values for the model
- Experimented with window sizes to see how the model performance changed
- Split the data into 70% training and 30% testing
- Applied the MinMaxScaler to the X and y values to scale the data between 0 and 1
- Reshaped the X_train and X_test data for the model

## Assess the Value of the Hog Crush
- Traders subtract the combined values of the corn and soymeal inputs from the value of the lean hogs.
- Hogs are priced per hundred pounds in eight futures contracts (40,000 lbs per contract) 
- Corn is priced per bushel in three contracts (5,000 bushels per contract)
- Soymeal is priced for short ton in a single contract (100 short tons per contract)
- Creating a 8-3-1 Hog Crush 
- Expressed as a positive value of price per cwt. (hundredweight) of lean hogs

## Trading Algo on Hog Crush
- Visualized correlations
- Confirmed the hog crush ratio through historical OLS
- Due to mean-reverting nature of spread, created z-score based algo
- Used feature engineering to enhance model using a z-score over MACD (Chose 5 and 60)
- Plot the equity curve and analyze the performance on a risk adjusted basis

## Built and Trained the LSTM RNN Model
- Defined the model architecture
- Compiled the model
- Fit the model 
- Ran two different models to exemplify our process

## Dashboard

![Single LSTM](./images/single_lstm.png)

![LSTM Heat Map](./images/Heat_map_multivariable.png)

![Multivariable LSTM](./images/multii_lstm.png)

![Hog Crush](./images/Lean_Hog_Crush.png)

![Standard Scaler](./images/Standard_Scaler.png)

![Hog Crush Heat Map](./images/Heat_Map_Hog_Crush.png)

![Mean Line](./images/Mean_Line.png)

![Z-Scores](./images/Z-scores.png)

![Featured Engineering](./images/Feature_Engineering.png)

![Rolling Ratio Z-Score](./images/Rolling_Ratio_Z_Score.png)

![Feature Train Z Score](./images/Feature_Train_Z_Score.png)

![Buy Sell Signal](./images/Buy_Sell_Hog_Corn_Soybean.png)

![Equity Curve](./images/Equity_Curve.png)

## Conclusions & Predictions
- We need to add more data to the model to train.
- We would need more time or an extremely powerful machine for us to play around with an LSTM model and move inputs and variables around.
- Consider risk-adjusted metrics to better ascertain algo robustness
- Optimize MA variables and z-score entry levels
- Calculate and implement cost of trading (commissions, slippage, etc.)
- Assess seasonality and remove outlier data like (PED in 2014, COVID, etc.)

## Future Considerations
- [Add Weather Data Api](https://www.aerisweather.com/features/aerisweather-api-amp/?gclid=Cj0KCQiAhMOMBhDhARIsAPVml-FcWnMwAw2Grk-DV8uZdGChvu9y8JuCGLRcTzi_motZ7Oa126vKDV4aAnGaEALw_wcB)
- [Add Oil Prices Api](https://www.oilpriceapi.com/)
- [Perform Livestock Disease Analysis](https://www.aphis.usda.gov/aphis/ourfocus/animalhealth/animal-disease-information)
- [Factor In Land, Storage and Fertilizer Costs](https://www.nrcs.usda.gov/Internet/FSE_DOCUMENTS/nrcs143_012131.pdf)

## Technical Requirements
- Created our slideshow presentation in Google Slides
- Summarized our conclusions and predictions
- Optional, apply a dimensionality reduction technique to reduce the input features, or perform feature engineering to generate new features to train the model
- Created two machine learning models.
- Fit the models to the training data.
- Evaluated the trained models using testing data. Include any calculations, metrics, or visualizations needed to evaluate the performance
- Showed the trained models using testing data. Include any calculations, metrics, or visualizations needed to evaluate the performance
- Saved PNG images of your visualizations to distribute to the class and instructional team for inclusion in our presentation and our repo's README.md
- Used one new machine learning library, machine learning model, or evaluation metric that hasn't been covered in class
- Created a README.md in your repo with a write-up summarizing your project

### Resources:
- [CME DataMine](https://www.cmegroup.com/market-data/datamine-historical-data.html#)
- [Nasdaq Data Link (Quandl)](https://data.nasdaq.com/)
- [USDA - National Agricultural Statistics Services](https://www.nass.usda.gov/)
- [USDA Economic Research Service](https://www.ers.usda.gov/publications/?page=1&topicId=0&authorId=0&seriesCode=LDPM&sort=CopyrightDate&sortDir=desc)
- [CME Institute](https://www.cmegroup.com/education.html?utm_source=pardot&utm_medium=email&utm_campaign=student_nurture&utm_content=20200930_graduated#)
- [Hog Feeding Spreads](https://www.cmegroup.com/trading/agricultural/files/AC-379_HogFeedingWhitePaper_r2.pdf)
- [Trading Opportunities in Lean Hogs](https://www.cmegroup.com/education/whitepapers/trading-opportunities-in-lean-hogs.html)
- [Niche Pork Production](https://www.ipic.iastate.edu/publications/840.feedbudgets.pdf)
- [Soybean Crush Synthetic Futures](https://www.cmegroup.com/markets/agriculture/oilseeds/soybean-crush.contractSpecs.html)
- [Tri-State Livestock News](https://www.tsln.com/news/cattle-futures-101-fundamentals-of-industry-marketing-tool-explained/#:~:text=There%20are%20two%20types%20of,the%20point%20of%20harvest%20weight)
- [Nasdaq Continuous Futures](https://data.nasdaq.com/databases/SCF/documentation)
- [RJO Futures - Lean Hog Futures](https://rjofutures.rjobrien.com/futures-markets/agriculturals/lean-hog-futures)
- [Pairs Trading With Python](https://github.com/KidQuant/Pairs-Trading-With-Python/blob/master/PairsTrading.ipynb)
- [Machine Learning Mastery](https://machinelearningmastery.com/machine-learning-in-python-step-by-step/)
- [How Cost of Carry Works](https://www.investopedia.com/terms/c/costofcarry.asp)
- [Supplementary Notebooks](https://nu.bootcampcontent.com/NU-Coding-Bootcamp/nu-chi-fin-pt-07-2021-u-c/-/tree/master/05-Student-Resources/Supplementary_Notebooks)
- [Hundred Weight (CWT)](https://www.investopedia.com/terms/h/hundredweight.asp)
- [Understanding the Hog Crush Margin](https://www.iowapork.org/wp-content/uploads/2015/06/Hog-Crush-Margin-IPPA-John-Lawrence.pdf)
- [Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/04.01-simple-line-plots.html)
- [Towards Data Science](https://towardsdatascience.com/how-to-build-your-first-machine-learning-model-in-python-e70fd1907cdd)
- [Investopedia: Cost of Carry](https://www.investopedia.com/terms/c/costofcarry.asp)
- [An Introduction to Hog Feeding Spreads](https://www.cmegroup.com/trading/agricultural/files/AC-379_HogFeedingWhitePaper_r2.pdf)
- [Iowa State University - Animal Industry Report](https://lib.dr.iastate.edu/cgi/viewcontent.cgi?article=2334&context=ans_air)
- [Nasdaq - Continuous Futures](https://data.nasdaq.com/databases/SCF/pricing/plans)

