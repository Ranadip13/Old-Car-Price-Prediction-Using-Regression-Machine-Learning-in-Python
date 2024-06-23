# Old Car price prediction - Regression ML project
To evaluate the appropriate price for a second-hand/old car, one typically considers factors such as the number of years, the type of fuel, and the number of kilometers it has run. In this project, the task is to create a machine learning model that can predict the price of a car based on its specifications.

In this project, a step-by-step approach to creating a Machine Learning predictive model for such scenarios was discussed. This flow can be used as a template to solve any supervised ML classification problem.
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
- Trying multiple classification algorithms
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

The final step is to deploy the model. To deploy the model, the following steps are followed.
1. Train the model using 100% data available
2. Save the model as a serialized file which can be stored anywhere
3. Create a python function which gets integrated with front-end (like Tableau) to take all the inputs and returns the prediction
