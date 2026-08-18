# Machine Learning & Python Projects

This repository contains a collection of beginner-friendly Python and Machine Learning projects developed using **Jupyter Notebook**. The projects demonstrate data analysis, visualization, regression modeling, model evaluation, prediction, and basic Python programming.

## 📌 Projects Included

### 1. Salary Prediction using Simple Linear Regression

This project demonstrates how **Simple Linear Regression** can be used to predict an employee's salary based on their years of professional experience.

#### Objective

The objective is to understand the relationship between:

* **Independent Variable:** Years of Experience
* **Dependent Variable:** Salary

The project loads a salary dataset, performs basic data inspection and cleaning, visualizes the relationship between experience and salary, trains a Linear Regression model, evaluates the model, and visualizes the regression line.

#### Dataset

The salary dataset contains:

* `YearsExperience` — Number of years of professional experience
* `Salary` — Employee salary
* `Unnamed: 0` — An index column that is removed during preprocessing

The dataset contains **30 observations**.

#### Steps Performed

1. Import required Python libraries.
2. Load the salary dataset using Pandas.
3. Display the first few records.
4. Inspect the dataset using `df.info()`.
5. Generate descriptive statistics using `df.describe()`.
6. Remove the unnecessary `Unnamed: 0` column.
7. Check for missing values.
8. Visualize Years of Experience against Salary using a scatter plot.
9. Define the independent variable `X` and dependent variable `y`.
10. Train a `LinearRegression` model.
11. Calculate the regression intercept and slope.
12. Generate salary predictions.
13. Create a results table containing actual salary, predicted salary, and residuals.
14. Calculate Mean Squared Error (MSE).
15. Calculate Root Mean Squared Error (RMSE).
16. Visualize the actual salary values and regression line.

#### Model

The project uses the following linear regression equation:

**Salary = Intercept + Slope × YearsExperience**

The trained model produced:

* **Intercept:** 24,848.20
* **Slope:** 9,449.96
* **Mean Squared Error:** 31,270,951.72
* **Root Mean Squared Error:** 5,592.04

These values are based on the notebook's executed output.

---

### 2. House Price Prediction using Multiple Linear Regression

This project demonstrates **Multiple Linear Regression** for predicting house prices using multiple independent variables.

#### Objective

The objective is to predict the price of a house based on several characteristics of the property.

#### Features Used

The model uses the following input features:

| Feature            | Description                          |
| ------------------ | ------------------------------------ |
| `Area_sqft`        | Area of the house in square feet     |
| `Bedrooms`         | Number of bedrooms                   |
| `Age_years`        | Age of the house in years            |
| `Distance_City_km` | Distance from the city in kilometers |

#### Target Variable

The target variable is:

`House_Price_Lakhs`

This represents the house price in lakhs.

#### Steps Performed

1. Import Pandas and NumPy.
2. Import Matplotlib for visualization.
3. Import `train_test_split` for splitting the dataset.
4. Import `LinearRegression`.
5. Import evaluation metrics such as MSE and R² score.
6. Load the house price dataset.
7. Display the first 10 records.
8. Check the shape and information of the dataset.
9. Select the required independent variables.
10. Select house price as the target variable.
11. Split the dataset into training and testing sets.
12. Use 80% of the data for training and 20% for testing.
13. Train the Multiple Linear Regression model.
14. Display the model intercept.
15. Generate a coefficient table for each feature.
16. Predict house prices for the test dataset.
17. Compare actual prices with predicted prices.
18. Calculate Mean Squared Error.
19. Calculate Root Mean Squared Error.
20. Calculate R² score.
21. Visualize actual prices versus predicted prices.
22. Use the trained model to predict the price of a new house.

#### Train-Test Split

The dataset is divided using:

* **80% Training Data**
* **20% Testing Data**
* `random_state = 42`

#### Example Prediction

The notebook also demonstrates prediction for a new house with:

* Area: **1800 sq ft**
* Bedrooms: **3**
* Age: **5 years**
* Distance from city: **7 km**

The trained regression model is then used to estimate the house price in lakhs.

---

### 3. Python Calendar Program

This is a simple Python program that displays the calendar for a user-selected month and year.

#### Objective

The purpose of this program is to demonstrate:

* User input
* Type conversion
* Python's built-in `calendar` module
* Formatted output

#### How It Works

The program asks the user to enter:

1. Year
2. Month

It then uses Python's `calendar.month()` function to display the calendar for the selected month.

#### Example

```text
ENTER YEAR: 2026
ENTER MONTH: 8

     August 2026
Mo Tu We Th Fr Sa Su
             1  2
 3  4  5  6  7  8  9
10 11 12 13 14 15 16
17 18 19 20 21 22 23
24 25 26 27 28 29 30
31
```

---

# 🛠️ Technologies Used

The projects in this repository use the following technologies and Python libraries:

* **Python**
* **Jupyter Notebook**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Scikit-learn**
* **Python Calendar Module**

## 📚 Libraries

### Pandas

Used for:

* Loading datasets
* DataFrame creation
* Data inspection
* Data manipulation
* Creating prediction result tables

