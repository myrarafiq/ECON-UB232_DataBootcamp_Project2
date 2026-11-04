# Ames Housing Price Prediction

## About the Project

This project was completed as part of our Data Bootcamp's Project 2. The goal was to build a machine learning model that predicts house sale prices using the Ames Housing dataset and submit our predictions to Kaggle.

During the project, we explored different regression approaches, including linear models, tree-based models, and Support Vector Regression (SVR). After experimenting with these approaches, we chose SVR for our final notebook because it was one of our strongest-performing models in our Kaggle experiments.

## What We Did

Our final notebook covers the main steps we followed to prepare the data, build the model, and generate predictions.

1. **Data exploration:** Loaded the training and test datasets, looked at the available features, checked missing values, and explored the distribution of house prices.

2. **Feature engineering:** Created additional features to give the model more information about each house. These included total living area, number of bathrooms, house age, garage features, and combinations of house size and quality.

3. **Data preprocessing:** Handled missing values, standardized numerical features, and converted categorical features into a format the model could use.

4. **Model building:** Trained a Support Vector Regression (SVR) model with an RBF kernel to capture relationships between house features and sale prices.

5. **Target transformation:** Applied a Yeo-Johnson transformation to the sale prices to help make their distribution more balanced.

6. **Evaluation:** Split the training data into training and validation sets and used Root Mean Squared Error (RMSE) to evaluate how well the model predicted house prices. We also used plots to compare actual and predicted prices and look at prediction errors.

7. **Kaggle submission:** Retrained the model using the full training dataset, generated predictions for the test dataset, and exported the results as a CSV file.

## Final Model

Our final model uses **Support Vector Regression (SVR)** with an RBF (Radial Basis Function) kernel.

We used the following parameters:

- `C = 5`
- `gamma = 0.008`
- `epsilon = 0.1`

The RBF kernel allows the model to capture non-linear relationships between house characteristics and sale prices. We also used a preprocessing pipeline so that numerical and categorical features were handled consistently before being passed into the model.

## Repository Contents

- `Data_Bootcamp_Project_2_Final_Model.ipynb` – Jupyter notebook containing our data exploration, feature engineering, preprocessing, model training, evaluation, and final predictions.
- `README.md` – Project overview and instructions.

## How to Run

1. Clone or download this repository.
2. Download the Ames Housing training and test datasets from the Kaggle competition (also uploaded in this repository).
3. Open `Data_Bootcamp_Project_2_Final_Model.ipynb` in [Google Colab](https://colab.research.google.com/drive/1UkxLNm8RdaEXRvLdI9eBiZhW1HQny-VY?usp=sharing) or Jupyter Notebook.
4. Update the dataset file paths in the data loading cell to match your local files or Google Drive.
5. Run the notebook cells in order.
6. The final cells generate a CSV file containing the predicted house sale prices, ready for Kaggle submission.

## Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## What We Learned

This project gave us experience working through a complete machine learning workflow, from exploring and preparing a dataset to training and evaluating a regression model.

We learned how feature engineering and preprocessing can affect model performance, how to compare different regression approaches, and how to use RMSE to evaluate predictions. We also got hands-on experience preparing predictions for a Kaggle competition.

## Team Members

- Myra Rafiq
- Muhammad Abdullah
- Saudha Shaheen
