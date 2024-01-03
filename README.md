# Prediction with Multiple Linear Regression
***

### Projects:

(i) Predicting the profit obtained in the startups from different states using R&D, administration and marketing spendings, respectively. 

(ii) Prediction of Toyota Corolla car price depnding upon the various parameters including cc, hp, km, etc
***
### Objectives:

Exploring Insights/Inferences by performing EDA on the given data. Relevant graphs were plotted to get some insights on data using seaborn package. Model fitting via linear regression by Importing sklearn package. Selecting the best fitted model via python programming.
***

### 50_Startups data Probelm: 
*File name: 50-Startups-data-files.zip*

* EDA concluded that R&D spending results in a linear increase in the profit earned by the startups from different countries. Also, the profit of the startups partially depends upon the Marketing spending.
* Florida has earned the maximum profit and has maximum (R&D and Marketing) spending followed by New York and California. T
* The profit earned in the startups is likely to depend upon the R&D and marketing spend.
* The data is normally distributed in all the cases. Since the skewness is calculted to be **0.20, 0.16,-0.49 and -0.05** for Profit, R&D, Administration and Marketing spend, respectively.
* Box plot shows that there are no outliers present in R&D, administration and marketing spend data but Profit data has one outlier which is succesfully removed.
* All these findings depicts that profit majorly depends on R&D and Marketing spend.
* In order to find the best fitted model, the data has been fitted with 3 different models
  * Method-1 : Multiple linear regression 
  * Method-2 : Ridge or L2 regression
  * Method-3 : Lasso or L2 regression
* The Correlation of R&D spending, Administration and Marketing with profit came out to be: **97%, 20%, 75%**, respectively
* In all the cases of linear regression, the model data is divided into train and test data by importing train_test_split from sklearn.model_selection package.
* In case of multiple linear regression, first one hot encoding is performed on the test data (states) then x and y values were choosen and model is divided into train and test data.
* The model data is then fitted by importing linear regression from sklearn.linear_model
* The fitted model is then used for the prediction of values which is done using the test data.
* The error is calculated by importing r2_score, mean_squared_earror from sklear.metrics
* The strength of the models (R square) is came out to be:
  
  |Methods | R square value|
   -------  --------------
  |Method 1 | 0.965      |
  
  |Method 2 | 0.941      |
  
  |Method 3 | 0.954     |
  
* R square value lies between 0 and 1 and the model is strongest when approaches 1 and weakest when approaches 0.
**All the model are very strong and Model 1 which is multiple linear regression is the strongest**.
* The model is saved by importing joblib package (50_startups_data_prj3.sav)
***


### Toyota_Corolla data Probelm: 
*File name: Toyota-Corolla-data-files.zip*

* EDA concluded that that increase in Age and Kilometers travelled by car results in the decrease in the car prices. 
* The relation between CC and Price of the car, implying that they are not correlated.T
* The price of the car partially depends upon its weight and does not have much affect on prices due to the car’s weight.
* The data is not normally distributed in all the cases. 
* Box plot shows that there are outliers present in Price, Age, KM, CC, HP and Quaterly tax and has been succesfully removed.
* The Correlation of Age, KM, CC, Weight, Quaterly_tax with price of car came out to be: **88%, 57%, 13%, 58% and 22%**, respectively
* All these findings depicts that profit majorly depends on Age, KM, Weight.
* In order to find the best fitted model, the data has been fitted with 3 different models
  * Method-1 : Multiple linear regression 
  * Method-2 : Ridge or L2 regression
  * Method-3 : Lasso or L2 regression
  * Method-4 : Polynomial regression
* In all the cases of linear regression, the model data is divided into train and test data by importing train_test_split from sklearn.model_selection package.
* In case of multiple linear regression, first one hot encoding is performed on the test data (states) then x and y values were choosen and model is divided into train and test data.
* The model data is then fitted by importing linear regression from sklearn.linear_model
* The fitted model is then used for the prediction of values which is done using the test data.
* The error is calculated by importing r2_score, mean_squared_earror from sklear.metrics
* The strength of the models (R square) is came out to be:
  
  |Methods | R square value|
   -------  --------------
  |Method 1 | 0.773      |
  
  |Method 2 | 0.718      |
  
  |Method 3 | 0.718     |
  
  |Method 4 | 0.755     |
  
* R square value lies between 0 and 1 and the model is strongest when approaches 1 and weakest when approaches 0.
**All the model are strong and Model 1&4 i.e., multiple linear regression and polynomial regression are the strongest**.
* The model is saved by importing joblib package (ToyotaCorolla_prj4.sav)
