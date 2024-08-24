# Diabetes Dataset README

[Dataset Link](https://www.kaggle.com/datasets/mathchi/diabetes-data-set/data)

## Project Overview

This dataset contains information about female patients of Pima Indian heritage who are at least 21 years old. The dataset includes several health-related features and a binary outcome variable indicating whether the patient has diabetes or not.

## Dataset Description

- **Pregnancies**: Number of times the patient has been pregnant. Higher values may indicate a higher risk of gestational diabetes.
- **Glucose**: Plasma glucose concentration measured 2 hours after an oral glucose tolerance test (OGTT). Elevated levels may indicate diabetes.
- **BloodPressure**: Diastolic blood pressure, measured in millimeters of mercury (mm Hg). Normal range is typically below 80 mm Hg.
- **SkinThickness**: Triceps skinfold thickness, measured in millimeters (mm). Used to estimate body fat percentage and assess obesity risk.
- **Insulin**: 2-Hour serum insulin levels, measured in micro international units per milliliter (mu U/ml). Elevated levels may indicate insulin resistance, a precursor to type 2 diabetes.
- **BMI**: Body mass index, calculated as weight in kilograms divided by height in meters squared. Higher BMI values may indicate higher body fat levels and obesity, risk factors for diabetes.
- **DiabetesPedigreeFunction**: A measure of diabetes heredity, calculated based on family history. Higher values indicate a higher risk of diabetes.
- **Age**: Age of the patient in years. Older age is a risk factor for diabetes.
- **Outcome**: Indicates whether the patient has diabetes (1) or not (0). This is the target variable for predictive modeling.

## Additional Information

- **Oral Glucose Tolerance Test (OGTT)**: A diagnostic test to measure how well the body metabolizes glucose. It involves fasting overnight, then drinking a sugary solution and measuring blood glucose levels at intervals to assess diabetes risk.
- **Diastolic Blood Pressure (mm Hg)**: The pressure in the arteries when the heart is resting between beats.
- **Triceps Skin Fold Thickness (mm)**: A measure of subcutaneous fat thickness at the triceps skinfold site, commonly used in body fat assessment.

## Reference Ranges

- **Blood Pressure**: Normal range for diastolic blood pressure is typically below 80 mm Hg. Elevated levels may indicate hypertension, a risk factor for cardiovascular diseases.
- **Glucose**: Fasting blood glucose levels below 100 mg/dL are considered normal, while values above 126 mg/dL indicate diabetes.
- **Insulin**: Normal fasting insulin levels are typically between 2 and 25 μU/mL. Elevated levels may indicate insulin resistance, a precursor to type 2 diabetes.
- **BMI**: BMI values below 18.5 are considered underweight, 18.5 to 24.9 are normal, 25 to 29.9 are overweight, and 30 or above are obese.
- **Diabetes Pedigree Function**: There's no universally accepted normal range for this measure, but higher values indicate a higher risk of diabetes, especially when combined with other risk factors.

## Univariate Analysis

### Analysis of Pregnancies

- **Description**: Represents the number of times the patient has been pregnant. Higher values may indicate a higher risk of gestational diabetes.
- **Visualization**: Histogram and box plot.
- **Key Insights**:
  - Median value of Pregnancies is 3.
  - Most patients had 0, 1, or 2 pregnancies.
  - Patients had up to 17 pregnancies.
  - Outliers were observed in the box plot.

### Analysis of Glucose

- **Description**: Plasma glucose concentration measured 2 hours after an oral glucose tolerance test (OGTT). Elevated levels may indicate diabetes.
- **Visualization**: Histogram and box plot.
- **Key Insights**:
  - Median (117.0) and mean (120.8) of Glucose are close, indicating a symmetric distribution.
  - Some outliers are observed with a value of 0.
  - Explanation of OGTT needed.

### Analysis of BloodPressure

- **Description**: Diastolic blood pressure, measured in millimeters of mercury (mm Hg).
- **Visualization**: Histogram and box plot.
- **Key Insights**:
  - Median (72.0) and mean (69.1) of BloodPressure are close, indicating a symmetric distribution.
  - Some outliers are observed with a value of 0.
  - Explanation of diastolic blood pressure needed.

### Analysis of Insulin

- **Description**: 2-Hour serum insulin levels, measured in micro international units per milliliter (mu U/ml). Elevated levels may indicate insulin resistance, a precursor to type 2 diabetes.
- **Visualization**: Histogram and box plot.
- **Key Insights**:
  - The plots for Insulin are highly skewed.
  - The 0-value is the most for this feature.

### Analysis of BMI

- **Description**: Body mass index, calculated as weight in kilograms divided by height in meters squared. Higher BMI values may indicate higher body fat levels and obesity, risk factors for diabetes.
- **Visualization**: Histogram and box plot.
- **Key Insights**:
  - Median (32.0) and Mean (31.9) of BMI are close, indicating a symmetric distribution.
  - There are 11 rows with BMI value as 0, which is considered an outlier.

### Analysis of Diabetes Pedigree Function

- **Description**: A measure of diabetes heredity, calculated based on family history. Higher values indicate a higher risk of diabetes.
- **Visualization**: Histogram and box plot.
- **Key Insights**:
  - The histogram is highly skewed on the left side.
  - Many outliers are observed in the box plot.

### Analysis of Age

- **Description**: Age of the patient in years. Older age is a risk factor for diabetes.
- **Visualization**: Histogram and box plot.
- **Key Insights**:
  - The distribution of Age is skewed on the left side.
  - Some outliers are observed in the box plot for Age.

### Analysis of Outcome (Target Variable)

- **Description**: Indicates whether the patient has diabetes (1) or not (0).
- **Visualization**: Pie chart.
- **Key Insights**:
  - 65.1% patients in the dataset do NOT have diabetes.
  - 34.9% patients in the dataset have diabetes.

## Multivariate Analysis

### Analysis of Glucose and Outcome:

#### Visualization:

Histogram with hue based on Outcome.

#### Insights:

From the above plot, we observe a positive linear correlation between Glucose levels and the likelihood of diabetes. As Glucose levels increase, the number of patients with diabetes (Outcome = 1) also increases. Additionally, after a Glucose value of 125, there is a noticeable rise in the number of diabetic patients.

### Analysis of BloodPressure and Outcome:

#### Visualization:

Histogram with hue based on Outcome.

#### Insights:

The plot does not reveal a clear linear correlation between BloodPressure and the likelihood of diabetes (Outcome). There is no significant trend indicating that higher or lower BloodPressure values are associated with a specific Outcome.

### Analysis of BMI and Outcome:

#### Visualization:

Histogram with hue based on Outcome.

#### Insights:

A positive linear correlation is evident between BMI and the likelihood of diabetes. Higher BMI values tend to be associated with a higher proportion of diabetic patients.

### Analysis of Pregnancies and Outcome:

#### Visualization:

Histogram with hue based on Outcome.

#### Insights:

No significant linear correlation is observed between the number of pregnancies and the likelihood of diabetes.

### Analyzing Correlations:

#### Visualization:

Heatmap of the correlation matrix.

#### Insights:

The correlation matrix heatmap provides an overview of the relationships between different features. It shows the strength and direction of the correlations between each pair of features. Certain features may exhibit stronger correlations with the outcome variable (diabetes) compared to others.
