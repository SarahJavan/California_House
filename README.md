# California Housing Price Prediction
Overview

This project explores the California Housing dataset and applies a Machine Learning approach to predict house prices using Linear Regression.

The workflow includes data exploration, data cleaning, feature selection based on correlation analysis, model training, and performance evaluation using Mean Squared Error (MSE).

Dataset

The dataset contains information about housing districts in California, including:

Income
House Age
Number of Rooms
Number of Bedrooms
Population
Average Occupancy
Latitude
Longitude
House Price (Target Variable)
Project Workflow
1. Data Exploration

The dataset was inspected using:

head()
describe()
shape
Missing value analysis
2. Data Cleaning

Missing values were identified and removed to ensure data quality before model training.

3. Exploratory Data Analysis (EDA)

Several visualizations were created:

House price distribution
Correlation matrix
Heatmap of numerical features
Scatter plots for important variables

These analyses helped reveal relationships between housing attributes and house prices.

4. Feature Selection

Correlation analysis was used to identify the most influential predictors of house prices.

Top features selected:

Income
Latitude
Rooms

These variables showed the strongest correlation with the target variable (Price).

5. Model Training

A Linear Regression model from Scikit-Learn was trained using the selected features.

from sklearn.linear_model import LinearRegression

model = LinearRegression()
model.fit(X_train, y_train)
6. Model Evaluation

Model performance was evaluated using Mean Squared Error (MSE):

from sklearn.metrics import mean_squared_error

mse = mean_squared_error(y_test, y_pred)

### The MSE metric measures the average squared difference between actual and predicted house prices.

Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-Learn
Jupyter Notebook
Key Learning Outcomes

Through this project I gained practical experience in:

Data preprocessing
Exploratory Data Analysis (EDA)
Correlation analysis
Feature selection
Linear Regression modeling
Model evaluation using MSE
Data visualization
Repository Structure
├── House.csv
├── regression_shirafkan.ipynb
└── README.md
Future Improvements

Possible enhancements for this project include:

Feature engineering
Cross-validation
Hyperparameter tuning
Comparison with advanced regression models such as:
Random Forest Regressor
XGBoost Regressor
Gradient Boosting Regressor
Author

Sara JavanAmoli

Data Analysis | Machine Learning | Digital Humanism Research

#### Acknowledgment

Throughout my academic and professional journey, I have had the privilege of learning from many outstanding professors and mentors. Many of them taught me how to work with data, analyze information, and understand patterns. However, Dr. Farshid Shirafkan taught me something deeper: how to immerse myself in data.

While others showed me how to communicate with data, he taught me how to think through data, question assumptions, explore hidden relationships, and discover the stories that data can tell. His approach transformed data analysis from a technical task into an intellectual journey of exploration and insight.

This project reflects not only the technical skills I have learned, but also the mindset of curiosity and deep analytical thinking that I developed under his guidance.

I sincerely thank Dr. Farshid Shirafkan for his mentorship, inspiration, and dedication to teaching.

LinkedIn: @Dr. Farshid Shirafkan
