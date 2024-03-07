# Customer Churn Prediction in Telecom

## 1. The purpose of the project is to predict churning customers.

## 2. Loading the data

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/4cfccceb-9b21-443f-b75c-91cf126d3e41)

#### This dataset is imbalanced, with an 85% to 15% ratio.

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/842777d3-406e-41e6-9673-81fb984ef1b4)

#### Next, define column classification with labels and features, distinguishing between categorical and numerical variables.

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/db667f76-21ac-469c-b466-4395a1005392)

## 3. Exploratory Data Analysis - EDA
 ### 3.1 Correlation heatmap

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/5aaeeab2-4b8d-4260-ae6e-b2ab587b619b)

#### -> From the heatmap, eliminate the four identical columns (with correlation coefficient = 1): `Total day minutes`, `Total eve minutes`, `Total night minutes`, and `Total intl minutes`.

 ### 3.2 Correlating categorical features

 ![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/e47ddbbc-6a62-41b7-ae27-bfb6af898df2)


### 3.3 Correlating numerical features: Histplots and Boxplots

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/cae80b39-1b67-423b-a1fb-799cc29f7e87)

#### -> High rates of customer churn occur for those with 0 to 5 customer service calls.

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/5f97d564-0e13-4075-9915-3299102bc863)

## 4. Feature Engineering

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/ae7c0853-77f1-41a6-a7d4-a6d85ccc77a6)

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/9a56b638-be1d-4fe7-b496-a60c8cca6113)

## 5. Model training
 ### 5.1 Spliting: X_train, X_val, y_train, y_val

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/dd1a8df5-fe84-40c7-95fc-74c2b7944498)

 ### 5.2 Exploring various models and evaluating the significance of different feature levels

 ![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/6e38c71a-176e-4a53-9a04-e8715128b782)

 ### 5.3 Scaling and Baseline Model Comparison

 ![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/9090e85d-8546-4fff-b000-61e7d830b224)

 ### 5.4 Combining Scaler, Sampler, and Model: the most effective combination is RobustScaler + SMOTE + RandomForestClassifier, achieving an accuracy score of 96%

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/f88cae87-e305-4919-9e3b-53b40fa86fce)
