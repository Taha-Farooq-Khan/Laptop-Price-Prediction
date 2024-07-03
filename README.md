# Laptop-Price-Prediction

# Predicting Laptop Prices: A Machine Learning Approach

## Introduction

As technology advances, laptops have become an integral part of our daily lives. Whether for work, entertainment, or education, choosing the right laptop involves considering various factors, including specifications, brand, and price. In this article, we'll explore how machine learning models can predict laptop prices based on relevant features.

## Dataset

We'll start by loading our dataset, which contains information about various laptops. The dataset includes features such as RAM capacity, storage (SSD and HDD), graphics card memory, brand, processor details, and warranty information.

## Data Preprocessing

Before building our predictive models, we need to preprocess the data. Here are the steps we'll follow:

1. **Feature Extraction:**
   - Extract numeric values from the 'rating' column.
   - Remove unnecessary columns ('Number of Ratings', 'Number of Reviews', and 'rating').

2. **Feature Scaling:**
   - Standardize numeric features (RAM, SSD, HDD, and graphics card memory) using the StandardScaler.

3. **One-Hot Encoding:**
   - Encode categorical features (brand, processor brand, processor name, RAM type, OS, OS bit, and warranty) using one-hot encoding.

## Model Selection and Training

We'll use the Random Forest regressor for our prediction task. Random Forest is an ensemble method that combines multiple decision trees to improve accuracy. Here's how we'll proceed:

1. **Data Splitting:**
   - Split the dataset into training and testing sets (80% training, 20% testing).

2. **Model Training:**
   - Fit the Random Forest model to the preprocessed training data.

3. **Prediction and Evaluation:**
   - Predict laptop prices on the testing set.
   - Calculate the Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) to evaluate model performance.

## Cross-Validation

To assess the model's robustness, we'll perform k-fold cross-validation. This technique divides the data into k subsets (folds) and trains the model on k-1 folds while validating on the remaining fold. We'll calculate the RMSE for each fold and report the mean RMSE.

## Results

Our Random Forest model provides accurate predictions for laptop prices. The MAE and RMSE indicate how closely our predictions align with the actual prices. Additionally, cross-validation ensures that our model generalizes well to unseen data.

## Conclusion

Predicting laptop prices using machine learning models allows us to make informed decisions when purchasing a new laptop. By considering relevant features and leveraging powerful algorithms, we can estimate prices accurately.
