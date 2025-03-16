# Find-Default_Capstone-Project
This project focuses on detecting fraudulent credit card transactions using machine learning techniques. The dataset which contains anonymized transaction features and is highly imbalanced, with fraudulent cases being significantly fewer than non-fraudulent ones.
This project aims to detect fraudulent transactions in a credit card dataset using machine learning techniques. The dataset is highly imbalanced, so techniques such as SMOTE (Synthetic Minority Over-sampling Technique) are used to balance the dataset before training models. Two machine learning models, XGBoost and Random Forest, are implemented to classify transactions as fraud or non-fraud.

## Dataset
##**https://kh3-ls-storage.s3.us-east-1.amazonaws.com/DS Project Guide Data Set/creditcard.csv**


Click the above link for data set 


The dataset used is `creditcard.csv`, which contains:

* Time: The time elapsed from the first transaction.  
* Amount: The transaction amount.  
* 28 anonymized PCA features.  
* Class: Target variable (0 for non-fraud, 1 for fraud).

## Project Workflow

1. Data Preprocessing

   * Handle missing values (if any).  
   * Standardize the `Amount` feature.  
   * Convert `time` to hours.  
   * Drop unnecessary columns.  
2. **Handling Class Imbalance**

   * Apply SMOTE to balance fraud and non-fraud transactions.  
3. Train-Test Split
* Data is split into 80% training and 20% testing.
  
4. Model Training & Evaluation

   * XGBoost Classifier  
   * Random Forest Classifier  
   * Hyperparameter tuning using `RandomizedSearchCV`.  
   * Model evaluation using classification metrics (confusion matrix, precision, recall, F1 score, and ROC-AUC score).  
5. Feature Importance Analysis

   * Plot feature importance for both models.  
6. Performance Visualization

   * ROC and Precision-Recall Curves.

## Installation

### Prerequisites

Ensure you have Python installed (\>=3.7) and install the required libraries:

pip install numpy pandas matplotlib seaborn scikit-learn imbalanced-learn xgboost

## Running the Code

1. Clone the repository or download the `creditcard.csv` dataset.  
2. Run the Python script:

python fraud\_detection.py

## Results

* XGBoost and Random Forest classifiers were used.  
* SMOTE significantly improved fraud detection.  
* Feature importance was visualised.  
* ROC-AUC and precision-recall curves were plotted for model evaluation.

## Future Improvements

* Experiment with deep learning techniques (e.g., Neural networks, autoencoders).  
* Feature selection techniques to improve model performance.  
* Further hyperparameter tuning for better precision and recall bal
