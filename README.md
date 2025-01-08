# Blinkit-analysis
**Project Overview**
This project presents a comprehensive Power BI dashboard for analyzing Blinkit's sales performance, customer satisfaction, and inventory distribution. The dashboard provides key insights and opportunities for optimization using various KPIs and visualizations.

**Dataset Features:**
*Item_Fat_Content:*
Represents the fat content of the item (e.g., low fat, regular). This is typically a categorical variable.

*Item_Visibility:*
Represents how visible the item is on the shelf. It is a numerical variable, likely a percentage or ratio.

*Item_Type:*
Describes the type or category of the item (e.g., dairy, beverages, snacks). This is a categorical variable.

*Item_MRP:*
Maximum Retail Price of the item. This is a continuous numerical variable.

*Outlet_Establishment_Year:*
The year when the outlet was established. This is a numerical variable, often transformed into the outlet age by subtracting it from the current year.

Outlet_Location_Type:
Describes the type of location of the outlet (e.g., Tier 1, Tier 2, Tier 3 cities). This is a categorical variable.

*Outlet_Type:*
Indicates the type of outlet (e.g., grocery store, supermarket type1, supermarket type2). This is a categorical variable.

*Item_Outlet_Sales:*
The target variable representing the total sales of the product at a particular outlet. It is a continuous variable.

**Models Trained:**

**1. Linear Regression**

*Purpose:* Predict the continuous target variable, Outlet_Location_Type.
Use Case:
Linear regression is ideal for predicting the total sales based on numerical and categorical features (encoded appropriately).

Process:
*Preprocessing:* Handling missing values, encoding categorical variables, scaling numerical variables.

*Training:* A linear relationship is assumed between the features and sales.

*Advantages:*
Simple and interpretable model.
Good baseline for regression tasks.

*Limitations:*

Assumes linearity in data.
Sensitive to multicollinearity and outliers.

**2. Logistic Regression**
   
*Purpose:* Predict a categorical outcome (e.g., binary classification based on sales levels: high/low).

Use Case:
Logistic regression is used when the task involves classifying sales into categories rather than predicting exact values.

*Process:*
*Preprocessing:* Similar steps to linear regression.

*Training:* Uses the logistic function to model the probability of an observation belonging to a particular category.

*Advantages:*
Works well with categorical data.
Provides probabilistic outputs for decision-making.

*Limitations:*
Assumes a linear relationship between features and the log-odds of the target variable.

**3. Decision Tree**

*Purpose:* Predict both continuous (Item_Outlet_Sales) and categorical outcomes.
Use Case:
Decision trees can handle both regression and classification tasks, making them versatile for this dataset.

Process:
*Preprocessing:* Minimal preprocessing needed (e.g., encoding categorical variables).

*Training:* Splits data based on feature thresholds to minimize prediction error (e.g., Gini impurity, entropy for classification, or mean squared error for regression).

*Advantages:*
Handles non-linear relationships effectively.
Easy to interpret and visualize.
No need for feature scaling or encoding.

*Limitations:*
Prone to overfitting, especially with deep trees.
Sensitive to small variations in the data.

**Key Performance Indicators (KPIs)**
The dashboard focuses on the following primary KPIs:

**Total Sale**s: Overall revenue generated from all items sold ($1.20M)	

**Average Sales**: Average revenue per sale ($141)

**Number of Items**: Total count of different items sold (8523)

**Average Rating**: Average customer rating for items sold (3.9 out of 5)

**Features**

**Filter Panel**: Allows users to filter data by outlet location type, outlet size, and item type.

**Outlet Establishment Trend**: Visualizes the growth of outlet establishments from 2012 to 2022.

**Fat Content Analysis**: Breaks down sales by low fat and regular fat products.

**Item Type Distribution**: Shows sales distribution across various product categories.

**Outlet Size and Location Analysis**: Provides insights on sales performance by outlet size and location tier.

**Outlet Type Comparison**: Compares different outlet types based on sales, number of items, average sales, ratings, and item visibility.


**Insights and Conclusions**

Strong overall sales performance with over $1M in total sales.
Consumer preference for low-fat products, indicating health-conscious buying habits.
Fruits, vegetables, and snack foods are the top-selling categories.
Medium-sized outlets in Tier 3 locations show the highest profitability.
Supermarkets generate higher sales volumes, while grocery stores have better item visibility
