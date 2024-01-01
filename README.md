Using Multiple linear regression:

(i) Predicting the profit obtained in the startups from different states using R&D, administration and marketing spendings, respectively. Exploring Insights/Inferences by performing EDA on the given data. Relevant graphs were plotted to get some insights on data using seaborn package. Model fitting via linear regression by Importing sklearn package. Selecting the best fitted model via python programming.

50_Startups data Probelm: File name: Project-3-MultipleReg-50-Startups.ipynb

(a) EDA concluded that R&D spending results in a linear increase in the profit earned by the startups from different countries. Also, the profit of the startups partially depends upon the Marketing spending.
(b) Florida has earned the maximum profit and has maximum (R&D and Marketing) spending followed by New York and California. Therefore, the profit earned in the startups is likely to depend upon the R&D and marketing spend.
(c) The data is normally distributed in all the cases. Since the skewness is calculted to be **0.20, 0.16,-0.49 and -0.05** for Profit, R&D, Administration and Marketing spend, respectively, which are between -1 and 1.
(d) Box plot shows that there are no outliers present in R&D, administration and marketing spend data but Profit data has one outlier which is adjusted or removed by using quartiles and lower threshold values.
(e) All these findings depicts that profir majorly depends on R&D and Marketing spend.
(f) In order to find the best fitted model, the data has been fitted with 3 different models
         Method-1 : Multiple linear regression 
         Method-2 : Ridge or L2 regression
         Method-3 : Lasso or L2 regressionsimple linear regression 
         
(g) The Correlation of R&D spending, Administration and Marketing with profit came out to be: **97%, 20%, 75%**, respectively
(h) In all the cases of linear regression, the model data is divided into train and test data by importing train_test_split from sklearn.model_selection package. 
(i) In case of multiple linear regression, first one hot encoding is performed on the test data (states) then x and y values were choosen and model is divided into train and test data. 
(j) The model data is then fitted by importing linear regression from sklearn.linear_model 
(k) The fitted model is then used for the prediction of values which is done using the test data. 
(l) The error is calculated by importing r2_score, mean_squared_earror from sklear.metrics 
(m) The strength of the models (R square) is came out to be:
       **Method-1 : 0.965 
         Method-2 : 0.941
         Method-3 : 0.954**
R square value lies between 0 and 1 and the model is strongest when approaches 1 and weakest when approaches 0.
**All the model are very strong and Model 1 whoch is multiple linear regression is the strongest**.
(n) The model is saved by importing joblib package (50_startups_data_prj3.sav)



(ii) Predicting the profit obtained in the startups from different states using R&D, administration and marketing spendings, respectively. Exploring Insights/Inferences by performing EDA on the given data. Relevant graphs were plotted to get some insights on data using seaborn package. Model fitting via linear regression by Importing sklearn package. Selecting the best fitted model via python programming.

50_Startups data Probelm: File name: Project-3-MultipleReg-50-Startups.ipynb

(a) EDA concluded that R&D spending results in a linear increase in the profit earned by the startups from different countries. Also, the profit of the startups partially depends upon the Marketing spending.
(b) Florida has earned the maximum profit and has maximum (R&D and Marketing) spending followed by New York and California. Therefore, the profit earned in the startups is likely to depend upon the R&D and marketing spend.
(c) The data is normally distributed in all the cases. Since the skewness is calculted to be **0.20, 0.16,-0.49 and -0.05** for Profit, R&D, Administration and Marketing spend, respectively, which are between -1 and 1.
(d) Box plot shows that there are no outliers present in R&D, administration and marketing spend data but Profit data has one outlier which is adjusted or removed by using quartiles and lower threshold values.
(e) All these findings depicts that profir majorly depends on R&D and Marketing spend.
(f) In order to find the best fitted model, the data has been fitted with 3 different models
         Method-1 : Multiple linear regression 
         Method-2 : Ridge or L2 regression
         Method-3 : Lasso or L2 regressionsimple linear regression 
         
(g) The Correlation of R&D spending, Administration and Marketing with profit came out to be: **97%, 20%, 75%**, respectively
(h) In all the cases of linear regression, the model data is divided into train and test data by importing train_test_split from sklearn.model_selection package. 
(i) In case of multiple linear regression, first one hot encoding is performed on the test data (states) then x and y values were choosen and model is divided into train and test data. 
(j) The model data is then fitted by importing linear regression from sklearn.linear_model 
(k) The fitted model is then used for the prediction of values which is done using the test data. 
(l) The error is calculated by importing r2_score, mean_squared_earror from sklear.metrics 
(m) The strength of the models (R square) is came out to be:
       **Method-1 : 0.965 
         Method-2 : 0.941
         Method-3 : 0.954**
R square value lies between 0 and 1 and the model is strongest when approaches 1 and weakest when approaches 0.
**All the model are very strong and Model 1 whoch is multiple linear regression is the strongest**.
(n) The model is saved by importing joblib package (50_startups_data_prj3.sav)


