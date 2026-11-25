# CIE 2 – Activity 2: Spam Email Detection Using Logistic Regression

## 1. Objective
The objective of this activity is to build a Logistic Regression model to classify emails as Spam or Not Spam. The model predicts the probability of an email being spam and evaluates its performance using classification metrics.

## 2. Dataset Information
- **Dataset Name:** Spam Email Dataset
- **Source:** [Kaggle – Spam Email Dataset](https://www.kaggle.com/datasets/jackksoncsie/spam-email-dataset)
- **Total Records:** 6000
- **Total Columns:** 16
- **Target Variable:** Spam Indicator

### Class Description
- **0 – Not Spam:** A genuine or normal email.
- **1 – Spam:** An unwanted or suspicious email.

### Input Features
- Attachments
- Link Count
- Word Count
- Uppercase Count
- Exclamation Count
- Question Count
- Dollar Count
- Punctuation Count
- HTML Tags Count

## 3. Data Preparation
The following steps were performed:
1. Loaded the dataset using Pandas.
2. Checked the dataset shape and column information.
3. Checked missing values and duplicate records.
4. Selected the required input features and target variable.
5. Divided the data into 80% training and 20% testing sets.
6. Used stratified splitting to maintain class distribution.
7. Applied StandardScaler to scale the input features.

## 4. Model Development
Logistic Regression was used for binary classification.

- Model: Logistic Regression
- Maximum iterations: 1000
- Train-test split: 80:20
- Random state: 42

The model generates spam probabilities and converts them into class labels using a decision threshold of 0.5.

## 5. Model Evaluation
The model was evaluated using:
- Confusion Matrix
- Accuracy
- Precision
- Recall
- Specificity
- F1-score
- ROC Curve
- ROC-AUC Score
- Classification Report

### Obtained Results

| Metric | Result |
|---|---:|
| Accuracy | 50.17% |
| Precision | 49.82% |
| Recall | 46.81% |
| Specificity | 53.48% |
| F1-score | 48.27% |
| ROC-AUC | 0.4906 |

### Confusion Matrix
- True Negative (TN): 323
- False Positive (FP): 281
- False Negative (FN): 317
- True Positive (TP): 279

## 6. Threshold Comparison
The model was tested using three decision thresholds: 0.3, 0.5 and 0.7.

A threshold of 0.5 was selected for the main evaluation. The comparison shows that changing the threshold affects precision, recall and F1-score.

## 7. New Email Prediction
A new email sample was given to the trained model.

- Predicted Spam Probability: 0.4975
- Predicted Class: 0
- Prediction: Not Spam

## 8. Conclusion
The Spam Email Detection model was successfully developed using Logistic Regression. The model was evaluated using different classification metrics and decision thresholds.

The obtained accuracy was approximately 50.17% and ROC-AUC was 0.4906. These results indicate that the model performs close to random classification and is not suitable for practical deployment in its current form. Better features and further model improvements are required.

## 9. GitHub Profile
**GitHub ID:** [complexiota](https://github.com/complexiota)

## 10. Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

**Activity:** CIE 2 – Activity 2  
**Topic:** Spam Email Detection Using Logistic Regression
