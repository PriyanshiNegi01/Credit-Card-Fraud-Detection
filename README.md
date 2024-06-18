# Credit Card Fraud Detection
This project aims to build a machine learning model to detect fraudulent credit card transactions. The dataset used contains 284,807 transactions, where the goal is to predict whether a transaction is normal or fraudulent.

### Project Overview
- **Objective**: Develop a binary classification model to predict fraudulent transactions.
- **Dataset**: 284,807 credit card transactions with 30 features.

### Steps Involved

1. **Data Preprocessing**:
    - Cleaned the dataset by removing duplicates and handling missing values.
    - Exploratory data analysis to understand feature distributions and correlations.
    - Identified and addressed the class imbalance in the dataset.

2. **Imbalanced Data Handling**:
    - Implemented undersampling and oversampling techniques to balance the dataset.
    - Evaluated model performance using both techniques.

3. **Model Implementation**:
    - Trained three different classifiers: Logistic Regression, Decision Tree Classifier, and Random Forest Classifier.
    - Evaluated models using metrics such as accuracy, precision, recall, and F1 score.

4. **Model Performance and Selection**:
    - **Undersampling**:
        - **Logistic Regression**: Balanced accuracy (0.95), precision (0.99), and recall (0.92).
        - **Random Forest Classifier**: Similar performance to Logistic Regression.
        - **Decision Tree Classifier**: Lower performance, less robust for unseen data.
    - **Oversampling**:
        - High accuracy across all models, but potential for overfitting.
        - Significant performance improvement observed, but overfitting remains a concern.

5. **Model Evaluation**:
    - Logistic Regression provided a good balance and interpretability.
    - Random Forest Classifier, despite potential overfitting, demonstrated strong performance and was chosen for its high accuracy.

### Conclusion
- Logistic Regression is effective for balancing identification of fraudulent transactions and minimizing false positives.
- Random Forest Classifier, saved after oversampling, was selected for deployment due to its robust performance.

### Repository Structure
- `Credit_Card_Fraud_Detection.ipynb`: Jupyter notebook containing all the steps and code for the project.
- `credit_card_fraud_model.pkl`: Saved Random Forest Classifier model.

### Future Work
<!--- Explore additional techniques to address overfitting. -->
- Implement real-time fraud detection using streaming data.
- Test other advanced machine learning models and compare performance.

### Acknowledgments
- This project uses the credit card dataset from [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud).

By following this README, you will be able to understand the project's scope, replicate the results, and potentially contribute to future improvements.
