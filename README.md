# Advance-EDA-and-feature-engineering
This projects aims to clean and correct the raw data. <br />
Please find the raw data by clicking 
[datasheet here](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)
We have taken a dataset which is as raw as it can be possible. The idea to do such EDA project is to demostrate on how to handle a raw datsheet and ways of exploring data aswell as understaning data using charts.

## Table of content


### EDA 1: <br />

 - With the help of 
 [numpy](https://numpy.org) 
 [Python3](https://www.interviewbit.com/blog/difference-between-python-2-and-3/) 
 library, the code blocks aims generate a list of feature  and find out percentages of missing value in a column.

- Wih the help of list of features which have feature names of missing value is plotted against the dependent / target feature ('SalePrice') so as to get an idea of how many colums have strong relations with dependent feature. This will eventually help us to underatsnd the need of retaining the while putting it into any ML model

- Similary we segregated numerical feture and all year based feature column.
 
 - With the help of [seaborn](https://seaborn.pydata.org) 
 and 
 [matplotlib](https://matplotlib.org)
 , we plotted few graphs for better understanding.
 
 
 ### EDA 2: <br />
 
 - We splitted our already splitted data set into train and test data using sklearn's model selection 
 [train-test-split](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html).
 
 - We treated missing values here
   - Categorical variable : <br /> with the help of if statment we collected all the categorical varible. To catch this we simply collected features with datatype as strings and replaced all null values with label as 'missing'.
   - Numerical variable : <br /> with the help of if statment we collected all the numerical varible. To catch this we simply collected features with datatype as not equall to strings and replaced all null values with 
   [median](https://vitalflux.com/pandas-impute-missing-values-mean-median-mode/) 
   values.
   - Year variable : <br /> with the help of if statment we collected all the year varible. To catch this we simply collected features with which have datatype as int, is not SalePrice, is not included in Id and is not included in numerical variables.
   
 - Handling rare Categorical Feature:<br /> With the help of 
 [numpy](https://numpy.org) 
 we recategorised the features which are present in categorical features and have contribution of less than 1 percent with tag as 'Rare'. The value of 1 percent has been chossen randomly and is mildly based on the size of dataset
 
 
 ### Feature scaling: <br />
 - Since every feature has 
     
    
