# 🏠 House Price Prediction

This project predicts house sale prices using machine learning. It is based on the popular Kaggle competition **"House Prices - Advanced Regression Techniques"**, which uses real housing data from Ames, Iowa.

The goal is simple: given information about a house (like its size, quality, location, and condition), predict how much it will sell for.

## 📊 About the Dataset

- The dataset has **1460 training rows** and **1459 test rows**, with **80+ features** describing each house.
- Features include things like lot size, number of rooms, year built, basement quality, garage size, and overall condition.
- Target column: **SalePrice** (the price the house sold for).
- Dataset source: [Kaggle - House Prices Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)

## 🔍 Project Workflow

1. **Data Loading** — Loaded the train and test CSV files using pandas.
2. **Exploratory Data Analysis (EDA)** — Explored the data using plots and statistics to understand patterns, distributions, and outliers (including a look at the SalePrice distribution with mean and standard deviation).
3. **Data Preprocessing** — Handled categorical columns using Label Encoding, and prepared the data so it could be fed into machine learning models.
4. **Model Training** — Trained and compared several regression models to see which one predicts prices best.
5. **Model Evaluation** — Used 10-fold cross-validation and R² score to fairly compare each model's performance.

## 🤖 Models Compared

| Model | R² Score |
|---|---|
| **Gradient Boosting Regressor** | **0.880** ✅ Best |
| Random Forest Regressor | 0.848 |
| XGBoost Regressor | 0.846 |
| Decision Tree Regressor | 0.711 |

**Gradient Boosting Regressor** gave the best results, so it was chosen as the main model for this problem.

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** pandas, numpy, scikit-learn, XGBoost, seaborn, matplotlib

## ▶️ How to Run

1. Clone this repository.
2. Install the required libraries:
3. Open `house_price_predict.ipynb` in Jupyter Notebook.
4. Update the dataset file paths to match your local `train.csv` and `test.csv` location.
5. Run the notebook cell by cell.

## 🚀 Future Improvements

- Hyperparameter tuning (e.g. GridSearchCV) to push the Gradient Boosting model's accuracy even higher.
- Feature engineering (combining related features like total square footage or total bathrooms).
- Trying stacking/ensemble methods that combine multiple models together.

## 🙋 Author

Muhammad Irfan Shahid
