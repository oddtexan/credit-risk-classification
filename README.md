# credit-risk-classification

# Background
In this Challenge,I will use various techniques to train and evaluate a model based on loan risk. I will use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

# Instructions

The instructions for this Challenge are divided into the following subsections:

- Split the Data into Training and Testing Sets

- Create a Logistic Regression Model with the Original Data

- Write a Credit Risk Analysis Report

# Split the Data into Training and Testing Sets

Open the starter code notebook and use it to complete the following steps:

1. Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.

2. Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

3. Split the data into training and testing datasets by using train_test_split.

# Create a Logistic Regression Model with the Original Data

Use your knowledge of logistic regression to complete the following steps:

1. Fit a logistic regression model by using the training data (X_train and y_train).

2. Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

3. Evaluate the model’s performance by doing the following:

      - Generate a confusion matrix.

      - Print the classification report.

******************************************************************

#### **Overview of the Analysis**

**Purpose of the Analysis:**

The primary objective of this analysis was to build and evaluate machine learning models to assess the risk associated with loan applications. The key aim was to classify loans as either low-risk (healthy) or high-risk, using various financial indicators from the applicants.

**Financial Information and Prediction:**

The dataset used for this analysis contained financial details about loan applications, including several features that represent the applicant's financial status and the terms of the loan. The goal was to predict whether a loan would be classified as 0 (healthy loan) or 1 (high-risk loan).

**Machine Learning Process:**

- **Data Preparation:** The dataset was cleaned and formatted to ensure that all required features were available and usable.
- **Feature Selection:** Relevant features were selected to train the machine learning models.
- **Model Training:** Multiple models were trained, including logistic regression and decision tree classifiers.
- **Model Evaluation:** The models were assessed using metrics like accuracy, precision, recall, and F1-score.

**Methods Used:**

- **Logistic Regression:** Selected for its simplicity and effectiveness in binary classification tasks.

---

### **Results**

**Machine Learning Model: Logistic Regression**

- **Accuracy:** 0.99

- **Precision:**
  - Class 0 (Healthy loan): 1.00
  - Class 1 (High-risk loan): 0.85

- **Recall:**
  - Class 0: 0.99
  - Class 1: 0.91

- **F1-Score:**
  - Class 0: 1.00
  - Class 1: 0.88

---

### **Summary**

**Model Performance:**

**Logistic Regression:**

- **Strengths:** The model performs exceptionally well overall, with near-perfect precision and recall for healthy loans. It also demonstrates solid performance for high-risk loans, reflected in an F1-score of 0.88.
- **Weaknesses:** Precision for high-risk loans is slightly lower, indicating that some healthy loans might be misclassified as high-risk.

---

### **Recommendation**

Based on the evaluation metrics, the logistic regression model is recommended for deployment. It delivers excellent performance, particularly in predicting healthy loans with near-perfect precision and recall, while also performing well in predicting high-risk loans. This balance is essential for minimizing financial risk while maintaining high prediction accuracy.

---

### **Performance Consideration**

- **Importance of Predicting High-Risk Loans:** Since predicting high-risk loans (class 1) is critical due to potential financial losses, the model’s recall of 0.91 for this class is beneficial in identifying most high-risk loans.
- **Overall Balance:** Logistic regression provides a strong balance between precision and recall across both classes, making it a reliable model for a loan approval system.

For future improvements, exploring additional features or alternative models may further enhance performance.  
