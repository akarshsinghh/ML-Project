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

![fig1](https://user-images.githubusercontent.com/66643857/189428133-e6545d4d-2ea7-45eb-8bbc-013372d11b64.jpg)
![fig2](https://user-images.githubusercontent.com/66643857/189428136-f45a0688-d2d1-46a6-bc71-74ad597b5f9b.jpg)
![fig3](https://user-images.githubusercontent.com/66643857/189428137-e25553cb-0d30-416c-b95a-500eb73300ab.jpg)
![fig4](https://user-images.githubusercontent.com/66643857/189428141-17ebd5b4-737c-4cbe-a2f4-b681bb861749.jpg)
![fig5](https://user-images.githubusercontent.com/66643857/189428163-b73060db-916d-4fee-a770-d9064a9d972e.jpg)

