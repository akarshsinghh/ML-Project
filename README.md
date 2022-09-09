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
Before we started training, the first step we took was to split the data into train and test data sets. We trained the model using the training dataset and evaluated the fit model using the test dataset. We also have split the data into folds for k-fold cross-validation for one of the machine learning models. Splitting the dataset into train, validation and test data helps in removing bias and in hyper-tuning the parameters.

### Exploratory Data Analysis and Visualization:
To get a complete overview of the dataset we were dealing with, we created a function that described the dimensions. The description includes the categorical attributes, numerical attributes, number of null values in all the columns and many more. 

![fig1](https://user-images.githubusercontent.com/66643857/189428827-f50af644-6621-4d56-adae-d18694346f79.jpg)
![fig2](https://user-images.githubusercontent.com/66643857/189428831-0c4912db-6834-4156-844f-91e47e12d7d8.jpg)
![fig3](https://user-images.githubusercontent.com/66643857/189428834-51399e53-1b50-4f8d-8aea-6867c1b09073.jpg)
![fig4](https://user-images.githubusercontent.com/66643857/189428849-48ed88e5-ba27-43cf-997b-0e6f0caa9434.jpg)
![fig5](https://user-images.githubusercontent.com/66643857/189428856-6f651301-8834-4e4d-a9c8-494cfe74936f.jpg)

All the attributes of the dataset contained non-null values. Hence, null value processing was not required. We then shifted our focus towards finding the correlation of each attribute with every other attribute in the table to remove recursive information.

![fig6](https://user-images.githubusercontent.com/66643857/189435495-6ab8b4b9-65e9-40e9-9ea9-52105ee934ca.jpg)

We see a high correlation between the ‘BounceRate’ and the ‘ExitRates’ (0.91) and between the ‘ProductRelated_Duration’ and the ‘ProductRelated’ (0.86). These columns were dealt with while Feature selection. 

 We plotted a bar plot to find the count values of the two classes in our dataset. 

![fig7](https://user-images.githubusercontent.com/66643857/189435617-628aefdf-2366-49ae-b0e2-cab42578c2bb.jpg)

The number of false cases heavily outweighs the number of True classes. From this graph, we realised that we had to work with the skewness in data by either upsampling or down-sampling the data while passing the training data sets into the model. 

To evaluate the distribution of values of the columns with relatively high correlation values with the ‘Revenue’ column, a bar plot was used.

![fig8](https://user-images.githubusercontent.com/66643857/189436022-dba33775-03b3-4b24-89c4-16239b330f34.jpg)

The data is highly skewed concerning revenue with many outliers. The skewness of the columns is dealt with while the skew handling process and the outlier and dealt with during Data preprocessing and cleaning.

In the next part, we checked for the linear separability of the two classes for the subset of the total number of attributes in our dataset. We used a grid plot for this case. The lower diagonal shows the kernel density estimate of the distribution concerning the attribute pairs, the upper diagonal shows the scatter plot of the same attribute pairs and the diagonal shows the distribution of attribute values across the dataset using kernel density estimate plot. The ‘TotalDuration’ here denotes the summation of the ‘Administrative_Duration’, the ‘Informational_Duration, and the ‘ProductRelated_Duration’.

![fig9](https://user-images.githubusercontent.com/66643857/189436377-ddbe6782-11bc-4a58-a8fd-e5ff85a46f1c.jpg)

