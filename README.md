# Project Title - Diabetes Prediction Using Machine Learning
## Author - Sreedevi Gurram

## Executive summary
This project focuses on analyzing medical data related to Diabetes and building predictive models to predict its status. It includes exploratory data analysis (EDA), observations, and the development of various models to predict the presence or absence of Diabetes.
## Rationale
Diabetes is a chronic disease that affects millions of people in the United States every year and poses a significant financial burden on the economy. The disease is caused by the body's inability to regulate glucose levels in the blood effectively, leading to reduced quality of life and life expectancy. Diabetes is associated with various complications like heart disease, vision loss, lower-limb amputation, and kidney disease. Although there is no cure for Diabetes, lifestyle changes like losing weight, eating healthily, being active, and receiving medical treatments can mitigate the harms of the disease. The Centers for Disease Control and Prevention (CDC) estimates that as of 2018, 34.2 million Americans have Diabetes, 88 million have prediabetes, and a significant proportion of them are unaware of their risk. Diabetes also places a considerable burden on the economy, with costs approaching 400 billion dollars annually.

Predictive models can assist healthcare companies and public health officials in assessing the risk of developing Diabetes.

## Research Question
Predicting Diabetes and improving understanding of the relationship between lifestyle and Diabetes in the US

## Data Sources
The Diabetes Health Indicators Dataset comprises healthcare statistics, lifestyle survey responses of individuals, and their diabetes diagnosis. The dataset includes demographic information, lab test results, and patient survey answers. The target variable for classification is the patients' health status: whether they have Diabetes, are Prediabetes, or are healthy (no diabetes).
## Methodology
I am developing a diabetes prediction model using various Machine Learning algorithms, including Logistic Regression, Random Forest Classifier, Decision Tree Classifier, and XGBoost. I will evaluate the performance of each model using metrics such as AUC, accuracy, precision, recall, and F1 score. The best performing model will be leveraged to predict Diabetes of a given person based on the identified risk factors.

## Results
### Discover which risk factors are most predictive of Diabetes risk.
Based on the EDA results, below are the observations made regarding diabetes risk factors.
Most people with Diabetes also have high blood pressure (High BP), high cholesterol (High Chol), and high BMI. 
Both men and women are equally susceptible to Diabetes. 
The age groups most affected are 60-64, 65-70, and 70-74. Smoking and alcohol consumption have minimal effects on Diabetes. 
Most people with Diabetes have less physical activity and difficulty walking. 
Poor general health is linked to both difficulty in walking and poorer physical health. Mental health is also affected similarly. Higher income levels may lead to better overall health. 
BMI has a positive correlation with Diabetes, and high cholesterol and high blood pressure also have a positive correlation with Diabetes.

#### The final selected model, RandomForestClassifier, demonstrated how machine learning can accurately predict whether an individual has diabetes based on various health indicators. The final model was chosen after considering model performance metrics such as accuracy, F1 score, and recall, as well as evaluating the confusion matrices.

## Future possible work
- Betterment of results using different hyperparameters for tuning
- Implementing more Artificial Neural Network (ANN) models to gain better results
- Using the same method to predict response

## Outline of project
#### Link to notebook 1 - https://github.com/sreegurram/capstone/blob/main/src/Diabetes_multiclass-012_EDA.ipynb - This notebook contains the exploratory data analysis.
#### Link to notebook 2 - https://github.com/sreegurram/capstone/blob/main/src/Diabetes_multiclass-012_EDA_ModelPred.ipynb - Initial Predictions using simple ML models
#### Link to notebook 3 - https://github.com/sreegurram/capstone/blob/main/src/Diabetes_multiclass-012_EDA_ModelPred_ANN.ipynb - Diabetes prediction Hyper parameter tuned ML Models and Diabetes prediction using ANN
#### Link to ModelComparision images - https://github.com/sreegurram/capstone/blob/main/img/Final%20Selected%20model%20performance.png - Final model performance metrics

## Contact and Further Information
#### Author : Sreedevi Gurram
#### Connect on LinkedIn : https://www.linkedin.com/in/sreedevi-gurram-a27219266/
#### Explore Github : https://github.com/sreegurram/

### References: https://www.cdc.gov/brfss/annual_data/annual_2015.html
