


# Andrei Muravev

### - Houses Price prediction in Ames,Iowa
### - Regression Challenge



 ## Problem Statement:

   Ask a home buyer to describe their dream house, and they probably won't begin with the height of the basement, ceiling or the proximity to the railroad. But these factors could affect the price of homes dramatically. To establish correlations, we  need to do a deep reserch of trends and habbits how, where and why people buy certain home. In my opinion, results could be extremely valuable for real estate, construction companies, financial sector and for everyone who want to buy, rent or sell residential or business properties.

  In my project, I will use the well known 'Ames Housing Dataset' to create a regression model to predicts the price of houses in Ames, IA. And, find out what feauters (for example, size, location or conditions) are more likely would affect the price of homes.
  
  The 'Ames Housing Dataset' is an exceptionally detailed and robust dataset with over 70 columns and 2000 raws. And, to analyse and achieve my goal, I'm going to use different techniques such as correlation between price and other features, train-test split and cross-validation, refine my models over time and apply lasso and redge regalurarizations.


  Moreover, I will participate in  the 'Regression Challenge' competition on Kaggle to compare efficiency of my model with other participants.





 ##  Data sources:

* [`train.csv`](./datasets/train.csv): the training datasets with multiple features and salaprice
* [`test.csv`](./datasets/test.csv): the test test, doesn't include the salaprice





  
 ## Workflow:
 
 
 #### Import Datasets and packages
 
 
 #### Data cleaning
 
 - rename columns
 - clean corrupted and empty spots
 - drop unwanted raws
 - create list of collinear features
 - use get dummies to split columns for subcategories
 - convert numerical objects to integers
 
 
 #### Check Outliers
 
  - Check general skew
  - Apply outliers function
  - Apply plots
  - Analysis
 
 
 ####  Exploratory Data Analysis
 
  - Establish correlation between saleprice and other feautures
  - Identify outliers
  - Look at distributions
  - pairplot, histograms and graphs
 
 
 #### Dummies
 
  - Categorical features extraction
  - Split columns
  - Create correlations table / heatmap
  - Analyse new data and create a list of potential features
  
  
 #### Model Preparation
 
  - Establish target and features
  - Train/test split data
  - Instantiate Standard Scaler
 
 
 ####  Modeling
 
 - Fit linear regression
 - Fit lasso and ridge
 - Compare different scores and evaluate
 - refine the model, add or remove features
 
 
 
 
 
 
 ## Kaggle Predictions and Submission:
 
 - Use test set and run predictions on best model
 - Create a kuggle submission variable from ID and SalePrice
 - Save new csv and submit to Kaggle
 

 
 ##  Conclusion and Bussiness Recommendations:
 
#### Based on my research, the  following recommendations could be considered:

1. After exploring correlations between sale price, features and a heatmap, I could tell that although people are looking for the overall quality in houses and the price will definitely increase with increase in quality, some other factors will affect price as well. For example, the size of a garage in sq ft and in car capacity would on average increase the price of a home by 0.7.

2. Based on dummies analysis: the most expensive houses were sold in Northridge. It is in a top 6 by number of houses sold and has the highest average price. Also, Northridge has higher impact on my model predictions compare with others.

3. Looking at charts using the value counts and average prices, excellent quality kitchens are more attractive for people rather than fabulous. After trying to predict prices on my model, the excellent quality had higher impact than good. 

4. Homes with basement quality good were sold in 4 times more than homes with basement quality excellent. Both features increased my model accuracy. A good performer on my model was "basement finished area" with rating 1.

5. Majority of homes were sold: 
  - with 3 bedroom(1108), 2 bedrooms(544), 4 bedrooms(265)
  - with 2 baths  (1096), 1 bath    (900), others are less than 100   

6. To make a price prediction, I've used 3 different models:  Linear Regression, Lasso and Ridge. At the beginning, the score was almost the same and sometimes Linear Regression would win. But, as I added more and more features, Lasso's score started to rise. And, I will use Lasso to make future predictions and use this model for Kaggle competition.

 7. At the beginning of my modeling, only 6 best features were used choosen from pairplots and heatmap. My model fitted my data with %82 accuracy. And, my errors of predicted price would fluctuate in a range of 32800. After dummies split, I included 7 other dummy's features and a few numeric columns.  The accuracy of my model  increased to %88, and errors of  predicted price dropped to 26900. 

 
 8. In the future, more research could be done in exploring  infrastructure and areas where these homes were sold. For example, effect of schools, public transportation, hospitals, parks, distance from downtown and other features.

##### To summarize everything in one sentence, I'd recommend 3-bedroom houses with two baths in Northridge neighborhood with excellent kitchen quality, paying particular attention to special attributes such as garage and basement sq ft. 






