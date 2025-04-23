# BA_Bootcamp_9_RandomForest_Challenge

# Random Forest Challenge


# 🌲 Random Forest Challenge – Predicting Customer Income

Welcome to the **Random Forest Challenge**! This project aims to predict customer income using a Random Forest Regression model. Leveraging customer behavior, demographics, and purchasing patterns, we train a model to uncover what makes a customer *wealthy*—a crucial insight for marketing, targeting, and business decision-making.

## 🚀 Challenge Overview

**"Figuring out who the wealthy customers are is every company’s dream."**

This challenge walks through an end-to-end predictive modeling project using a marketing dataset, following these main steps:

1. **🧹 Data Preparation**  
2. **🌲 Random Forest Modeling**  
3. **📊 Accuracy Assessment**  
4. **🛠️ Model Tuning**  
5. **💡 Generating Insights with Explainable AI**

---

## 🧠 Problem Statement

**Goal:** Predict customer income using various behavioral and demographic indicators.

Understanding customer income helps businesses segment users effectively, personalize campaigns, and drive smarter decision-making—especially when identifying high-value individuals, or *whales*, who are less price-sensitive.

---

## 📂 Dataset & Attributes

Dataset: [`marketing_campaign.csv`](./marketing_campaign.csv)  
More info: [`Customer_s income.docx`](./Customer_s%20income.docx)

The dataset includes attributes across:
- **People** (Age, Education, Marital Status)
- **Products** (Amount spent on Wine, Meat, Gold, etc.)
- **Promotion Response** (Accepted Campaigns, Complaints)
- **Channel Usage** (Web, Catalog, Store Purchases)

---

## 📈 Model & Key Findings

### ✅ Model Type
- **Random Forest Regressor** — since income is a **continuous variable**

### 🔍 Accuracy Assessment
- **Mean Absolute Error (MAE):** `~6543`
- **Mean Income:** `~50,734`  
- **Std Dev of Income:** `~22,074`

This suggests the model does a reasonable job predicting income, with an average error of ~13% of the mean income.

### 🌟 Top 5 Features Influencing Income

    1. MntWines (~33.2%)
    
    2. MntMeatProducts (~24.2%)
    
    3. MntFruits (~8.5%)
    
    4. NumWebVisitsMonth (~7.3%)
    
    5. NumDealsPurchases (~6.6%)

#

        ✅ Spending habits—especially on **wines and meats**—are strong predictors of income.
        
        ---
        
        ## 🔧 Parameter Tuning
        
        A grid search across `n_estimators` was conducted to minimize MAE.  
        **Best Parameter:**  
        ```python
        {'n_estimators': 50}

    --> This shows that fewer trees in this case led to better generalization—possibly due to reduced overfitting.




## 📌 Repository Structure

📁 Random Forest Challenge

├── marketing_campaign.csv             # Dataset

├── Random Forest Challenge.ipynb      # Complete analysis in Python

├── Random Forest Challenge.pdf        # Challenge overview & tasks

├── Customer_s income.docx             # Variable descriptions

└── README.md                          # You’re here!



## 📊 Key Takeaways

    * Random Forests are powerful for handling feature-rich data with minimal preprocessing.
    
    * Customer spending behaviors are powerful proxies for estimating income.
    
    * Tuning even a single parameter like n_estimators can meaningfully improve performance.
    
    * XAI techniques like feature importance provide clarity on the black-box nature of ensemble models.


## 🤝 Let's Connect

    --> If you found this project insightful or want to collaborate, feel free to reach out or connect on LinkedIn!


⭐ Don’t forget to give this repository a star if you like it!



    
