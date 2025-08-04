My First Machine Learning Project: Predicting House Prices!
Hey there! This is my first real dive into the world of machine learning. I decided to build a simple project from scratch to figure out how all this stuff actually works. The goal? To see if I could teach a computer to predict house prices in California.

It was a fun learning experience, and I've documented all my steps here.

# Dataset
The model is trained on the California Housing dataset, sourced from the 1990 California census. This dataset is included within the scikit-learn library.

1. Features (Independent Variables): The model utilizes 8 numerical features, including Median Income, House Age, Average Rooms, and geographic location (Latitude/Longitude).

2. Target (Dependent Variable): The objective is to predict the median house value, which is a continuous numerical target.

# Technologies and Libraries
Language: Python

#  Libraries:

scikit-learn for machine learning algorithms and data processing.

pandas for data manipulation and analysis.

jupyterlab for interactive development and demonstration.

matplotlib for data visualization.

# Methodology
Data Loading: The dataset was loaded directly from sklearn.datasets.

Data Preprocessing: The data was partitioned into features (X) and the target variable (y). Subsequently, it was split into an 80% training set and a 20% testing set to ensure unbiased model evaluation.

Model Training: A LinearRegression model was instantiated and trained on the training data using the .fit() method.

Model Evaluation: The trained model's performance was assessed on the unseen test set using standard regression metrics.

# Results
The model's performance was evaluated based on the following metrics:

Mean Squared Error (MSE): 0.56

This metric indicates the average of the squares of the errors between predicted and actual values. A lower value is preferable.

R-squared (R2) Score: 0.57

This score represents the proportion of the variance in the dependent variable that is predictable from the independent variables. An R 
2 of 0.57 signifies that the model accounts for 57% of the price variability.

# Instructions to run the project

1. Set Up Environment: It is recommended to use a virtual environment.
python -m venv venv
source venv/bin/activate  # On macOS/Linux
venv\Scripts\activate  # On Windows

2. Install Dependencies: Install the requirements.txt using pip
pip install -r requirements.txt

3. Run Notebook: Launch JupyterLab and open the project notebook.
jupyter-lab


