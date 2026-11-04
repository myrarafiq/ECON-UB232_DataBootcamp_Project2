# Ames Housing Price Prediction

## About the Project

This project was completed as part of our Data Science Bootcamp assignment. The goal was to build a regression model that predicts house sale prices using the Ames Housing dataset and submit our predictions to Kaggle.

We experimented with different regression models and approaches during development, including linear models, tree-based models, and Support Vector Regression. Based on our Kaggle experiments, SVR was one of our strongest approaches, so we decided to focus on it for our final notebook.

## Our Approach

Our final notebook walks through the following steps:

1. **Data exploration:** Loading the datasets, checking their structure, and exploring missing values and the distribution of house prices.
2. **Data preprocessing:** Separating numerical and categorical features, handling missing values, standardizing numerical variables, and encoding categorical variables.
3. **Model selection:** Building a Support Vector Regression model using an RBF kernel.
4. **Hyperparameter tuning:** Using GridSearchCV and five-fold cross-validation to test different values of `C` and `gamma`.
5. **Evaluation:** Measuring model performance using Root Mean Squared Error (RMSE) on a separate validation set.
6. **Final predictions:** Retraining the selected model on the full training dataset and generating predictions for the Kaggle test data.

## Model

We used **Support Vector Regression (SVR)** with a Radial Basis Function (RBF) kernel.

We chose this approach because it can capture non-linear relationships between house characteristics and sale prices. We also applied a logarithmic transformation to the target variable to help account for the skewed distribution of house prices.

The preprocessing and regression steps were combined into a pipeline to keep the process consistent during cross-validation.

## Repository Contents

- `Ames_Housing_SVR.ipynb` – Jupyter notebook containing our data exploration, preprocessing, model training, evaluation, and predictions.
- `README.md` – Project overview and instructions.

## How to Run

1. Clone or download this repository.
2. Download the Ames Housing training and test datasets from the Kaggle competition.
3. Open `Ames_Housing_SVR.ipynb` in Google Colab or Jupyter Notebook.
4. Update the dataset file paths in the data loading cell to match your local files or Google Drive.
5. Run the notebook cells in order.
6. The final cell exports a CSV file containing the predicted house sale prices, ready for Kaggle submission.

## Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## What We Learned

Through this project, we learned how important data preprocessing and feature representation are when building regression models. We also got experience comparing different approaches, tuning hyperparameters with cross-validation, evaluating predictions using RMSE, and preparing submissions for a Kaggle competition.

## Team Members

- Myra Rafiq
- Muhammad Abdullah
- Saudha Shaheen
