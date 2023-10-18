# McDonald's Menu: Caloric Analysis

**Introduction:** McDonald's is a globally known fast food resteraunt that's recognizable in 118 countries. This fast food chain has varouis menus that differ across each region and are known to have tasty food options raning from there Breakfast, Lunch, Dinner Beverages and Desserts. For this menu analysis, we are exploring the correlation between nutritional components and calorie values. I retrieved a dataset from Kaggle.com in which I leveraged Excel to the verify integrirty of the data to ensure it's clean and ready for analysis. This dataset can be accessed here: https://www.kaggle.com/datasets/mcdonalds/nutrition-facts 

**Tools used for analysis:** Excel, SQL and Tableau.

**Goal:** In this data analysis project, the goal is to conduct a exploratory analysis of the nutritional elements within the McDonald's menu. The focus is to pinpoint the healthiest and least healthy menu items based on their respective calorie values. McDonald's is one of the largest and most popular fast-food chains globally, and understanding the nutritional profile of its menu items can provide valuable insights for both consumers and the company itself in promoting healthier food choices.

**Metrics:** The metric used for this project is going to be based on the calorie intake and meal consumption reccomended by the World Health Orginzation. Accoridng to the World Health Orginzaiton, the recommended calorie intake for Men is 2,500 calories and for women is 2,000 calories, divded across three balanced meals daily. Based on these reccomended values we will use our own custom formula using Excel to retrieve our metric value that will be used for each item in the dataset.
Metirc Formula =(AVERAGE(2500,2000)/3)
Metric for this analysis: **750 calories**

**Questions to answer:**

How many items are in this dataset? How many items are there per meal type?

What are the maximum values of the the nutritional components from the menu?

Which top 10 items contain the highest amount of calories?

Which meal type contains the most items exceeding 750 calories?

How many items contain more than 750 calories? Which items are they?

Do the top 5 items with the highest Trans Fat, Saturated Fat, & Total Fat exceed 750 calories? If an item has high Total Fat does it correlate to a rise in overall calories?

Do the top 5 items with the highest sodium exceed 750 calories calories? 

Do the top 5 items with highest protein exceed 750 calories? 




**Preparing the data:** I leveraged Excel prior to jumping into this analysis to ensure that the dataset was clean and did not contain any cells that can cause potential inaccuracies when querying the data in SQL. This dataset originally was grouped into 7 categories being Breakfast, Beef & Pork, Chicken & Fish, Salads, Snacks & Sides, Desserts, and Beverages. To consolidate the categories and be able to analyze the data, I utilized SQL to create a new column in which I recategorized Beef & Pork, Chicken & Fish, and Salads as Lunch & Dinner. The reason being is because these catergories are normally ordered in the afternoon to the evening, and consolidating these categories into one gives a better overview of the nutrtional componenets specifically for meals that are consumed later in the day. Same goes for the Snacks & Sides, I recategorized these items into one category being Snacks & Deserts for the same reasons, these foods are normally consumed later in the day and this gives a better overview of the nutritional componenets. To summarize my preperation, my dataset is going to analyze four categories of food items being, Breakfast, Lunch & Dinner, Snacks & Sides and Beverages. By consolidating these categories is going to give straightforward insights of the menu and how the nutritonal components differ from one another.
