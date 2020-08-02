# Housing Market

**Goal:** Analyse a housing market data set and create a regression model to predict housing prices.

**Data Source:** https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data

**Packages:** pandas, numpy, seaborn, matplotlib, scikit-learn


## Data Cleaning: 

Replacing certain missing values with 0 (ex. since no garage = no cars in garage)

Replaced other missing values with their median or mode.

Normalized housing prices

Standardized the features by removing the mean and scaling to unit variance

Engineered new features with increased correlation to housing prices.


## EDA

(click to enlarge)

### Checking Null Values

![GitHub Logo](/graphs/im6.png)





Reason for such high null values is that some houses do not have pools, fences or fireplaces therefore they are designated as null.
 
 &nbsp;  
 
 
### Checking Correlations

 
Correlation Scatter Matrix            |  Correlation Heat Map     
:-------------------------:|:-------------------------:
![](/graphs/im2.png )  |  ![](/graphs/im5.png)




We can see many linear correlations between the price and other features. It shows that we can also remove a lot of the features with little predictive value. Maybe create new ones as well. For instance, Overall Quality * size of 1st floor. 


 &nbsp;  

### Some Categorical Data

Overall Quality            |  Year Built
:-------------------------:|:-------------------------:
![](/graphs/im3.png )  |  ![](/graphs/im4.png)

Overall Quality looks like a good predictor. However, there doesn't seem to be a strong relationship between Year Built and Sale Price

## Model Building and Performance

#### Decision Tree Regressor

Mean: 0.19604384670583616

Standard deviation: 0.02391913580318775

#### Linear regression

Mean: 0.19501553190431847

Standard deviation: 0.0188229654440847

#### Random forest
Mean: 0.13793490937539316

Standard deviation: 0.015427082599145223

 &nbsp;  

**Best performing algorithm has been random forest.**
