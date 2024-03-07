# Customer Churn Prediction in Telecom

## 1. The purpose of the project is to predict churning customers.

## 2. Loading the data

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/4cfccceb-9b21-443f-b75c-91cf126d3e41)

### This dataset is imbalanced, with an 85% to 15% ratio.

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/842777d3-406e-41e6-9673-81fb984ef1b4)

### Next, define column classification with labels and features, distinguishing between categorical and numerical variables.

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/5a598999-bfaf-4a72-891c-e3e3776c6d4f)

## 3. Exploratory Data Analysis - EDA
 ### - Correlation heatmap

![image](https://github.com/DzungDo82/TeleChurn/assets/138108830/5aaeeab2-4b8d-4260-ae6e-b2ab587b619b)

### From the heatmap, eliminate the four identical columns (with correlation coefficient = 1): `Total day minutes`, `Total eve minutes`, `Total night minutes`, and `Total intl minutes`.
