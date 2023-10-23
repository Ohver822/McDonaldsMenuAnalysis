# McDonald's Menu: Caloric Analysis

**Introduction:** McDonald's is a globally known fast food resteraunt that's recognizable in 118 countries. This fast food chain is known to have tasty food options across their menu. For this project I will be conducting a calorie analysis to see how high calorie items correlate with other nutrtional components. I retrieved a dataset from Kaggle.com in which I leveraged Excel to the verify integrirty of the data to ensure it's clean and ready for analysis. This dataset can be accessed here: https://www.kaggle.com/datasets/mcdonalds/nutrition-facts 

**Tools used for analysis:** Excel, SQL and Tableau.

**Goal:** The goal of this project is to conduct a exploratory analysis of the nutritional elements within the McDonald's menu. The focus is to pinpoint the highest calorie items exceeding 750 calories, and see if the calorie value indicates that all other nutrtional components contain high values as well. 

**Metric:** The metric used for this project is going to be based on the calorie intake and meal consumption reccomended by the World Health Orginzation. Accoridng to the World Health Orginzaiton, the recommended calorie intake for Men is 2,500 calories and for women is 2,000 calories, divded across three balanced meals daily. Based on these reccomendedations I will use Excel to retrieve the metric value that will be used for this analysis.
Metirc Formula =(AVERAGE(2500,2000)/3)
Metric for this analysis: **750 calories**

**Questions to answer:**

How many items are in this dataset? How many items are there per meal type?

What are the maximum calories for each Category?

What are the top 5 highest calorie items per meal type?

How many items contain more than 750 calories? Which items are they?

Do the top 5 items with the highest Trans Fat, Saturated Fat, & Total Fat exceed 750 calories? 

At which percentage of fat does an item start exceeding 750 calories?

Do the top 5 items with the highest sodium, carbohydrates and protein exceed 750 calories calories? 

Categorize items by calorie ranges: 0-299, 300-599, 600-749, 750 or more.



**Preparing the data:** I leveraged Excel prior to jumping into this analysis to ensure that the dataset was clean and did not contain any cells that can cause potential inaccuracies when querying the data in SQL. This dataset originally was grouped into 7 categories being Breakfast, Beef & Pork, Chicken & Fish, Salads, Snacks & Sides, Desserts, and Beverages. To consolidate the categories and be able to analyze the data, I utilized SQL to create a new column in which I recategorized Beef & Pork, Chicken & Fish, and Salads as Lunch & Dinner. The reason being is because these catergories are normally ordered in the afternoon to the evening, and consolidating these categories into one gives a better overview of the nutrtional componenets specifically for meals that are consumed later in the day. Same goes for the Snacks & Sides, I recategorized these items into one category being Snacks & Deserts for the same reasons, these foods are normally consumed later in the day and this gives a better overview of the nutritional componenets. To summarize my preperation, my dataset is going to analyze four categories of food items being, Breakfast, Lunch & Dinner, Snacks & Sides and Beverages. By consolidating these categories is going to give straightforward insights of the menu and how the nutritonal components differ from one another.
