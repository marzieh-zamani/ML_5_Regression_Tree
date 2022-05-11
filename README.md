# Project 5: Regression Tree, Cross Validation, Bagging, and Random Forest
Regression tree, cross validation, bagging, and random forest on Carseats sale dataset.

## Code Breakdown
### Step 0: Define function_0 to normalize the dataset
`input_feature_norm = function_0(input_feature)`

### Step 1: Define function_1 to caluculate MSE
`mse = function_1(y_true, y_pred)`

### Step 2: Import carseats sale data from carseats_sale.csv
1. Importing carseats sale data from carseats_sale.csv using panda.read_csv function;
2. Processing numeric and categorical features
3. Creating dummy variables
4. Converting df to ordinal df: df_ord
5. Converting string categories to numerical values
6. Converting Panda data to Numpy data
7. Spliting features and target
8. Splitting train and test data

### Step 3: Use Scikit Learn DecisionTreeRegressor() functions to fit regression tree to model and predict the output
For full depth tree (depth = 16) and pruned tree (depth = 4): 
1. Fit regression tree to model
2. Predict using fit trees.

### Step 4: Implement K-fold Cross Validation to find the depth for best test MSE (best_test_depth)
Use cross-validation in order to determine the optimal level of tree complexity. 
Plot MSE vs. tree depth.
Find the depth for best test MSE (best_test_depth).

### Step 5: Implement the bagging approach on regression trees with the best_test_depth
Use the bagging approach in order to analyse this data. Obtain the test MSE.

### Step 6: Implement the random forest approach on regression trees with the best_test_depth
Use random forests to analyse this data. Obtain the test MSE.

## Main files to check
The main file to check is the Jupyter notebook where:
- The functions are defined;
- The data is given;
- Then, the functions are called;
- The results are displayed and saved.

## Setup
Install [Miniconda](https://conda.io/miniconda).
Then, run the jupyter notebook in the "code" folder.

## Acknowledgment and References
This project has been developed based on the assignment provided by Dr. Abdul Bais, P.Eng. (abdul.bais@uregina.ca), my instructor for the course “ENEL-865/ENSE 865: Applied Machine Learning”.

This assignment is based on the first assignment of Machine Learning Regression course (from Coursera). 

- Dr. Abdul Bais, P.Eng. (abdul.bais@uregina.ca) page: 
https://www.uregina.ca/engineering/faculty-staff/faculty/bais-abdul.html

## Dataset
Download the Carseat sale dataset from https://r-data.pmagunia.com/dataset/r-dataset-package-islr-carseats. Random split data into 80% training and 20% test data.

## My contribution
All scripts are written by my self.
______________
Marzieh Zamani