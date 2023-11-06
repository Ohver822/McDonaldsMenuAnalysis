# McDonald's Menu: Caloric Analysis

**Introduction:** McDonald's is a globally known fast food resteraunt that's recognizable in 118 countries. This fast food chain is known to have tasty food options across their menu. For this project I will be conducting a calorie analysis to see how high calorie items correlate with other nutrtional components. I retrieved a dataset from Kaggle.com in which I leveraged Excel to the verify integrirty of the data to ensure it's clean and ready for analysis. This dataset can be accessed here: https://www.kaggle.com/datasets/mcdonalds/nutrition-facts 

**Tools used for analysis:** Excel, SQL and Tableau.

**Goal:** The goal of this project is to conduct a exploratory analysis of the nutritional elements within the McDonald's menu. The focus is to pinpoint the highest calorie items, and see if the calorie value indicates that all other nutrtional components contain high values as well. 

**Questions to answer:**

1. What is the distribution of calorie values in the dataset, and are there any extreme outliers?

2. Can you identify any statistically significant correlations between calorie content and macronutrients (such as carbohydrates, proteins, and fats) in the dataset?

3. Are there any trends or patterns in how high-calorie items relate to specific food categories or types (e.g., desserts, fast food, healthy options)?

4. What is the average calorie content in different meal types (breakfast, lunch, dinner, snacks), and do these values vary significantly?

5. Is there a relationship between the calorie content of a food item and its portion size or serving size?

6. Can you identify any seasonal or temporal trends in high-calorie food consumption, and how do these trends correlate with other nutritional components?

7. Are there specific combinations of nutritional components (e.g., high calorie, high fat, low protein) that are common in certain types of cuisine or dishes (e.g., Italian, Asian, American)?

8. How do high-calorie items in the dataset compare in terms of calorie density (calories per unit weight or volume) to low-calorie items, and what insights can this provide about food choices and nutritional density?


**Preparing the data:** I leveraged Excel prior to jumping into this analysis to ensure that the dataset was clean and did not contain any cells that can cause potential inaccuracies when querying the data in SQL. This dataset originally was grouped into 7 categories being Breakfast, Beef & Pork, Chicken & Fish, Salads, Snacks & Sides, Desserts, and Beverages. To consolidate the categories and be able to analyze the data, I utilized SQL to create a new column in which I recategorized Beef & Pork, Chicken & Fish, and Salads as Lunch & Dinner. The reason being is because these catergories are normally ordered in the afternoon to the evening, and consolidating these categories into one gives a better overview of the nutrtional componenets specifically for meals that are consumed later in the day. Same goes for the Snacks & Sides, I recategorized these items into one category being Snacks & Deserts for the same reasons, these foods are normally consumed later in the day and this gives a better overview of the nutritional componenets. To summarize my preperation, my dataset is going to analyze four categories of food items being, Breakfast, Lunch & Dinner, Snacks & Sides and Beverages. By consolidating these categories is going to give straightforward insights of the menu and how the nutritonal components differ from one another.
