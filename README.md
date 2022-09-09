# IE7374 FINAL PROJECT REPORT
## Online Shopper's Purchasing Intention
Made by 
* Sai Vinay Teja Jakku - [jakku.s@northeastern.edu](jakku.s@northeastern.edu)
* Akarsh Singh - [singh.akar@northeastern.edu](singh.akar@northeastern.edu)
* Janvi Shetty - [shetty.j@northeastern.edu](shetty.j@northeastern.edu)
* Anurag Palanki - [palanki.a@northeastern.edu](palanki.a@northeastern.edu)

### Problem Setting & Definition:
Over the past few years, business owners and retailers, big or small, have started taking their shops online to increase their reach, promote their brand and increase sales that cover a wide range of customers. For these businesses, it is essential to identify the customer base and give them enough rewards and incentives to encourage their online purchase. The primary objective of this project is to identify patterns of the customers that browse a website and make a successful purchase. We intend to achieve this by using various Machine learning techniques and selecting the best classification algorithms that successfully classify the revenue promoting customers from other users using the Online Shoppers’ Purchasing Intention dataset.

### Data Sources:
[UCI Repository link](https://archivebeta.ics.uci.edu/ml/datasets/online+shoppers+purchasing+intention+dataset) 

### Data Description:
Of the 12,330 sessions in the dataset, 84.5% (10,422) were negative class samples that did not end with shopping, and the rest (1908) were positive class samples ending with shopping[1]. The dataset was created so that each session would belong to a different user in a year to avoid any tendency to a specific campaign, special day, user profile, or period. It contains ten numerical and seven categorical columns, with the 8th and target column being the target column.

### Splitting The Dataset:
The first step before we start training the model is to split the data into train and test data sets. We train the model using the training dataset and evaluate the fit model using the test dataset. We also have split the data into folds for k-fold cross-validation for one of the machine learning models. Splitting the dataset into train, validation and test data helps in removing bias and in hyper-tuning the parameters.

### Exploratory Data Analysis and Visualization:
To get a complete overview of the dataset we were dealing with, we created a function that described the dimensions. The description includes the categorical attributes, numerical attributes, number of null values in all the columns and many more.

![fig1](https://user-images.githubusercontent.com/66643857/189426553-1df0d788-6ee2-4ff4-92d4-4f2a61b2c5b9.jpg)
![fig2](https://user-images.githubusercontent.com/66643857/189426558-0151e923-cc2e-4554-b32d-234b7718df36.jpg)
![fig3](https://user-images.githubusercontent.com/66643857/189426567-bb1b34d7-1ca6-4649-b230-f41f7911c019.jpg)
![fig4](https://user-images.githubusercontent.com/66643857/189426574-477c12e8-5519-46c5-8ff3-a0a1a7ec9eb9.jpg)
![fig5](https://user-images.githubusercontent.com/66643857/189426584-2d50f842-d26e-42c9-a3d8-b45d2e7a2634.jpg)

