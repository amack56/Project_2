# Agricultural Futures
![Image Credit:Dreamstime.com](images/agricultural_futures.jpeg)
    
## Determined Our Source Data & Environment
- [CME DataMine](https://www.cmegroup.com/market-data/datamine-historical-data.html#)
- [Nasdaq Data Link (Quandl)](https://data.nasdaq.com/)
- Looked at continuous contracts
- All have different expirations
- We built everything in Python Jupyer Lab

## Project Goals
- Predicted hog prices
    - Feed is 95% of the cost
    - Farmers need to determine quantity of corn to purchase
    - What are farmers margins?
   
## Loaded in and Cleaned the Data
    - HE - lean hogs
    - ZC - corn
    - ZM - soybean meal
    - LE - live cattle
    - GF - feeder cattle
- Joined the data into a single dataframe

## Data Preparation
- Created a correlation matrix
- Used the window_data function to generate the X and y values for the model
- Experimented with window sizes to see how the model performance changed
- Split the data into 70% training and 30% testing
- Applied the MinMaxScaler to the X and y values to scale the data between 0 and 1
- Reshaped the X_train and X_test data for the model

## Built and Trained the LSTM 
- Defined the model architecture and compiled the model
- Fit the model 
- Ran two different models to exemplify our process

## Hog Crush
- Created a new dataframe utilizing the 8-3-1 formula
    - 8 hog - 3 corn - 1 soymeal
- 


## Dashboard
- Showcased our visualizations

## Future Considerations / Additional Variables
- [Weather Data Api](https://www.aerisweather.com/features/aerisweather-api-amp/?gclid=Cj0KCQiAhMOMBhDhARIsAPVml-FcWnMwAw2Grk-DV8uZdGChvu9y8JuCGLRcTzi_motZ7Oa126vKDV4aAnGaEALw_wcB)
- [Oil Prices](https://www.oilpriceapi.com/)
- [Livestock Disease Analysis](https://www.aphis.usda.gov/aphis/ourfocus/animalhealth/animal-disease-information)
- [Land, Storage and Fertilizer](https://www.nrcs.usda.gov/Internet/FSE_DOCUMENTS/nrcs143_012131.pdf) 

## Technical Requirements
- Create our slideshow presentation in Google Slides
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

