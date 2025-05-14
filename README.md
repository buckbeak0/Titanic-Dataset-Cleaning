# 🛳 Cleaning the Titanic Dataset

## 📖 Overview

This project focuses on cleaning and preprocessing the Titanic dataset to prepare it for exploratory data analysis and machine learning modeling. The dataset, sourced from Kaggle, contains information about passengers aboard the Titanic, including demographics and survival status.

## 🧰 Tools & Libraries

- **Python 3.x**: Core programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical operations
- **Jupyter Notebook**: Interactive coding environment

## 🧹 Data Cleaning Steps

1. **Loading the Dataset**: Imported the dataset using `pandas.read_csv()`.

2. **Exploratory Data Analysis**:
   - Utilized `df.info()` and `df.describe()` to understand data structure and summary statistics.
   - Identified missing values and data types.

3. **Handling Missing Values**:
   - **Age**: Filled missing values with the median age.
   - **Embarked**: Filled missing values with the mode.
   - **Fare**: Filled missing values with the median fare.

4. **Dropping Irrelevant Features**:
   - Removed `Cabin`, `Ticket`, and `Name` columns due to high missing values or irrelevance to the analysis.

5. **Encoding Categorical Variables**:
   - Converted `Sex` to numerical values: male = 0, female = 1.
   - Converted `Embarked` to numerical values: S = 0, C = 1, Q = 2.

6. **Feature Engineering**:
   - Created `FamilySize` by combining `SibSp` and `Parch`.
   - Created `IsAlone` feature: 1 if alone, 0 otherwise.

7. **Saving the Cleaned Data**:
   - Exported the cleaned dataset to `titanic_cleaned.csv` using `df.to_csv()`.


## 🚀 Getting Started

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/titanic-data-cleaning.git
   cd titanic-data-cleaning
   ```

2. **Install dependencies**:
   ```bash
   pip install pandas numpy jupyter
   ```

3. **Run the notebook**:
   ```bash
   jupyter notebook Titanic_Cleaning_Notebook.ipynb
   ```
