Toyota Cars - Data Preprocessing

**Overview**

Data preprocessing pipeline for Toyota car dataset following structured lab exercises.



**Dataset: toyota\_cars.xlsx**

Contains Toyota car models with specs (price, engine, seats, dimensions, etc.)



**Tasks Completed**

Task 1: Data Quality Assessment

Checked data types



Converted price, engine\_displacement, seats to numeric



Task 2: Missing Values

Applied Median Imputation to 'seats' column



Why: Robust to outliers, preserves data size



Task 3: Outlier Detection (IQR)

Visualized price with boxplot



Calculated Q1, Q3, IQR



Removed price outliers



Task 4: Normalization

Min-Max Scaling (range 0-1)



Z-score Standardization (mean=0, std=1)



Task 5: PCA

Reduced 3 features to 2 components



Analyzed explained variance ratio



Visualized PCA projection



**Libraries**

pandas numpy matplotlib seaborn scikit-learn



**Output**

Clean, normalized dataset ready for machine learning models.

