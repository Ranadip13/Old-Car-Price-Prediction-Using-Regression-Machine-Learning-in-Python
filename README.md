# Old Car Price Prediction Using Regression Machine Learning in Python
The objective of this project is to determine the accurate price of a second-hand car. Based on specifications such as the number of years the car has been used, fuel type, total KM it has run, etc. a predictive model can be built to estimate the appropriate price.

In this project, a step-by-step approach to creating a Machine Learning predictive model for such scenarios was discussed. This flow can be used as a template to solve any supervised ML Regression problem.
The flow of the case study is as below:
- Reading the data in python
- Defining the problem statement
- Identifying the Target variable
- Looking at the distribution of Target variable
- Basic Data exploration
- Visual Exploratory Data Analysis for data distribution (Histogram and Barcharts)
- Feature Selection based on data distribution
- Outlier treatment
- Missing Values treatment
- Visual correlation analysis
- Statistical correlation analysis (Feature Selection)
- Selecting final predictors for ML
- Converting data to numeric for ML
- Splitting the data into Training and Testing sample
- Standardization / Normalization of data (if required)
- Sampling and K-fold cross validation
- Trying multiple Regression algorithms
- Selecting the best Model
- Deploying the best model in production

##### Data description: The business meaning of each column in the data is as below
- Price: The Price of the car in dollars
- Age: The age of the car in months
- KM: How many KMS did the car was used
- FuelType: Petrol/Diesel/CNG car
- HP: Horse power of the car
- MetColor: Whether car has metallic color or not
- Automatic: Whether car has automatic transmission or not
- CC: The engine size of the car
- Doors: The number of doors in the car
- Weight: The weight of the car

Following the above steps, various classification machine learning algorithms were tried, including Linear Regression, Decision Trees, Random Forest, AdaBoost, XGBoost, KNN, and their average accuracies were calculated. In this case, multiple algorithms have produced similar average accuracy, so any one of them can be chosen. XGBOOST is selected as the final model since it is producing the best accuracy on this data.

To deploy the model, the following steps are followed:
1.	Train the model using 100% of the available data.
2.	Save the model as a serialized file for storage and future use.
3.	Develop a Python function that integrates with front-end applications to take inputs and return predictions.
