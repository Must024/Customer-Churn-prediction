#  Customer Churn Prediction – Subscription-Based Business

##  Overview
Customer churn is one of the biggest challenges for subscription-based businesses. This project analyzes Telco customer data to identify factors that influence churn and predict customers who are most likely to leave.  
Using machine learning models (Logistic Regression, Random Forest, XGBoost), I built a predictive pipeline and explained the results with SHAP values to give actionable retention strategies.

---

##  Business Problem
Losing customers is costly, acquiring a new customer can be up to **5x more expensive** than retaining an existing one.  
This project answers two key questions:
1. **Which customers are most likely to churn?**
2. **What are the key factors driving churn?**

---

##  Project Structure
```
customer-churn-prediction/
│
├── notebooks/
│   └── Customer_Churn_Analysis.ipynb
├── slides/
│   └── Customer_Churn_Presentation.pdf
├── images/
│   ├── churn_distribution.png
│   ├── contract_type_churn.png
│   ├── shap_summary.png
│   └── model_comparison.png
├── requirements.txt
└── README.md
```

---

##  Data Source
- **Dataset:** [Telco Customer Churn – Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Rows:** 7,043  
- **Columns:** 21  
- **Features:** Demographics, account info, service usage, and charges.

---

## ️ Process
1. **Data Cleaning** – Handled missing values, corrected data types, encoded categorical variables.
2. **Exploratory Data Analysis (EDA)** – Visualized churn patterns by tenure, contract type, and monthly charges.
3. **Modeling** – Built and compared Logistic Regression, Random Forest, and XGBoost models.
4. **Model Interpretation** – Used SHAP values to explain model predictions.
5. **Recommendations** – Developed data-driven retention strategies.

---

##  Model Performance
| Model               | Accuracy | Precision | Recall | F1-score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | 78.68%   | 0.619     | 0.513  | 0.561    |
| Random Forest       | 78.53%   | **0.632** | 0.460  | 0.533    |
| XGBoost             | 73.70%   | 0.504     | **0.676** | **0.578** |

**Best Model:**  
- For overall **balanced performance** → **Logistic Regression**  
- For **high recall (catching more churners)** → **XGBoost**  
- For **highest precision** → **Random Forest**

---

##  Key Visuals

### Churn Distribution
![Churn Distribution](images/churn_distribution.png)

### Churn by Contract Type
![Contract Type vs Churn](images/contract_type_churn.png)

### Model Comparison
![Model Comparison](images/model_comparison.png)

### SHAP Summary Plot
![SHAP Summary Plot](images/shap_summary.png)

---

##  Key Insights from SHAP
- **Contract type** is the strongest churn driver — month-to-month customers are far more likely to churn.
- **Fiber optic internet service** customers churn more than DSL users.
- **Tenure** is negatively correlated with churn — long-term customers are more loyal.
- **Online security & tech support** lower churn probability.
- **Electronic check payment method** is linked to higher churn.

---

##  Recommendations
- **Promote long-term contracts** with incentives.
- **Target new customers early** (first 6 months) with retention campaigns.
- **Offer discounts or bundles** to high-bill customers.
- **Encourage switching to automatic payment** instead of electronic checks.
- **Bundle services** like online security and tech support to increase customer stickiness.

---

##  Deliverables
-  **Notebook:** [Customer Churn Analysis]([notebooks/Customer_Churn_Analysis.ipynb](https://github.com/Must024/Customer-Churn-prediction/blob/main/Customer%20Churn%20Analysis%20for%20a%20Subscription-Based%20Business%20(2).ipynb))  
-  **Slides (PDF):** [Customer Churn Presentation](slides/Customer_Churn_Presentation.pdf)  
- ️ **SHAP Summary Plot:** ![SHAP](images/shap_summary.png)

---

## ️ Tools & Libraries
- Python: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, `shap`
- Jupyter Notebook
- Google Slides (presentation)
- GitHub (version control & portfolio hosting)

---

##  Author
**Gafar Mustopha** – Data Analyst  
 [LinkedIn](www.linkedin.com/in/mustopha-gafar-6207a6325) |  [GitHub](https://github.com/) | [Email](Mustopha024@Gmail.com)
