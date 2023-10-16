# McDonald's Menu: Nutrition Analysis

**Introduction:** McDonald's is a globally known fast food resteraunt that's recognizable in 118 countries. This fast food chain has varouis menus that differ across each region and are known to have tasty food options raning from there Breakfast, Lunch, Dinner Beverages and Desserts. The question in mind for this analysis how healthy is the overall menu and are people aware of nutrition facts of the tasty menu. I retrieved a dataset from Kaggle.com in which I leveraged Excel to the verify integrirty of the data to ensure it's clean and ready for analysis. This dataset can be accessed here: https://www.kaggle.com/datasets/mcdonalds/nutrition-facts 

**Tools used for analysis:** Excel, SQL and Tableau.

**Goal:** The goal of this data analysis project is to comprehensively evaluate the nutritional components of the McDonald's menu items with the primary goal of identifying the healthiest and unhealthiest item's from the menu. McDonald's is one of the largest and most popular fast-food chains globally, and understanding the nutritional profile of its menu items can provide valuable insights for both consumers and the company itself in promoting healthier food choices.

**Questions to answer:**

How many different categories are in this dataset? How many items are in this dataset? How many items are there per category?

What are the average, minimum, and maximum values of the the nutritional components from the menu?

Which category from the menu contain the highest calories? How many items contain more fat from calories than overall calories?

Which category of the menu contains the highest saturated fats? If an item has a high percentage saturated fats does it correlate to a rise in overall calories?

Which category of foods contains the highest sodium content? Does high sodium correlate with increase or decrease in carbohydrates or vice versa.

Which category of foods contains the highest sugar amount? Does high amount of sugar correlate with an increase in calories? 

Which category of foods conain high proteins? Does high amount of protein correlate with an increase in calories?

Query items with the highest content of each nutrition component, and the lowest of each nutritional component.

If the items with the max nutrtional componenets were consumed three times in one day, does it meet the standard of consuming on average 2,000 calories per day?

**Preparing the data:** I leveraged Excel prior to jumping into this analysis to ensure that the dataset was clean and did not contain any cells that can cause potential inaccuracies when querying the data in SQL. This dataset originally was grouped into 7 categories being Breakfast, Beef & Pork, Chicken & Fish, Salads, Snacks & Sides, Desserts, and Beverages. To consolidate the categories and be able to analyze the data, I utilized SQL to create a new column in which I recategorized Beef & Pork, Chicken & Fish, and Salads as Lunch & Dinner. The reason being is because these catergories are normally ordered in the afternoon to the evening, and consolidating these categories into one gives a better overview of the nutrtional componenets specifically for meals that are consumed later in the day. Same goes for the Snacks & Sides, I recategorized these items into one category being Snacks & Deserts for the same reasons, these foods are normally consumed later in the day and this gives a better overview of the nutritional componenets. To summarize my preperation, my dataset is going to analyze four categories of food items being, Breakfast, Lunch & Dinner, Snacks & Sides and Beverages. By consolidating these categories is going to give straightforward insights of the menu and how the nutritonal components differ from one another.

## Analysis of the Average, Minimum and Max values per category

To commence this analysis, my first task is to identify the nutritional components and determine their Average, Minimum, and Maximum values in order to spot outliers among these three metrics.

![image](https://github.com/Ohver822/McDonaldsMenuAnalysis/assets/86633487/f32eac87-7a38-4af5-bfdf-41d59c2d3bf6)


Clearly, among all the food categories, 'Lunch & Dinner' stands out as the one with the highest calorie count, boasting an impressive 1,880 calories for one of my McDonald's food items. Another outlier of the category with the lowest calorie count lies in the 'Snacks & Desserts' category with light 15 calorie food item (water not included).

### Calorie Analysis (Low Vs High)

![image](https://github.com/Ohver822/McDonaldsMenuAnalysis/assets/86633487/f62697f4-4178-40ff-b62a-faba5381bdb2)

**Insight for Consumers:**
Apple Slices stand out as the menu's most calorie-friendly option, containing just 15 calories, while the Chicken McNuggets (40-piece) top the list with the highest calorie content. This information is valuable for individuals striving to maintain a balanced diet as well as those seeking to increase their calorie intake.

**Insight for Company:**
These insights can be indicators to possible reevaluate the menu depending on business expectations and considfer offering more calorie friendly options, or including more items on the menu that can meet the standards of containing foods with high calories.

### Calories from Fat Analysis (Low Vs High)

![image](https://github.com/Ohver822/McDonaldsMenuAnalysis/assets/86633487/8efc407a-b00e-48f6-a566-f697ba151c37)

**Insight for Consumers:**

**Insight for Company:**
