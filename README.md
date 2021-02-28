# CAPSTONE PROJECT
This project is an analysis of the cannabis quality to find the factors that affect the most in the “best” plants.

## Exploratory Analysis
- Contains 10 variables, 9 independent and 1 dependent (Quality)
- Contains 5 Multiclass variables
- Has 1472 rows and null values

## Cleaning
- Around 9% of Null values were filled with mean to eliminate variability
- Around 40% of outliers rows were eliminated
- A high correlation between Bmch_Fm and Crown_Fm and Ht and DBH
- Change from 5 Multiclass to a Binomial, being “best” vs “others” and balance it

## Analysis
- Three models tested for their efficiency and simplicity
- Logistic Regression, Linear Discriminant Analysis (LDA) and Quadratic Discriminant Analysis (QDA).
  - Dataset divided into: Training 80% and Testing 20%.
  - Metrics: Recall 90% and AUC 0.9.
- Validation was done with Classification Matrix and AUC Curve.

## Results
- Data quality is not the best as there was a lot of preprocessing.
- LDA is the most accurate model considering the suggested metrics with:
  - NestedCV Recall (weighted): 0.88 +/-0.02
  - AUC: 0.82
- The target was not achieved in any of the metrics.

## Recommendations
- The main factors affecting the quality are Vig, Crown_Fm and PmCno
- Take another more balanced dataset
- Get a more balanced dataset that contains Binomial classes
