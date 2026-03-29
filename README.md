
**Student Performance Prediction (Multi Linear Regression)**
 
**Overview**

This project uses Multiple Linear Regression to predict the Performance Index of students based on several academic and lifestyle factors. The dataset contains 10,000 rows and 6 columns, cleaned and prepared for modeling.

Problem Statement:

We aim to predict the Performance Index using the following features:
1. 	Hours Studied
2. 	Previous Scores
3. 	Extracurricular Activities (Yes/No → 1/0)
4. 	Sleep Hours
5. 	Sample Question Papers Practiced

Steps Followed
1. Import Libraries
    - Pandas, NumPy for data handling
    - Matplotlib, Seaborn for visualization
    - Scikit-learn for model building and evaluation
2. Load Dataset
    - File:Student_Preformance.csv 
    - Shape: 10,000 rows × 6 columns
3. Data Cleaning
     - Removed 127 duplicate rows
     - Converted categorical column Extracurricular Activities into numerical values (Yes=1, No=0)
     - Checked for null values (none found)
     - Outlier detection using IQR (no significant outliers found)
4. Exploratory Data Analysis (EDA)
     - Univariate Analysis: Histograms for Hours Studied, Previous Scores, Sleep Hours
     - Categorical Analysis: Countplot for Extracurricular Activities
     - Correlation Heatmap:
     - Previous Scores → strongest correlation with Performance Index (0.92)
     - Hours Studied → moderate correlation (0.38)
     - Extracurricular Activities → least impact
5. Model Building
     - Train-test split: 70/30
     - Model: Linear Regression (OLS method)
     - Extracted coefficients and intercept
6. Model Evaluation
      - Metrics used:
        - Mean Squared Error (MSE)
        - Mean Absolute Error (MAE)
        - R² Score

Results
  - Previous Scores is the most influential factor.  
  - Hours Studied also contributes significantly.  
  - Extracurricular Activities have minimal impact.  
  - The model achieves high accuracy with R² ≈ 0.98.  



Future Enhancements
   - Hyperparameter tuning for better accuracy
   - Try advanced models (Random Forest, XGBoost)
   - Deploy as a web app for real-time predictions


