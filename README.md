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
  
The dataset, diabetes _ 012 _ health _ indicators _ BRFSS2015.csv is a clean dataset of 253,680 survey responses to the CDC's BRFSS2015. The target variable Diabetes_012 has 3 classes. 0 is for no diabetes or only during pregnancy, 1 is for prediabetes, and 2 is for diabetes. There is a class imbalance in this dataset. This dataset has 21 feature variables  
  
### Diabetes Dataset Features
Input variables:  
**** Diabetes data:  
**Diabetes_012** : you have diabetes (0,1,2) - target feature  
  
0 = Not diabetic  
1 = Pre diabetic  
2 = diabetic  
  
**HighBP** : Adults who have been told they have high blood pressure by a doctor, nurse, or other health professional (0,1)  
**HighChol** : Have you EVER been told by a doctor, nurse or other health professional that your blood cholesterol is high? (0,1)  
**CholCheck** : Cholesterol check within past five years (0,1)  
**BMI** : Body Mass Index (BMI)  
**Smoker** : Have you smoked at least 100 cigarettes in your entire life? [Note: 5 packs = 100 cigarettes] (0,1)  
**Stroke** : (Ever told) you had a stroke. (0,1)  
**HeartDiseaseorAttack** : Respondents that have ever reported having coronary heart disease (CHD) or myocardial infarction (MI) (0,1)  
**PhysActivity** : Adults who reported doing physical activity or exercise during the past 30 days other than their regular job (0,1)  
**Fruits** : Consume Fruit 1 or more times per day (0,1)  
**Veggies** : Consume Vegetables 1 or more times per day (0,1)  
**HvyAlcoholConsump** : Heavy drinkers (adult men having more than 14 drinks per week and adult women having more than 7 drinks per week)(0,1)  
**AnyHealthcare** : Do you have any kind of health care coverage, including health insurance, prepaid plans such as HMOs, or government plans such as Medicare, or Indian Health Service? (0,1)  
**NoDocbcCost** : Was there a time in the past 12 months when you needed to see a doctor but could not because of cost? (0,1)  
**GenHlth** : Would you say that in general your health is: rate (1 ~ 5)  
**MentHlth** : Now thinking about your mental health, which includes stress, depression, and problems with emotions, for how many days during the past 30 days was your mental health not good? (0 ~ 30)  
**PhysHlth** : Now thinking about your physical health, which includes physical illness and injury, for how many days during the past 30 days was your physical health not good? (0 ~ 30)  
**DiffWalk** : Do you have serious difficulty walking or climbing stairs? (0,1)  
**Sex** : Indicate sex of respondent (0,1) (Female or Male)  
**Age** : Fourteen-level age category (1 ~ 14)  
**Education** : What is the highest grade or year of school you completed? (1 ~ 6)  
**Income** : Is your annual household income from all sources: (If respondent refuses at any income level, code "Refused.") (1 ~ 8)  

### Findings from the initial dataset examination  
This dataset is imbalanced, with only 17.3% of the population having diabetes (15.3%) or prediabetes (2. 01%) condition, and the rest of the 82.7% of the population has no diabetes condition.
![image](https://github.com/sreegurram/capstone/assets/146612066/03d8a2ec-8f4b-4cda-b58f-807e226458de)  

The dataset's Body Mass Index (BMI) data has outliers, and the distribution is skewed to the left. After removing the records with BMI > 52, the data distribution is almost symmetrical.  
The below image illustrates the BMI distribution along with other features, Physical Health (PhyHlth) and Mental Health (MentHlth)
![image](https://github.com/sreegurram/capstone/assets/146612066/49ed3d3d-ce38-4b49-b208-24a87c447252)

   
## Methodology
I have created a diabetes prediction model using different Machine Learning algorithms, such as Logistic Regression, Random Forest Classifier, Decision Tree Classifier, and XGBoost. I will assess the performance of each model using metrics like AUC, accuracy, precision, recall, and F1 score. The model with the best performance will be used to predict diabetes in individuals based on identified risk factors.

## Results
### Discover which risk factors are most predictive of Diabetes risk.  
- Based on the EDA results, below are the observations made regarding diabetes risk factors.    
- Most people with Diabetes also have high blood pressure (High BP), high cholesterol (High Chol), and high BMI.   
- Both men and women are equally susceptible to Diabetes.   
- The age groups most affected are 60-64, 65-70, and 70-74. Smoking and alcohol consumption have minimal effects on Diabetes.   
- Most people with Diabetes have less physical activity and difficulty walking.   
- Poor general health is linked to both difficulty in walking and poorer physical health. Mental health is also affected similarly.   
- Higher-income levels may lead to better overall health.   
- BMI has a positive correlation with Diabetes, and high cholesterol and high blood pressure also have a positive correlation with Diabetes.  
#### The below image illustrates the High Cholestrol, High BP and BMI risk factors for the Diabetes.
![image](https://github.com/sreegurram/capstone/assets/146612066/6bf6c684-3367-4a4e-a94f-c52f727c546f)

### The selected Model -  
The final selected model, RandomForestClassifier, demonstrated how machine learning can accurately predict whether an individual has diabetes based on various health indicators. The final model was chosen after considering model performance metrics such as accuracy, F1 score, and recall, as well as evaluating the confusion matrices.

##### The below image illustrates that the final selected Diabetes model is accuracy is at 97% (% of the correct predictions made by the model)
![image](https://github.com/sreegurram/capstone/assets/146612066/726dc1ed-3e4e-442a-982b-767c94989110)


## Future possible work
- Betterment of results using different hyperparameters for tuning
- Implementing more Artificial Neural Network (ANN) models to gain better results
- Using the same method to predict the response

## Outline of project
#### Link to notebook 1 - https://github.com/sreegurram/capstone/blob/main/src/Diabetes_multiclass-012_EDA.ipynb - This notebook contains the exploratory data analysis.
#### Link to notebook 2 - https://github.com/sreegurram/capstone/blob/main/src/Diabetes_multiclass-012_EDA_ModelPred.ipynb - Initial Predictions using simple ML models
#### Link to notebook 3 - https://github.com/sreegurram/capstone/blob/main/src/Diabetes_multiclass-012_EDA_ModelPred_ANN.ipynb - Diabetes prediction Hyper parameter tuned ML Models and Diabetes prediction using ANN
#### Link to ModelComparision images - https://github.com/sreegurram/capstone/blob/main/img/Final%20Selected%20model%20performance.png - Final model performance metrics

## Contact and Further Information
#### Author : Sreedevi Gurram
#### Connect on LinkedIn : https://www.linkedin.com/in/sreedevi-gurram-a27219266/
#### Explore Github : https://github.com/sreegurram/

### References: 
#### Ref1 - https://www.cdc.gov/brfss/annual_data/annual_2015.html
#### Ref2 - https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7487151/
