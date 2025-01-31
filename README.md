# Python-Project-Health-analysis-

## Overview
This project focuses on cleaning, transforming, and analyzing health-related data from a dataset. The goal is to preprocess the data, handle missing values, remove outliers, and prepare it for further analysis and modeling. The cleaned data is used to generate various visualizations and statistical models.

### Technologies Used
Python: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

### Steps Involved
**Data Cleaning**:

Dropped columns with irrelevant data (e.g., SYMBOL, TERMINATED).
Removed rows with missing values in the key column 'VALUE'.
Filled missing 'STATUS' and 'DGUID' values with placeholders.
Renamed columns for better clarity and consistency.
Removed duplicate values and inconsistent entries like 'Unknown', 'N/A'.

**Handling Missing Values**:

Replaced missing numerical values with the median of the respective columns.
Replaced missing categorical values with the mode of the respective columns.
Dropped rows with 'Unknown' or 'UNK' entries.
Standardized categorical values (e.g., converted to lowercase).

**Outlier Detection and Removal**:

Applied log transformation and scaling to handle skewness and standardize values.
Used the IQR method to identify and remove outliers in the 'VALUE' column.

**Exploratory Data Analysis (EDA)**:

Visualized the distribution of data using box plots and histograms.
Created correlation heatmaps to explore relationships between numerical features.
Used various plotting techniques to understand how 'VALUE' varies across different categories like Age, Gender, and Indicators.

**Data Preprocessing for Modeling**:

Converted categorical data into numerical codes.
Applied feature scaling for machine learning models.
Split the data into training and testing sets for model evaluation.

**Modeling**:

Trained and evaluated a Linear Regression model and a Random Forest Regressor to predict the 'VALUE' column.
Used metrics like Mean Squared Error (MSE) and R-squared to assess model performance.
Performed clustering using K-means to segment the data based on relevant features.

**Final Output**:

Saved the cleaned data to a CSV file (health_data_final_cleaned.csv).
Generated insights through visualizations and machine learning models.

## Conclusion
This project demonstrates how to handle raw health data, clean it, perform exploratory analysis, and apply basic machine learning techniques to gain insights. The cleaned data and visualizations provide valuable information for health-related decision-making.
