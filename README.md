# Exploratory Data Analysis on Insurance Spending Dataset

## Overview

This project focuses on performing **Exploratory Data Analysis (EDA)** and implementing a **Simple Linear Regression** model to predict insurance charges using the `insurance.csv` dataset. The dataset contains information about individuals' age, BMI, children, region, and their medical charges. The goal is to explore the data visually and use a linear regression model to predict insurance charges based on the individual's BMI.

## Prerequisites

Ensure you have the required dependencies installed:

- **Python ≥ 3.5**
- **Scikit-Learn ≥ 0.20**
- **pandas**
- **numpy**
- **matplotlib**
- **seaborn**

You can install the necessary packages using `pip`:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
## Data Description

The dataset contains several features:

- **age**: The age of the individual.
- **sex**: Gender of the individual.
- **bmi**: Body Mass Index (BMI).
- **children**: Number of children/dependents covered by the insurance.
- **smoker**: Whether the individual is a smoker.
- **region**: The region where the individual resides.
- **charges**: The medical charges (target variable).

## Steps

### 1. Load the Data

The dataset is loaded into a Pandas DataFrame to begin analysis.

### 2. Exploratory Data Analysis (EDA)

The first step in understanding the dataset is visualizing the data to identify any patterns or relationships between features.

- Scatter plots are used to show the relationships between variables such as age and BMI.
- Histograms are plotted to understand the distributions of numerical features like charges and BMI.
- Pairwise plots (scatter matrix) are created to observe how multiple features correlate with one another, particularly focusing on age, BMI, children, and charges.

### 3. Data Preprocessing

The data is split into **training** and **testing** sets to ensure the model is evaluated on unseen data. This is done by randomly splitting the data into two parts, typically using 85% for training and 15% for testing.

### 4. Linear Regression Model

- A simple **linear regression** model is chosen to predict insurance charges based on BMI. 
- The model is trained using the training data, where the BMI of individuals is used as the feature (independent variable) and charges as the target (dependent variable).
- After training, predictions are made on the test data to evaluate the model’s performance.

### 5. Model Evaluation

- The model’s performance is evaluated using the **R-squared value**, which indicates how well the model explains the variance in the target variable (charges).
- A regression line is plotted on a scatter plot of the training data to visually assess how well the model fits the data.

### 6. Conclusion

The project demonstrates the use of linear regression to predict insurance charges. By performing exploratory data analysis and training a simple linear regression model, we gain insights into the relationship between BMI and insurance charges. The performance of the model is evaluated, and predictions are made to assess its effectiveness.

## Files

- `insurance.csv`: The dataset used for analysis.
- `InsuranceSpendingAnalysis.ipynb`: Jupyter notebook containing the EDA and linear regression steps.

## License

This project is licensed under the MIT License.

---

Feel free to explore and extend the analysis or apply similar techniques to other datasets!
