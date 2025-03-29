# ML Repo for FOSS WEEKEND

Click [My Collab Notebook](https://colab.research.google.com/drive/1Am1pOJunGHBPTPW6uUZgm54FmbIkpy1Q?usp=sharing) to get my notebook on data cleaning.
# Data Cleaning and Preprocessing for Wine Dataset

## Prerequisites
To make the most out of this tutorial, you should have a basic understanding of programming concepts and some experience with Python.

## What To Do
Tasks and updates to this repository are managed through issues. If you have any suggestions, ideas, or find any issues, please check the issues tab. If you don't find your concern listed, feel free to open a new issue.

## Data Cleaning Process

The following methods were implemented to clean and preprocess the wine dataset for machine learning tasks:

### 1. **Handling Missing Data**
   - **Method:** `df.dropna()` or `df.fillna()`
   - **Description:** Missing values in the dataset were handled by either removing rows with missing values or filling them using a specified strategy (like mean or median for numerical features).
   
### 2. **Handling Duplicates**
   - **Method:** `df.drop_duplicates()`
   - **Description:** Duplicate rows were removed to ensure that no redundant data was used in the model.

### 3. **Data Type Conversion**
   - **Method:** `df.astype()`
   - **Description:** Some columns were converted to appropriate data types (e.g., 'year' as integer, 'price' as float).

### 4. **Outlier Detection and Removal**
   - **Method:** Z-Score or IQR
   - **Description:** Outliers were detected using Z-Score or the Interquartile Range (IQR) method and removed to improve model performance.

### 5. **Feature Scaling**
   - **Method:** `StandardScaler()` or `MinMaxScaler()`
   - **Description:** Features like 'rating', 'num_reviews', 'price', etc., were scaled to a standard range for better model performance.

### 6. **Handling Categorical Variables**
   - **Method:** `LabelEncoder()` and `OneHotEncoder()`
   - **Description:** Categorical variables were encoded into numerical values using label encoding or one-hot encoding.

### 7. **Feature Engineering**
   - **Method:** Custom calculations like `wine_age` and `rating_per_dollar`.
   - **Description:** New features were engineered like 'wine_age' based on the 'year' column and 'rating_per_dollar' to give more context for the model.

### 8. **Saving the Cleaned Data**
   - **Method:** `df.to_csv()`
   - **Description:** After cleaning and preprocessing, the data was saved as a CSV file (`cleaned_wine_data.csv`) for future use.

---



