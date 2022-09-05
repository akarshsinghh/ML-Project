# IE7374 FINAL PROJECT REPORT
## Online Shopper's Purchasing Intention [Group 10]
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

