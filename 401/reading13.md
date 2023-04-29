## Linear Regressions

#### Things I Want to Know More About



### How to Run Linear Regression in Python

1. Can you explain the basic concept of linear regression and its purpose in the context of machine learning and data analysis?

Linear regression allows us to find a straight line that "best fits" a set of scattered data points, and further allows prediction of new data points.  

Input = independent feature x or explanatory variable

Output = dependent feature, y or response variable

Slope = steepness of the regression

Correlation= the relation b/n 2 vars in terms of strength and degree, values b/n -1.0 and 1.0 

Residual = vertical distance b/n a data point and the line of regression, variance

import scikit-learn for the LinearRegression class. 

### Linear Regression in Python

Working to find a function that maps some features or variables to other sufficiently well. 

To get the best weights, minimize the sum of the squared residuals for all observations, method of ordinary least squares

Underfitting: model can't accurate capture the dependencies among the data, cannot predict new data, misses the trends in the data. 

Overfitting: model learns both data dependencies and random fluctuations. Model learns the existing data too well and describes the noise in the training data, instead of the actual relationships between the variables in the data.  

### Intro to Simple Linear Regressions

Regression analysis explores the relationship b/n a quantitative response variable and one or more explanatory variables.

Start by plotting the data pairs. 

One explanatory variable is simple regression vs mutliple regression. 

Sometimes you may want to measure the strength of the relationship b/n x and y.

note: random error component, there will be some variablity in the data points

2. Describe the process of implementing a linear regression model using Python’s Scikit Learn library, including the necessary steps and functions.

Scikit-learn built on top of NumPy. 

1. Import packages and classes that you need
2. Provide data to work with, eventually do the appropriate transformations
3. Create a regression model, fit w/ existing data
4. Check results of model fitting for accuracy
5. Apply the model for predictions

Once you provide the np.array, call `.reshape((-1,1))` to create a 2_D model (-1,1) which will create one column and as many rows as necessary. -1 is a placeholder when you do not know how many rows there will be. 

`model = LinearRegression()`

Optional params for the class: fit_intercept, Boolean defaults to True, normalize, defaults to False, copy_x, Ture by default, n_jobs, an integer or None

Then fit the model: `model.fit(x,y)` or `model = LinearRegression().fix(x,y)`

Then get results: 

`r_sq = model.score(x, y)`
`print(f"coefficient of determination: {r_sq}")`

To check the results:

`print(f"intercept: {model.intercept_}")`
`intercept: 5.633333333333329`

`print(f"slope: {model.coef_}")`

Finally, apply for predictions: 

`y_pred = model.predict(x)`
`print(f"predicted response:\n{y_pred}")`

### Train and Test Splits

3. What is the purpose of splitting the dataset into train and test sets, and how does this contribute to the evaluation of a machine learning model’s performance?

Training set contains a known output and the model learns on this data in order to be generalized to other data later on. 

The test dataset in order to test our models predictions. 

Use the train_test_split function to split 80/30 or 70/30 of the data.

Be sure to cross validate, which similar to train/test split, but applied to more subsets. 

Two methods: K-Folds Cross Validation, and Leave One Out Cross Validation. 

K-Folds uses k-1 subsets to train data and leave the last subset as test data. Then average the model against each of the fold and finalize it. Finally test it against the test set. 

LOOCV--the numver of folds equals to the number of observations in the dataset, then average, and build the model w/ the average.  Test against the last fold. Best for smaller datasets. 

### What is Linear Regression

common type of predictive analysis. 

does a set of predictor variable do a good job in predicting an outcome variable

which variables in particular are significant predictors of the outcome variable and do they predict the outcome variable? 

regression analysis for: 

(1) determining the strength of predictors, 
(2) forecasting an effect, and 
(3) trend forecasting






