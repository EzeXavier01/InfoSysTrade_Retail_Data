# InfoSysTrade_Retail_Data

## Tableau Visualization
To access my Tableau visualization, please click on this [Link](https://public.tableau.com/app/profile/ifeanyi.eze3640/viz/RetailDashboard_17428850803440/Dashboard1?publish=yes).

## Project Overview
This project focuses on analyzing retail transaction data to uncover patterns, trends, and insights that can drive business decisions. The dataset was preprocessed, explored, and used to develop predictive models for classification tasks.

## Installation
To install the necessary libraries for this project, run the following command:

```bash
pip install numpy matplotlib seaborn pandas scikit-learn xgboost statsmodels
```

Alternatively, you can install them manually:

```python
# Importing the necessary libraries
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
from sklearn.preprocessing import LabelEncoder, StandardScaler, OneHotEncoder
from sklearn.model_selection import train_test_split, cross_val_score
from sklearn.ensemble import RandomForestClassifier, GradientBoostingClassifier
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score, classification_report
from xgboost import XGBClassifier
from statsmodels.tsa.holtwinters import ExponentialSmoothing
```

## Exploratory Data Analysis (EDA)
### **Data Preprocessing Summary**  

#### **Handling Duplicates**  
Duplicate records were identified and removed to maintain data integrity. One duplicate transaction was detected and eliminated to prevent redundancy.

#### **Handling Missing Values**  
A small number of missing values were found across multiple columns. Since they were randomly distributed and had a low occurrence, they were removed to avoid biasing the analysis.

#### **Feature Engineering**  
- **Date Conversion**: Transformed the `Date` column into `datetime` format for better time-series analysis.
- **Month Extraction**: Created a new `Month` column to analyze seasonal purchasing trends.

These steps ensured a clean and structured dataset, ready for deeper analysis and predictive modeling.

## Predictive Modeling
Several machine learning models were trained to predict customer purchasing behavior. The models used include:
- **Random Forest Classifier**
- **Gradient Boosting Classifier**
- **Logistic Regression**
- **XGBoost Classifier**

Performance metrics such as accuracy, precision, recall, and F1-score were used to evaluate model effectiveness.

## Business Insights & Visualization
The project also includes a business insights analysis file (`Retail_data`), where key findings from the data are documented.


