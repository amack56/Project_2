# Agricultural Futures
![Image Credit:Dreamstime.com](images/agricultural_futures.jpeg)
    
## Determined Our Source Data & Environment
- [CME DataMine](https://www.cmegroup.com/market-data/datamine-historical-data.html#)
- [Nasdaq Data Link (Quandl)](https://data.nasdaq.com/)
- Looked at continuous contracts
- All have different expirations
    
## Loaded In and Cleaned Data
- HE - lean hogs
- ZC - corn
- ZM - soybean meal
- LE - live cattle
- GF - feeder cattle

## Project Goals
- Predicted hog prices
    - Feed is 95% of the cost
    - There is also land, storage and fertilizer costs
    - Farmers need to determine quantity of corn to purchase
    - What are farmers margins?
    - Livestock disease & outlier analysis
- Created a Correlation Matrix
- Assessed the Value of the Hog Crush
- Created a Dashboard
- Sharpe and Sortino Ratios

## Usage Instructions
- Split data into train and test
- Used the MinMaxScaler to scale data between 0 and 1
- Reshaped the features for the model

## Future Considerations
- Add Weather Data as Variable
- Add Oil Prices as Another Variable

## Technical Requirements
- Create our slideshow presentation
    - PowerPoint, Keynote or Google Slides
- Summarize our conclusions and predictions
- Optional, apply a dimensionality reduction technique to reduce the input features, or perform feature engineering to generate new features to train the model
- Create one or more machine learning models.
- Fit the model(s) to the training data.
- Evaluate the trained model(s) using testing data. Include any calculations, metrics, or visualizations needed to evaluate the performance
- Show the predictions using a sample of new data. Compare the predictions if more than one model is used.
- Save PNG images of your visualizations to distribute to the class and instructional team for inclusion in our presentation and our repo's README.md
- Use one new machine learning library, machine learning model, or evaluation metric that hasn't been covered in class
- Create a README.md in your repo with a write-up summarizing your project. Be sure to include any usage instructions to set up and use the model

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

