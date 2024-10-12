
# Telecom Churn Prediction

This project aims to predict customer churn using a variety of machine learning techniques. The dataset used includes features such as call usage statistics, which are analyzed to identify customers likely to churn.

## Project Structure

- **Data Preprocessing**: Data is cleaned and imputed where necessary to ensure consistency. Missing values are handled, and feature scaling is applied.
- **PCA for Dimensionality Reduction**: Principal Component Analysis (PCA) is used to reduce the dimensionality of the dataset and retain only the most significant features for model training.
- **Random Forest Classifier**: A Random Forest Classifier is trained to predict churn. GridSearchCV is applied to tune hyperparameters, optimizing the model performance.
- **Feature Engineering**: Recursive feature elimination (RFE) is used to select the most relevant features for training the model.

## Key Steps

1. **Data Cleaning and Imputation**: Missing data is filled using various techniques.
2. **Dimensionality Reduction**: PCA is applied to reduce feature dimensions while retaining 89 principal components.
3. **Model Training**: The Random Forest Classifier is trained using cross-validation and hyperparameter tuning (n_estimators, max_depth, etc.).
4. **Model Evaluation**: The model is evaluated on the test set, and predictions are generated.

## Outputs

- The model predicts the probability of churn for each customer in the test dataset.
- A submission file (`submission.csv`) is generated, containing the churn probabilities.

## Insights & Recommendations

- **Key Features Influencing Churn**:
  - Customers with lower usage of local incoming and ISD outgoing calls.
  - Lower charges for certain outgoing calls in July and incoming calls in August.
  - Increasing costs in the action phase.
  - Decreasing incoming minutes for certain operators in August.

### Recommendations for Targeting Customers
- Focus on customers with lower usage and increasing costs in the action phase.
- Offer incentives to customers with decreasing usage, particularly for specific operators, to reduce churn likelihood.


## Requirements

- Python 3.x
- Libraries:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib

## Acknowledgements

This project is part of the upGrad and IIITB Machine Learning & AI Program.

--- 
