Project Overview

The primary goal of this lab is to prepare the global_cars_enhanced dataset for further analysis or machine learning. The dataset includes features such as engine size, horsepower, mileage, and price, with Efficiency_Score as the target numerical variable.
Tasks Covered
1. Data Quality Assessment
•Initial Inspection: Loaded the dataset and identified that the first row contained column headers incorrectly placed as data.
• Cleaning: Re-assigned the first row as column names and dropped the redundant row to ensure proper alignment.
• Integrity Check: Checked for missing values and duplicates across the 301 entries.
2. Missing Value Imputation
• Strategy: Implemented a Median Imputation strategy for the Price_USD column.
• Justification: The median was selected because it is more robust to potential outliers in car pricing compared to the mean, which can be skewed by luxury or economy extremes.
3. Outlier Detection
• Method: Utilized the Interquartile Range (IQR) method on the Price_USD column.
• Result: No outliers were detected, suggesting a relatively stable price distribution within the provided sample.
4. Feature Scaling (Normalization)
• Min-Max Scaling: Applied MinMaxScaler to Price_USD and Horsepower to transform values into a range between 0 and 1. This ensures that different units (dollars vs. HP) do not disproportionately influence analysis.
5. Dimensionality Reduction (PCA)
• Standardization: Performed Z-score standardization using StandardScaler as a prerequisite for PCA.
• Principal Component Analysis: Applied PCA to reduce the complexity of the dataset while retaining maximum variance.
• Variance Interpretation: The explained variance ratio was calculated to determine how much information each principal component captures (e.g., PC1 captured approximately 55% of the variance).
Requirements

To run this notebook, you will need the following Python libraries:
• pandas
• numpy
• matplotlib
• seaborn
• scikit-learn

Dataset

The analysis requires the global_cars_enhanced.xlsx file to be present in the same directory as the notebook.
