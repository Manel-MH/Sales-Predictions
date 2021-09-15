# Sales-Predictions


  This project uses the dataset from the Big Mart Sales Practice Problem. It is a first learning project on the Coding Dojo DataScience course for which this is produced. 
  The project is carried out using Python and the Google Colab cloud environment to build a predictive model.
  Google Colab is an open source development tool published by Google. It has built-in GitHub and Google Drive integration. It is a free IDE Jupyter notebook with GPU support.
  Pandas and NumPy are open-source Python packages, the former built on top of the later, that are used to handle data pre-processing, exploration, visualization, engineering and analysis for the development of an accurate machine learning model method for predictive forecast of a target vector.
  The goal of this project is to highlight some of the most commonly used tools in Pandas/NumPy data pre-processing, exploration, visualization, engineering and analysis in order to feed our dataset into a machine learning algorithm. The analysis will aim at predicting the target vector using several supervised predictive model methods.
	The dataset showcases sales for food items sold at various stores. The target vector “Item_Outlet_Sales” is a continuous variable and to predict it, we will develop supervised machine learning regression methods. These regressor methods will be optimized and compared to one another to select the most performant machine learning algorithm to carry out the predictive task.


# Dataset


This is .info() output. The dataset shape is 8523 entries and 12 columns. 

![Screen Shot 2021-09-14 at 23 03 46](https://user-images.githubusercontent.com/87575638/133364027-8588a478-8078-44d6-a470-e0b52e779d14.png)


# Data Cleaning
 
 Uniformisation of categorical data for feature Item_Fat_Content
 
 ![Screen Shot 2021-09-14 at 23 14 35](https://user-images.githubusercontent.com/87575638/133364714-fce9f664-1410-4fb7-9ce6-1f51d5f9490f.png)
 
 
 Missing values handling for features Outlet_Size and Item_Weight
 
 
![Screen Shot 2021-09-14 at 23 18 35](https://user-images.githubusercontent.com/87575638/133365241-784cc22a-5245-4494-9a97-cd6d97cdc8d0.png)


![Screen Shot 2021-09-14 at 23 17 59](https://user-images.githubusercontent.com/87575638/133365134-2ececa3d-b98e-4064-adbf-93710677de6f.png)
 
 
 
# Data Vizualisation and Statistics

This is a .describe()

![Screen Shot 2021-09-14 at 23 25 21](https://user-images.githubusercontent.com/87575638/133365655-a88edebf-012b-4c90-ae51-3fc579a82af8.png)

The target vector of interest is Item_Outlet_Sales. The following heatmap showcases our target vector correlation with other numerical features.

![Screen Shot 2021-09-14 at 23 30 15](https://user-images.githubusercontent.com/87575638/133366019-d4f843ca-c0e6-405a-81a3-2a91d2dba704.png)

Relationship between a categorical feature Outlet_Size and our target vector with a boxplot graph.

![Screen Shot 2021-09-14 at 23 35 08](https://user-images.githubusercontent.com/87575638/133366502-77a36808-165e-4c1c-b41a-845f018ba61d.png)

# Regression Models

Change categorical data with encoding

![Screen Shot 2021-09-14 at 23 41 57](https://user-images.githubusercontent.com/87575638/133367056-4ae71952-4660-4341-8f98-7cf1dc2e1087.png)

We will predict our target vector Item_Outlet_Sales against the matrix features present in the dataset.

![Screen Shot 2021-09-14 at 23 44 45](https://user-images.githubusercontent.com/87575638/133367303-abece4d6-b348-4701-8d20-ffb7d7d545a2.png)

We built several regression models with linear regression, decision tree, bagged tree and random forest methods. The measure of performance we use below is RMSE. Accoriding to this measure of performance we can see that all models performed well, the best method in our process is random forest trees. 


![Screen Shot 2021-09-14 at 23 47 49](https://user-images.githubusercontent.com/87575638/133367564-d9c6e16a-935b-48af-b7d1-a531b963db10.png)

# Feature Importance 

This feature importance ranking will help us make decision as to steps ahead.

![Screen Shot 2021-09-14 at 23 54 00](https://user-images.githubusercontent.com/87575638/133368120-915081ff-51ad-428a-b851-2b2b7e3dfea6.png)

![Screen Shot 2021-09-14 at 23 56 12](https://user-images.githubusercontent.com/87575638/133368286-8dacd6c1-b670-49a5-bb05-4d8736edaed5.png)


# Recommendations

Our target vector is correlated with features Item_MRP, Outlet_Type_GroceryStore, Item_Visibilty and Outlet_Type_SupermarketType 3. To increase Item_Outlet_Sales working on the visibility/access of items is an avenue to work on. It seems Grocery stores and Supermarket Type 3 importance needs to be assessed further to understand the relationship better. 

