#Lab6
# 📈 Linear Regression Lab: Housing Prices & E-commerce Customers

This repository contains the code and analysis for a Machine Learning lab (ARTI308) focused on implementing **Linear Regression**. The project is divided into two parts, applying predictive modeling to two distinct industries: Real Estate and E-commerce.

##  Project Overview

The goal of this project is to build machine learning models that can predict continuous target variables based on various features. 
1. **Part 1 (USA Housing):** Helping a real estate agent predict house prices based on regional features.
2. **Part 2 (E-commerce):** Helping an online business decide whether to focus their efforts on their mobile app experience or their website by predicting customer yearly spend.

##  Technologies & Libraries Used

* **Python 3**
* **Jupyter Notebook**
* **Pandas** (Data manipulation and analysis)
* **NumPy** (Numerical operations)
* **Matplotlib & Seaborn** (Data visualization)
* **Scikit-Learn** (Machine Learning model building and evaluation)

##  Datasets

### 1. USA Housing Dataset (`USA_Housing.csv`)
Contains information about houses in various regions of the United States.
* **Features:** Avg. Area Income, Avg. Area House Age, Avg. Area Number of Rooms, Avg. Area Number of Bedrooms, Area Population.
* **Target Variable:** Price (The price the house sold at).

### 2. E-commerce Customers Dataset (`Ecommerce Customers`)
Contains customer data from an online clothing store that offers both in-store style advice sessions and online platforms (App and Website).
* **Features:** Avg. Session Length, Time on App, Time on Website, Length of Membership.
* **Target Variable:** Yearly Amount Spent.

##  Project Workflow

1. **Data Loading & Exploration:** Importing the datasets, checking data types, and exploring basic statistical summaries (`head()`, `info()`, `describe()`).
2. **Exploratory Data Analysis (EDA):** Visualizing data distributions and relationships between variables using Seaborn.
3. **Data Preparation:** Splitting the data into feature variables (`X`) and target variables (`y`), and using `train_test_split` to create training and testing sets.
4. **Model Training:** Initializing and fitting a `LinearRegression` model from Scikit-Learn.
5. **Model Evaluation:** Interpreting model coefficients and calculating regression evaluation metrics (MAE, MSE, RMSE).

##  Key Insights & Results

### E-commerce Customer Analysis
Based on the Linear Regression coefficients, we discovered how different customer behaviors impact their yearly spend:
* **Length of Membership** is the most significant factor. For every 1 unit increase in Length of Membership, the Yearly Amount Spent increases by **~$61.28**.
* **Time on App** is significantly more profitable than **Time on Website**. A 1 unit increase in Time on App results in an increase of **~$38.59** spent, whereas a 1 unit increase in Time on Website only results in a **~$0.19** increase.
* **Business Recommendation:** The company should either focus on further developing their Mobile App (since it is already working well and driving sales) or overhaul their Website to catch up to the App's performance. Fostering customer loyalty (Length of Membership) should also be a top priority.

##  How to Run the Code

1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
