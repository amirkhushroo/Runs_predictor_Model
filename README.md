🏏 IPL Runs Predictor using Machine Learning

A Machine Learning project that predicts the total runs scored by an IPL batter based on batting statistics from the IPL 2025 season. The project uses Linear Regression to learn the relationship between player performance metrics and total runs.

📌 Project Overview

This project demonstrates the complete Machine Learning workflow:

Loading the dataset
Data preprocessing
Handling missing values
Feature engineering
Training a Linear Regression model
Evaluating model performance
Predicting runs for individual players

The notebook is implemented in Python using Pandas, NumPy, and Scikit-learn.

📂 Project Structure
IPL-Runs-Predictor/
│
├── Run_predictor_model.ipynb      # Main Jupyter Notebook
├── IPL2025Batters.csv             # Dataset
├── README.md                      # Project Documentation
└── requirements.txt               # Python dependencies (optional)
📊 Dataset

The dataset contains batting statistics of IPL 2025 players.

Features Used
Matches
Innings
Not Outs
Highest Score
Balls Faced
Strike Rate
Centuries (100s)
Half Centuries (50s)
Fours
Sixes
Target Variable
Runs
🛠 Technologies Used
Python
Pandas
NumPy
Scikit-learn
Jupyter Notebook
📈 Machine Learning Algorithm

Linear Regression

The model predicts the number of runs scored by a player using multiple batting statistics.

⚙ Data Preprocessing

The following preprocessing steps were performed:

Loaded CSV dataset
Checked dataset information
Handled missing values
Removed/converted invalid values (e.g., "-" in AVG)
Converted numerical columns into proper numeric format
Processed Highest Score (HS) by removing the * symbol
Created a new feature:
HS_NotOut
🚀 Model Training

The dataset was divided into:

80% Training Data
20% Testing Data

The model was trained using:

LinearRegression()
📏 Model Evaluation

The model is evaluated using:

Mean Absolute Error (MAE)
Mean Squared Error (MSE)
R² Score

Example:

from sklearn.metrics import mean_absolute_error
from sklearn.metrics import mean_squared_error
from sklearn.metrics import r2_score
🎯 Prediction Example

The notebook predicts the runs for specific players such as:

Virat Kohli
Shubman Gill

Example:

prediction = model.predict(X_new)
print(prediction)
▶ How to Run
1. Clone the repository
git clone https://github.com/your-username/IPL-Runs-Predictor.git
2. Navigate to the project folder
cd IPL-Runs-Predictor
3. Install dependencies
pip install pandas numpy scikit-learn jupyter
4. Launch Jupyter Notebook
jupyter notebook
5. Open
Run_predictor_model.ipynb

Run all the cells sequentially.

📦 Requirements
Python 3.x
pandas
numpy
scikit-learn
jupyter
📌 Future Improvements
Use advanced regression algorithms such as:
Random Forest Regressor
XGBoost Regressor
Gradient Boosting
Hyperparameter tuning
Feature selection
Model deployment using Flask/FastAPI
Build a web interface with React
Predict future IPL season performance
📸 Sample Workflow
Dataset
   │
   ▼
Data Cleaning
   │
   ▼
Feature Selection
   │
   ▼
Train-Test Split
   │
   ▼
Linear Regression
   │
   ▼
Model Evaluation
   │
   ▼
Runs Prediction

👨‍💻 Author (Amir Khushroo)
B.Tech CSE (Data Science & AI)
