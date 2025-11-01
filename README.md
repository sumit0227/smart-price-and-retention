# smart-price-and-retention

**data driven solutions for AirBnb and telecom industries**

---

# Airbnb Price Prediction & Customer Churn Prediction

## Project Overview

This repository contains two major data science projects involving real-world datasets:  
1. **Airbnb Price Prediction and Insights**  
2. **Customer Churn Prediction**

Both projects involve extensive data exploration, preprocessing, feature engineering, model development, and evaluation using machine learning techniques with Python.

***

## Part A: Airbnb Price Prediction and Insights

### Objective

To predict Airbnb listing prices based on various features of the listings and to gain insights about factors influencing pricing.

### Dataset

- Dataset containing 74,111 Airbnb listings with 29 features including property type, amenities, location, host details, reviews, and pricing.
- Target variable: price (exponentiated from logprice)

### Key Steps

- Data exploration and preprocessing including handling missing values, outlier detection, and transformation of target variable from log-price to actual price.
- Feature engineering: extraction of host experience, amenities count, encoding categorical variables.
- Train-test split for model validation.
- Development of Random Forest regression model.
- Model evaluation using R-squared, MAE (Mean Absolute Error), and RMSE (Root Mean Squared Error).
- Visualization of prediction accuracy and feature importance.

### Insights

- Missing values were handled by appropriate imputations (median/mode).
- Price distribution shows significant outliers, which were accounted for during modeling.
- More amenities and host experience tend to correlate with higher prices.
- The Random Forest Regressor effectively captured complex nonlinear relationships in the data.
- Model results showed good predictive performance, indicating reliable pricing estimation for Airbnb listings.

***

## Part B: Customer Churn Prediction

### Objective

To build a machine learning model that reliably predicts customer churn for a telecom company based on customer demographics, services, contract and payment details.

### Dataset

- Dataset containing 7,043 customer records with 21 features, including demographics, service subscriptions, contract type, monthly charges, and churn status as the target.

### Key Steps

- Data exploration and preprocessing including converting TotalCharges to numeric, imputing missing values, encoding categorical variables, and scaling numeric features.
- Feature engineering and encoding of binary and multi-category variables.
- Splitting data into training and testing sets with stratification on target variable.
- Building and tuning a Random Forest Classifier using GridSearchCV for hyperparameter optimization.
- Model evaluation using accuracy, precision, recall, F1 score, and confusion matrix.
- Feature importance analysis to identify churn drivers.

### Insights

- Cleaning and preprocessing ensured high data quality for modeling.
- The Random Forest Classifier provided good performance with accuracy around 79% after tuning.
- Key features influencing churn prediction included contract type, tenure, monthly charges, and tech support availability.
- The model demonstrated balanced classification capability and can assist telecoms in proactive churn management.

***

## Technologies Used

- Python 3 with libraries: pandas, numpy, matplotlib, seaborn, scikit-learn
- Machine learning models: Random Forest Regressor and Classifier
- Data preprocessing and feature engineering techniques
- Model evaluation metrics for regression and classification

***

## How to Use

1. Clone this repository.
2. Install the dependencies: `pip install -r requirements.txt` (if provided)
3. Open respective notebooks (`PART-A.ipynb` for Airbnb, `PART-B.ipynb` for Churn).
4. Run cells sequentially to reproduce data preprocessing, model training, and evaluation.
5. Analyze insights, visualizations, and model performance embedded in notebooks.

***

## Project Insights Summary

| Aspect               | Airbnb Price Prediction                          | Customer Churn Prediction                        |
|----------------------|-------------------------------------------------|-------------------------------------------------|
| Data Size            | 74,111 listings                                 | 7,043 customers                                 |
| Target               | Airbnb price                                    | Churn (yes/no)                                  |
| Preprocessing        | Missing value imputation, feature extraction    | Missing value handling, categorical encoding    |
| Models               | Random Forest Regression                         | Random Forest Classification with GridSearchCV |
| Evaluation Metrics   | R2, MAE, RMSE                                   | Accuracy, Precision, Recall, F1 Score           |
| Noteworthy Features  | Amenities count, host experience, location      | Contract type, tenure, monthly charges          |
| Outcome              | Good predictive accuracy for pricing            | Reliable churn prediction with ~79% accuracy    |

***

## Conclusion

This project delivers practical ML solutions for price prediction and churn classification, combined with deep insights obtained from preprocessing and feature importance analyses. It showcases end-to-end workflow from raw data to actionable models for business applications.



[1](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/118753464/317c951e-fb27-409a-a0b5-ef317875f76e/PART-A.ipynb)
[2](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/118753464/d2e5ac58-7b4c-4a5b-b541-25a2d2383547/PART-B.ipynb)
