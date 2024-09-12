# House Prices - Advanced Regression Techniques (Kaggle)

This repository contains an exploratory data analysis (EDA) and feature engineering process for a house price prediction dataset. The goal of this project is to predict the final sale price of homes based on various features using machine learning models. This project is based on a Kaggle competition dataset.

Dataset
The dataset used in this project can be found on Kaggle's House Prices Competition. The dataset consists of 81 columns and 1460 rows, with features describing different attributes of houses (such as square footage, neighborhood, number of rooms, etc.) and the target variable SalePrice, which represents the house sale price.

Libraries Used
The following Python libraries are used in this analysis:

NumPy: For numerical computing.

Pandas: For data manipulation and analysis.

Seaborn: For data visualization.

Matplotlib: For creating plots and graphs.

SciPy: For statistical functions.

Stats: For fitting normal distributions.

Project Steps

1. Importing Libraries
The necessary libraries are imported for data analysis, visualization, and handling statistical computations.


2. Loading Dataset
The dataset is loaded from a CSV file (train.csv) using pandas.read_csv() and basic exploration is performed using head() and info().


3. Shape and Structure of Data
We first inspect the data to check the number of rows and columns, and then print the structure of the data with info() to observe the data types and missing values.


4. Data Cleaning
Missing data is handled by dropping columns with high missing values using the drop_col list.


5. Distribution of Target Variable (SalePrice)
A distribution plot (dist plot) is used to check if the target variable, SalePrice, follows a normal distribution. Since the distribution is skewed, a log transformation is applied to make it more normally distributed.


6. Detecting Missing Values
Missing values are identified using isnull() and displayed as a percentage of the total dataset. The missing values are visualized using a bar plot.


7. Correlation Analysis
The dataset is reduced to only numerical columns for correlation analysis. A correlation matrix is generated to identify the relationship between features and the target variable, SalePrice.


How to Run the Code
Clone the repository:
git clone https://github.com/your-username/house-prices-regression.git

Install the necessary Python libraries:
pip install -r requirements.txt

Load the dataset by placing the train.csv file in the root directory.
Run the Python script.

Outputs
Data Visualization: Various graphs and distribution plots are created using Seaborn and Matplotlib to gain insights into the data.
Missing Values Handling: Missing data is visualized and handled effectively.
Target Variable Normalization: The SalePrice target variable is transformed using a log function to better fit a normal distribution.

Notes
The distplot function from Seaborn is deprecated. The code includes warnings suggesting the use of displot or histplot for future compatibility.
