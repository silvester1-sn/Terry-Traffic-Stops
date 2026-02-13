# Terry-Traffic-Stops
# Overview
Analysis of Terry Traffic Stops around 1967 in Ohio to justify a criteria for "Reasonable suspicion Stop" by if an Arrest was Made. 
# Problem statement
Predict wheather a Terry Stop results in an arrest from :
- The type of call made i.e Suspicion calls
- Time of day of stop
- If a Frisk was done
- Subjects Gender
- Possession of weapon by subject

# Approach
The binary Model uses feature selection on columns to build a model to satisfy the problem statemnt. 
# Relevance
- Model provides Analysis useful to Officer training on Suspicion 
- Help Law enforcement evaluate patterns leading to arrest
- Data driven oversight understanding and judgements
- Thin trancparency in arrests ,limiting discrimination
# Dataset
The Dataset is Sourced from the Seattle government state [website](https://data.seattle.gov/Public-Safety/Terry-Stops/28ny-9ts8/data_preview). 

To combact effects of class imbalance on the Model Training , the SMOTE technique is to be used.

# Evaluation
The following is a likelihood of a Stop subject in possession of a weapon :
  - Male   - 7%
  - Female - 3%
- White - 7%
- Black or African American - 6% 
- Asian - 6%
- Hispanic - 6% 
- American Indian or Alaska Native - 5%
- Native Hawaiian or Other Pacific Islander  - 4%


Fitting the Logistic Regression and Decision Tree Model

 Metric | LogisticRegression | Decision Tree |
| :--- | :---: | :---: |
| Accuracy | 58% | 59% |
| Precision | 16.38% | 16.54% |
| Recall | 64% | 63% |
| F1 Score | 26% | 26% |
| ROC-AUC Score | 65% | 65% |


The Decision Tree had;
   - Training Accuracy: 0.5863049305499147
   - Testing Accuracy: 0.5881815412732257
       

# summary
On the ROC curve, both Models had and AUC of 65%. Considering the nature of our data this indicates a strong probability generation power and functionality of the models .


Arguably, Satisfies the Metrics of success.