### NumPy

Used for:

* Numerical calculations
* Calculating RMSE from MSE
* Working with numerical data

### Matplotlib

Used for:

* Scatter plots
* Regression line visualization
* Actual vs predicted price visualization

### Scikit-learn

Used for Machine Learning tasks including:

* Linear Regression
* Train-test splitting
* Mean Squared Error
* R² Score

### Calendar

Python's built-in `calendar` module is used to generate monthly calendars.

---

# 📊 Machine Learning Concepts Demonstrated

This repository demonstrates several fundamental Machine Learning concepts.

## Simple Linear Regression

Simple Linear Regression predicts a dependent variable using one independent variable.

In this project:

```text
YearsExperience → Salary
```

The model attempts to find the best-fitting straight line through the data.

## Multiple Linear Regression

Multiple Linear Regression predicts a dependent variable using multiple independent variables.

In this project:

```text
Area_sqft
Bedrooms
Age_years
Distance_City_km
        ↓
House Price
```

The model learns how these variables contribute to house prices.

## Model Evaluation

The projects demonstrate common regression evaluation metrics:

### Mean Squared Error (MSE)

MSE measures the average squared difference between actual and predicted values.

Lower MSE generally indicates better prediction performance.

### Root Mean Squared Error (RMSE)

RMSE is the square root of MSE and provides an error value in the same unit as the target variable.

### R² Score

R² measures how much of the variation in the target variable is explained by the regression model.

A value closer to 1 generally indicates a stronger fit.

---

# 📈 Visualizations

The notebooks include visualizations such as:

### Salary vs Years of Experience

A scatter plot is used to visualize the relationship between years of experience and salary.

### Regression Line

The fitted linear regression line is plotted along with the actual salary observations.

### Actual vs Predicted House Prices

A scatter plot compares actual house prices with predicted prices.

A reference line is included to help visualize how closely predictions match actual values.

---

# 📁 Repository Structure

A recommended GitHub repository structure is:

```text
Machine-Learning-Python-Projects/
│
├── README.md
│
├── notebooks/
│   └── Untitled2.ipynb
│
├── datasets/
│   ├── Salary_dataset.csv
│   └── Multiple_Regression_HousePrice_Dataset.csv
│
└── .gitignore
```

If you don't want to create separate folders, you can also keep everything in the main repository:

```text
Machine-Learning-Python-Projects/
│
├── README.md
├── Untitled2.ipynb
├── Salary_dataset.csv
├── Multiple_Regression_HousePrice_Dataset.csv
└── .gitignore
```

---

# 🚀 How to Run the Projects

## 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

## 2. Open the Project Folder

```bash
cd Machine-Learning-Python-Projects
```

## 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

The `calendar` module is included with Python, so it does not need to be installed separately.

## 4. Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Untitled2.ipynb
```

and run the cells.

---

# ⚠️ Important Note About Dataset Paths

The notebook currently loads datasets using local Windows file paths such as:

```python
C:\Users\Abhay\Downloads\Salary_dataset.csv
```

and:

```python
C:\Users\Abhay\Downloads\Multiple_Regression_HousePrice_Dataset.csv
```

These paths will only work on the computer where those files exist.

For GitHub, it is recommended to place the CSV files inside a `datasets` folder and change the notebook paths to relative paths.

For example:

```python
df = pd.read_csv("datasets/Salary_dataset.csv")
```

and:

```python
df = pd.read_csv("datasets/Multiple_Regression_HousePrice_Dataset.csv")
```

This makes the notebook portable and allows other users to run it after cloning the repository.

---

# 🎯 Learning Objectives

After completing these projects, you can understand:

* How to load datasets using Pandas
* How to inspect datasets
* How to identify columns and data types
* How to check missing values
* How to remove unnecessary columns
* How to visualize relationships between variables
* How Simple Linear Regression works
* How Multiple Linear Regression works
* How to split data into training and testing sets
* How to train a Machine Learning model
* How to generate predictions
* How to calculate MSE
* How to calculate RMSE
* How to calculate R²
* How to visualize model predictions
* How to use a trained model for new predictions
* How to create a basic Python program using user input

---

# 💡 Future Improvements

The projects can be improved further by:

* Adding more datasets
* Performing detailed exploratory data analysis (EDA)
* Adding feature correlation analysis
* Creating train/test regression plots
* Adding R² score to the salary prediction project
* Performing cross-validation
* Comparing Linear Regression with other regression algorithms
* Adding data preprocessing pipelines
* Adding error/residual analysis
* Creating a user interface for predictions
* Deploying the Machine Learning model as a web application
* Adding detailed documentation for each individual project

---

# 👨‍💻 Author

**Abhay Chandel**

This repository was created as part of a learning journey in **Python, Data Analysis, and Machine Learning**.

---

# ⭐ Acknowledgement

This repository is intended for educational and learning purposes. It demonstrates fundamental Python programming and Machine Learning concepts using practical examples.

If you find this repository useful, consider giving it a ⭐ on GitHub.

---

# 📜 License

This project is available for educational purposes. You may modify and use the code for learning and experimentation.
