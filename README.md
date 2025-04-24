# AI-ADHD-Diagnosis
In this Repository there will be the codes, data processing scripts, and documentation for the project "AI-Powered ADHD Diagnosis: Analyzing Motor Activity and Heart Rate Data Using Machine Learning." The goal of this project is to develop a machine learning model that can classify ADHD patients based on motor activity and heart rate data.
# AI-Powered ADHD Diagnosis: Machine Learning on Motor Activity & Heart Rate Data

## ** Project Overview**
This project applies **machine learning techniques** to analyze **motor activity and heart rate data** for ADHD diagnosis. Traditional ADHD assessment methods rely on **behavioral tests and clinical interviews**, which can be subjective and time-consuming. This project aims to explore **data-driven methods** for ADHD classification using supervised learning models.

## ** Dataset Information**
- **Dataset Name**: [HYPERAKTIV ADHD Diagnosis Data](https://www.kaggle.com/datasets/arashnic/adhd-diagnosis-data)
- **Source**: Kaggle  
- **Description**:  
  - **51 ADHD patients** and **52 clinical control subjects**  
  - **Time-series data** on motor activity and heart rate variability  
  - **Neuropsychological test results** (CPT-II Conners Performance Test)  
  - **Demographic data** (Age, Sex, Medication Status)  

## ** Project Goals**
**Clean and preprocess dataset** (handle missing values, remove outliers)  
**Perform Exploratory Data Analysis (EDA)** (visualizing trends in data)  
**Feature Engineering** (extract statistical & time-series features)  
**Train ML models** (Logistic Regression, Random Forest, SVM, Neural Networks)  
**Evaluate model performance** (Accuracy, Precision, Recall, F1-score, ROC-AUC)  

---
## **Machine Learning Approach**
**The following supervised learning models will be tested:**
**Logistic Regression**
**Random Forest**
**Support Vector Machine (SVM)**
**Neural Networks (MLP)**
**Feature selection techniques will be used to optimize performance.**

---
## ** Results & Performance Metrics**
**After training the models, their performance will be assessed using:**
**Accuracy**
**Precision & Recall**
**F1-score**
**ROC-AUC Curve**
**Confusion Matrix Analysis**
---
## **Project Status:**
**1) Cleaning and Restructuring CPT Test Data on (Feb 22nd 2025)**
**I processed and transformed CPT test data to prepare it for analysis. The dataset was initially in a wide format with multiple trial and response columns. I first loaded the CSV file into a Pandas DataFrame and renamed columns for consistency. Then, I classified the columns into summary-level data and trial-level data. Using Pandas’ melt() function, I reshaped the trial and response data into a long format, where each row represents a single trial-response pair. I then merged this transformed data with participant-level summary metrics to create a structured dataset. Finally, I handled missing values, converted data types, and performed basic validation to ensure the dataset was ready for analysis. This cleaned and structured format makes it easier to perform statistical analysis and visualization on the CPT test results.**
****All of this process has been implemented in the adhd_w1.ipynb file.****

**2) Status update on (March 24th 2025): I have completed the EDA process as well and uploaded the eda coding file In this file I have done the analysis of Distribution of ADHD Diagnosis to see the count of the people who have and don't have ADHD. And then there is the Raw Score HitRT analysis in a box plot.**
**And then there is a bar chart of Top 15 Important features score where it shows which will be the best feature to make as a target variable. At last I have trained and evaluated 3 models ie., **XGBoost, LightGBM, Gaussian Naive Bayes** it has the results of all the metrics and a confusion matrics.**

 
