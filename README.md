BREAST CANCER PREDICTION USING SNOWFLAKE SCHEMA AND K-NEAREST NEIGHBORS
====================================================================

PROJECT OVERVIEW
----------------
This project focuses on breast cancer diagnosis using the K-Nearest Neighbors (KNN)
algorithm applied to the Breast Cancer dataset. The dataset is structured using a
Snowflake Schema to demonstrate normalized data warehousing concepts along with
instance-based machine learning classification.

The project highlights how distance-based classification can be applied to structured
medical data stored in a Snowflake Schema.


PROBLEM STATEMENT
-----------------
Breast cancer diagnosis requires accurate classification of tumors as malignant or
benign based on multiple numerical features. Traditional diagnosis methods may be
subjective and time-consuming.

This project aims to:
- Organize breast cancer data using a Snowflake Schema
- Apply K-Nearest Neighbors for classification
- Evaluate model performance using standard metrics


DATASET
-------
Dataset Used:
- Breast Cancer Wisconsin Dataset

Target Variable:
- Diagnosis (Malignant / Benign)

Features:
- Tumor measurements such as radius, texture, perimeter, area, smoothness, etc.

Data Representation:
- Fact table stores measurement records
- Dimension tables store normalized attribute details
- Snowflake Schema is used to reduce redundancy


TECHNOLOGIES USED
-----------------
- Python
- Pandas
- NumPy
- Scikit-learn
- SQL (for Snowflake Schema modeling)


SNOWFLAKE SCHEMA DESIGN
----------------------
- Fact Table:
  - Record_ID
  - Feature values
  - Diagnosis_ID

- Dimension Tables:
  - Patient Dimension
  - Feature Dimension
  - Diagnosis Dimension

Purpose:
- Normalized data storage
- Improved data integrity
- Demonstration of data warehousing principles


ALGORITHM USED
--------------
K-Nearest Neighbors (KNN)

Description:
KNN is a distance-based, non-parametric algorithm that classifies data points based on
the majority class of the nearest neighbors in the feature space.

Key Characteristics:
- No explicit training phase
- Classification based on distance metrics (Euclidean distance)
- Performance depends on choice of K and feature scaling


IMPLEMENTATION STEPS
--------------------
1. Load the Breast Cancer dataset
2. Clean and preprocess the data
3. Normalize feature values
4. Design Snowflake Schema tables
5. Split data into training and testing sets
6. Select optimal value of K
7. Apply KNN classification
8. Evaluate model performance


EVALUATION METRICS
------------------
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix


RESULTS
-------
- KNN achieves competitive accuracy on the Breast Cancer dataset
- Model performance is sensitive to feature scaling
- Snowflake Schema improves data organization but does not directly impact accuracy


ADVANTAGES
----------
- Simple and intuitive algorithm
- No assumption about data distribution
- Effective for well-separated classes
- Easy to implement


LIMITATIONS
-----------
- High memory usage
- Slower prediction time for large datasets
- Sensitive to noise and irrelevant features
- Choice of K significantly affects results


FUTURE ENHANCEMENTS
-------------------
- Hyperparameter tuning for optimal K
- Comparison with Logistic Regression and SVM
- Dimensionality reduction using PCA
- Deployment using a web-based interface


CONCLUSION
----------
This project demonstrates effective breast cancer classification using the K-Nearest
Neighbors algorithm combined with Snowflake Schema-based data modeling. It emphasizes
the importance of data normalization and distance-based learning in medical data
analysis.


AUTHOR
------
Project Title : Breast Cancer Prediction Using Snowflake Schema and K-Nearest Neighbors
