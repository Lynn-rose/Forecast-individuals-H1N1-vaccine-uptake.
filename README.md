<!-- #region -->

# Forecast individuals' H1N1 vaccine uptake.

![awesome](https://github.com/Lynn-rose/phase-3-project/blob/main/images/WhatsApp%20Image%202024-06-06%20at%209.42.13%20AM.jpeg)

## Business Understanding
### Overview
The H1N1 flu, sometimes called Swine flu is a type of influenza A virus. During the 2009-10 flu season, a new H1N1 virus began causing illness in humans and it was often called Swine flu and was a combination of influenza viruses that infect pigs, birds, and humans. The World Health Organization (WHO) declared the H1N1 flu to be a pandemic in 2009. That year the virus caused an estimated 284,400 deaths worldwide. In August 2010, WHO declared the pandemic over. However, the H1N1 flu strain from the pandemic became one of the strains that cause seasonal flu. Most people with the flu get better on their own. But flu and its complications can be deadly, especially for people at high risk. The seasonal flu vaccine can now help protect against the H1N1 flu and other seasonal flu viruses.

The CDC recommends flu vaccination for everyone aged 6 months and older in the United States since the 2010-2011 flu season. It is crucial for preventing flu and its complications, especially for those at higher risk. Suitability for vaccination or a specific vaccine depends on factors like age, health, and allergies. Various vaccines are approved for different age groups, and some are not recommended for specific individuals. Notably, there are three flu vaccines preferentially recommended for people aged 65 and older.

## Problem Statement
Faced with the reality of how quickly viral diseases like H1N1 and seasonal flu can spread, along with their associated health risks and a notable mortality rate, there is a pressing need to develop a model to accurately identify individuals who are more likely to receive their H1N1 and seasonal flu vaccines.

The goal of the "Flu Shot Learning: Predict H1N1" competition is to predict whether individuals received H1N1 vaccines based on their demographic information, opinions, and health behaviors. This predictive model has significant implications for public health initiatives and vaccine campaigns.


### Objective
To predict the probability for each individual receiving:

H1N1 Vaccine: The likelihood that a person received the H1N1 flu vaccine.

## Data Understanding
The dataset is derived from the National 2009 H1N1 Flu Survey and contains information on 26,707 respondents, with each row representing one individual's responses. The dataset includes:

* Demographic Information: Age group, sex, race, education, income, and employment status.

* Health Behaviors: Measures like washing hands, avoiding large gatherings, and antiviral medication usage.

* Opinions and Knowledge: Levels of concern and knowledge about the H1N1 flu, opinions on vaccine effectiveness, and perceived risks.

* Health and Medical Data: Presence of chronic medical conditions, health insurance status, and healthcare worker status.

* Doctor Recommendations: Whether a doctor recommended the H1N1.

## Data Preprocessing
The following steps were taken in the preparation of the data ready for modelling.

1. Data Cleaning: Selected relevant columns, handled missing values by dropping rows with NaNs.

2. Train-Test Split: Split the dataset into training (80%) and testing (20%) sets.

3. Standardization: Standardized the feature set using StandardScaler.

4. Handling Class Imbalance: Applied SMOTE to balance the class distribution in the training data.

## Modeling

The following models were used during the developing of a machine learning model that can predict whether individuals received the H1N1 vaccine based on demographic information, health behaviors, opinions, and medical data. These models aims to assist public health initiatives in identifying factors that influence vaccine uptake and targeting specific populations to improve vaccination rates.

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier
4. K-Nearest Neighbors (KNN) Classifier

## Evaluation
In this project, multiple evaluation metrics were used to assess the performance of different models in predicting H1N1 vaccine uptake. These metrics provided insights into the accuracy, precision, recall, and overall predictive power of the models.

1. Accuracy
Definition: The proportion of true results (both true positives and true negatives) among the total number of cases examined.

2. Precision
Definition: The proportion of positive identifications that were actually correct.

3. Recall (Sensitivity)
Definition: The proportion of actual positives that were correctly identified.

4. F1-Score
Definition: The harmonic mean of precision and recall, providing a balance between the two metrics.

5. ROC-AUC (Receiver Operating Characteristic - Area Under Curve)
Definition: Measures the ability of the model to distinguish between classes. The ROC curve plots the true positive rate (sensitivity) against the false positive rate (1-specificity).
AUC Value: The area under the ROC curve, which provides a single value representing the model's performance. A higher AUC indicates better model performance.
6. Confusion Matrix
Definition: A table used to describe the performance of a classification model, showing the actual vs. predicted classifications.

## Conclusion
Based on the evaluation metrics (accuracy, ROC-AUC, classification reports), the Random Forest Classifier outperformed other models with the highest test accuracy and robust ROC-AUC scores. This model was selected as the final model for predicting H1N1 vaccine uptake.The following are the results of the metrics used during he modeling:

Random Forest Classifier
* Train Accuracy: 0.79

* Test Accuracy: 0.80

* AUC: 0.78 (train), 0.77 (test)

This model can help public health campaigns identify and target populations that are less likely to receive the vaccine, thereby improving vaccination coverage..

 ## For More Information  
Please review my full analysis in my [Jupyter Notebook](https://github.com/Lynn-rose/phase-3-project/blob/main/index.ipynb) or my [Presentation](https://github.com/Lynn-rose/dsc-phase-1-project-movie-data-analysis/blob/master/presantation.pdf)

For any additional questions, please contact Lynn Rose Achieng, lynn90952@gmail.com
<!-- #endregion -->

```python

```
