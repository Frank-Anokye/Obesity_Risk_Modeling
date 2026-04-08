# END-TO-END ML PROJECT: Predicting obesity risk to uncover key risk factors and population subgroups for actionable public health intervention

## Project Overview

Obesity is a global health crisis affecting over 600 million people worldwide. Traditional assessment requires clinical measurements, limiting access. This project applies machine learning models notably Random Forest, Decision Tree, and Logistic Regression through classification, regression, and clustering to predict obesity levels using **self-reported eating habits and physical activity**, enabling cost-effective, scalable approach to large-scale screening.



## Data Sources
The dataset include data for the estimation of obesity levels in individuals from the countries of Mexico, Peru and Colombia, based on their eating habits and physical condition. It contains **2,111 records** (real  and synthetic) with 16 features. Target variable: **NObeyesdad** (7 obesity levels).

| Category | Features |
|----------|----------|
| Demographic | Gender, Age, Height, Weight, family_history_with_overweight |
| Eating habits | FAVC (high-calorie food), FCVC (veg frequency), NCP (meals/day), CAEC (between meals), CH2O (water), CALC (alcohol) |
| Physical condition | SMOKE, SCC (calories monitoring), FAF (activity frequency), TUE (tech use), MTRANS (transportation) |

**source:** [UC IRVINE MACHINE LEARNING REPOSITORY](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition)

---

## Tools & Libraries

- **Jupyter Notebook** – programming language  
- **pandas, numpy** – data manipulation  
- **matplotlib, seaborn** – visualization  
- **scikit-learn** – preprocessing, modeling, and evaluation  

---


## Data Cleaning & Preprocessing

- No missing values – dataset was complete.  
- Duplicates removed (Number of duplicate rows: 24).  
- Categorical variables label-encoded.  
- Created continuous BMI feature for regression.  
- Train-test split: 70/30 with stratification for classification.

## EXPLORATORY DATA ANALYSIS (EDA)

### Target Distribution
The data is relatively balanced, however, obesity level (Insufficient_Weight) has the fewer samples

![Target Distribution](images/target_distribution)
