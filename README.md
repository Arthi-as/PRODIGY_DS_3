# Decision Tree Classifier

A machine learning project that uses Decision Tree Classifier to predict bank customer deposit decisions based on various demographic and behavioral features.

## 📊 Project Overview

This project performs comprehensive exploratory data analysis (EDA) and builds predictive models using the Decision Tree algorithm to classify whether a bank customer will subscribe to a term deposit.

## 📁 Dataset

- **Source:** Bank Marketing Dataset (bank-task3.xlsx)
- **Features:** 20 demographic and behavioral attributes
- **Target Variable:** Deposit (yes/no)
- **Records:** 4521 rows

## 🔄 Project Workflow

### 1. **Data Loading & Exploration**
   - Load data from Excel file
   - Check data shape, columns, and data types
   - Identify missing values and duplicates

### 2. **Exploratory Data Analysis (EDA)**
   - Distribution analysis using histograms
   - Categorical features visualization with bar plots
   - Outlier detection with box plots
   - Correlation analysis

### 3. **Data Preprocessing**
   - Outlier removal using IQR method for numerical features (age, campaign, duration)
   - Feature selection by removing highly correlated columns (>0.90 correlation)
   - Label encoding for categorical variables

### 4. **Model Building**
   - Train-test split (75-25%)
   - **Model 1:** Decision Tree with Gini criterion (max_depth=5, min_samples_split=10)
   - **Model 2:** Decision Tree with Entropy criterion (max_depth=1, min_samples_split=15)

### 5. **Model Evaluation**
   - Accuracy Score
   - Confusion Matrix
   - Classification Report
   - Training vs Test Performance

## 📋 Features Used

**Numerical:** age, balance, day, duration, campaign, pdays, previous

**Categorical:** job, marital, education, default, housing, loan, contact, month, poutcome

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Matplotlib & Seaborn** - Data visualization
- **Scikit-learn** - Machine learning models
- **SciPy** - Statistical functions

## 🚀 How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Place the dataset file at: `D:/ARTHI/prodigy info tech/bank-task3.xlsx`

3. Run the notebook:
   ```bash
   jupyter notebook prodigy_task3.ipynb
   ```

4. Execute all cells to see:
   - EDA visualizations
   - Model training and evaluation
   - Decision tree visualizations

## 📈 Results

The project builds and compares two Decision Tree models with different hyperparameters and evaluation metrics including accuracy, confusion matrices, and classification reports.

## 📝 Files

- `prodigy_task3.ipynb` - Main notebook with full analysis and modeling
- `requirements.txt` - Python dependencies
- `README.md` - This file

## 🔧 Key Fixes Applied

- Fixed outlier removal logic using IQR method
- Fixed eval_model() function for proper confusion matrix calculation
- Safe column dropping to prevent KeyError

## ✨ Author

Created as part of Prodigy Info Tech Machine Learning tasks

## 📄 License

MIT License
