# **Clinical Movement Patterns and Predictive Models of Long COVID**

## *Objective*

The objective of this project is to investigate whether gait analysis can be used as a potential biomarker for diagnosing and monitoring long COVID. Using clinical movement data, the project applies statistical and machine learning methods to identify gait differences between long COVID patients and healthy controls, and to evaluate predictive models for clinical decision support.

## *Key Questions*

1. ### Gait Differences Between Long COVID patients(Case) and Controls
What biomechanical differences exist in walking velocity, step length and step width?

2. ### Model Performance in Predicting Long COVID
Which machine learning models provide the most reliable predictions for classifying long COVID patients based on gait data?

3. ### Demographic Comparisons
How do age, gender, height and BMI differ between long COVID patients and control groups?

4. ### Feature Importance
Which gait features (velocity, step length, step width, BMI) contribute most to model accuracy?

5. ### Statistical Significance
Are the observed gait differences statistically significant between groups?

6. ### Clinical Potential
Can gait-based machine learning models serve as non-invasive tools for diagnosis and monitoring of long COVID?

## *Data Used*

1. ### Clinical Data:
1070 participants, with long COVID patients and healthy controls. Includes demographics (age, gender, height, BMI).

2. ### Gait Data:
Walking trials captured using the Stepsense motion analysis system across 32 skeletal joints.

3. ### Derived Features:
Gait parameters such as average/maximum velocity, step length, step width.

4. ### Trial Data:
Multiple walking and balance trials including Romberg and Fukuda tests, both with and without cognitive distractions.

## *Methodology*

1. ### *Database Schema & Integration*:
Data normalised into separate tables for participants, demographics, and trial-level gait metrics.

2. ### *Feature Engineering*:

Step length: Euclidean distance between heel strikes.

Step width: Lateral displacement of feet.

Walking velocity: Mean and maximum trial speeds.

BMI derived from height and weight.

3. ### *Statistical Testing*:

Independent t-tests comparing long COVID and control groups on demographics and gait features.

4. ### *Machine Learning Models*:

Logistic Regression

Random Forest

Gradient Boosting

XGBoost

Support Vector Machine (SVM)

Voting Classifier (ensemble of best models)

## *Evaluation Metrics*:
Accuracy, Precision, Recall, F1-score, AUC-ROC.

## *Observations and Results*

1. ### *Demographic Insights*:
Long COVID patients showed no major demographic differences from controls in age, gender, or height. Slight differences observed in BMI.

2. ### *Gait Differences*:

Higher maximum walking velocity in long COVID patients.

Slightly shorter step length.

Narrower step width, suggesting compensatory balance adjustments.

3. ### *Model Performance*:

Voting Classifier: Best performer (Accuracy: 68%, AUC: 0.74).

Random Forest & XGBoost: Strong results (~67% accuracy, AUC up to 0.76).

Logistic Regression: Weakest performer (Accuracy: 55%, AUC: 0.58).

4. ### *Feature Importance*:
Step width and velocity emerged as the strongest predictors of long COVID classification.

## *Recommendations*

Based on the findings, the following conclusions and recommendations are made:

Voting Classifier should be prioritised as the most effective predictive tool, supported by Random Forest and XGBoost models.

Gait analysis shows significant promise as a non-invasive biomarker for diagnosing and monitoring long COVID.

Further research is needed with larger, more diverse datasets to validate model robustness.

Expansion into deep learning methods could uncover more complex movement patterns beyond the engineered features.

Clinical application should focus on integrating gait analysis into diagnostic workflows, particularly in long COVID monitoring programmes.
