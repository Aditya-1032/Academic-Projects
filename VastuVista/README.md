# वास्तुविस्ता (VastuVista)
## Future Prospects in Real Estate Price Modelling

## Project Overview

VastuVista is an academic project focused on exploring real estate price modelling using Bengaluru housing data. The project investigates the application of statistical techniques and machine learning algorithms to understand property price patterns and develop predictive models.

The study involves exploratory data analysis, data preprocessing, feature engineering, multicollinearity analysis and regression modelling to evaluate different approaches to house price prediction.

## Project Objectives

- Explore and understand factors influencing residential property prices.
- Perform exploratory data analysis to identify patterns and relationships within the dataset.
- Clean and preprocess the housing data for modelling.
- Apply feature engineering and outlier treatment techniques.
- Examine multicollinearity among explanatory variables using Variance Inflation Factor (VIF).
- Develop and compare different regression models for property price prediction.

## Dataset

**Dataset:** Bengaluru House Price Data  
**Source:** Kaggle  
**Original Dataset Size:** 13,320 observations  
**Original Variables:** 9

The dataset contains information about residential properties in Bengaluru.

### Key Variables

| Variable | Description |
|---|---|
| Area Type | Classification of the property area |
| Availability | Property availability status |
| Location | Property location |
| Size | Property size, generally expressed in BHK |
| Society | Residential society name |
| Total Sqft | Total property area |
| Bath | Number of bathrooms |
| Balcony | Number of balconies |
| Price | Property price in lakhs |

## Methodology

### 1. Data Cleaning and Preprocessing
- Examined missing values and inconsistent entries.
- Processed property size and total square footage.
- Handled missing and irregular values.
- Prepared categorical and numerical variables for analysis.

### 2. Exploratory Data Analysis (EDA)
- Analysed distributions of property prices and other variables.
- Examined relationships between property characteristics and prices.
- Identified patterns and potential outliers.

### 3. Feature Engineering
- Extracted useful information from existing variables.
- Created additional features for analysis and modelling.
- Applied categorical encoding techniques.

### 4. Multicollinearity Analysis
- Used Variance Inflation Factor (VIF) to examine multicollinearity among selected explanatory variables.

### 5. Model Development
The following regression techniques were implemented and evaluated:

- Linear Regression
- Ridge Regression
- Support Vector Regression (SVR)

Different SVR kernel functions were explored to compare model performance.

## Model Performance

The following results were reported in the original project presentation:

| Model | R² Score | RMSE |
|---|---:|---:|
| Linear Regression | 86.02% | 37.23 |
| Ridge Regression | 86.02% | 37.23 |
| SVR (Linear Kernel) | 81.13% | 43.27 |
| SVR (RBF Kernel) | 87.16% | 35.69 |
| SVR (Sigmoid Kernel) | 77.97% | 46.75 |

**Best Reported Model:** Support Vector Regression with RBF Kernel.

The RBF kernel achieved the highest reported R² score and the lowest RMSE among the evaluated models.

*Note: These are the results reported in the original academic presentation. They have not been independently reproduced or validated here.*

## Technologies and Libraries

- **Programming Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Data Visualisation:** Matplotlib
- **Machine Learning:** Scikit-learn
- **Development Environment:** Jupyter Notebook

## Repository Structure

```text
VastuVista/
│
├── dataset/
│   └── Bengaluru_House_Data.csv
│
├── notebooks/
│   └── Final_RR.ipynb
│
├── presentation/
│   ├── VastuVista.pdf
│   └── VastuVista.pptx
│
└── README.md
```

## Limitations

- The analysis is based on a historical Bengaluru housing dataset.
- The model results depend on the preprocessing and modelling choices used in the original study.
- The original modelling workflow includes a price-per-square-foot feature derived from the target variable (price). Using this feature to predict price introduces target leakage and can inflate performance estimates.
- The reported model performance should therefore not be interpreted as evidence of generalisation to unseen real estate markets.

## Conclusion

VastuVista provided an opportunity to explore statistical analysis and machine learning applications in real estate price modelling. By applying exploratory data analysis, feature engineering, multicollinearity assessment and regression techniques, the project compared different approaches to understanding and predicting residential property prices.

The project strengthened practical understanding of statistical modelling, data preprocessing and machine learning evaluation.

---

**Project Type:** Master's Academic Project  
**Domain:** Statistics | Real Estate Analytics | Machine Learning  
**Dataset Location:** Kaggle – Bengaluru House Price Data
