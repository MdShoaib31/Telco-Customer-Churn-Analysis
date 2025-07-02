# Telco Churn Analysis
## Project Overview
This project focuses on analyzing a telecommunications customer dataset to understand the factors contributing to customer churn. By exploring various demographic, service, and billing attributes, this analysis aims to identify patterns and insights that can help predict and mitigate customer churn. The insights gained can be valuable for developing targeted retention strategies.

## Table of Contents
- Project Overview
- Dataset
- Analysis Goals
- Key Features & Preprocessing
- Exploratory Data Analysis (EDA) & Visualizations
- Technologies Used

## Dataset
The analysis uses the customer ```churn.csv dataset```, which contains information on a telecommunications company's customers. Each row represents a unique customer, and columns contain various attributes, including:
Demographic Information: ```gender```, ```SeniorCitizen```, ```Partner```, ```Dependents```
Service Information: ```PhoneService```, ```MultipleLines```, ```InternetService```, ```OnlineSecurity```, ```OnlineBackup```, ```DeviceProtection```, ```TechSupport```, ```StreamingTV```, ```StreamingMovies```
Account Information: ```tenure```, ```Contract```, ```PaperlessBilling```, ```PaymentMethod```, ```MonthlyCharges```, ```TotalCharges```
Target Variable: **Churn** (indicating whether the customer churned or not)
The dataset comprises 7043 customer entries and 21 features.

## Analysis Goals
The primary goals of this analysis are to:

- Understand the distribution and characteristics of the customer base.
- Identify key features and factors that are strongly correlated with customer churn.
- Visualize relationships between various attributes and churn.
- Provide actionable insights that can inform customer retention strategies.

## Key Features & Preprocessing
The notebook includes essential data preprocessing steps to ensure data quality and prepare it for analysis:

**Data Loading & Initial Inspection:**

  - Loading the customer churn.csv into a pandas DataFrame.
  - Initial checks using ```df.head()```, ```df.info()```, and ```df.describe()``` to understand data types, non-null counts, and statistical summaries.
  - Confirmation of no duplicate ```customerID``` values.

**Handling TotalCharges:**
  - The ```TotalCharges``` column, initially an object type, contained blank values (" ") for new customers. These blanks were replaced with "0".
  - The column was then successfully converted to a float data type to enable numerical computations.

**Converting SeniorCitizen:**
  - The ```SeniorCitizen``` column, originally numerical (0 or 1), was transformed into more readable categorical labels ("No" and "Yes") for better interpretability during analysis and visualization.

## Exploratory Data Analysis (EDA) & Visualizations
The project leverages matplotlib.pyplot and seaborn to perform comprehensive Exploratory Data Analysis. While the specific visualizations are within the Jupyter Notebook (Telco Churn Analysis.ipynb), they are designed to reveal:

  - **Distribution of Churn:** Understanding the overall churn rate within the dataset.
  - **Demographic Impact:** How gender, SeniorCitizen status, Partner status, and Dependents relate to churn.
  - **Service Impact:** The influence of various services like PhoneService, InternetService (and its sub-services), and MultipleLines on churn.
  - **Contract and Billing Impact:** The relationship between Contract type, PaperlessBilling, and PaymentMethod with churn.
  - **Numerical Feature Analysis:** Distribution of tenure, MonthlyCharges, and TotalCharges in relation to churn, likely using histograms, box plots, or violin plots.

(Self-correction/Improvement: If you add specific charts later, you can expand this section, e.g., "Visualizations include: count plots for categorical variables showing churn distribution, histograms for numerical variables, and possibly correlation heatmaps.")



## Technologies Used -
- Python 3.x
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn

## THANK YOU!
