# Laptop Price Prediction Model
This project is a Machine Learning application that predicts the price of a laptop based on various features like brand, processor type, RAM, storage, etc. It uses a regression model to estimate the laptop price based on the given input features. The application is built with Streamlit for the front end and supports real-time predictions.

## Table of Contents
Overview
Features
Tech Stack
Dataset
Model
Installation
Usage
Screenshots
Contributing
License
## Overview
The goal of this project is to predict the price of laptops based on several hardware and brand attributes. By training various machine learning models, we compare their performance and select the best one for predicting laptop prices. The web app built using Streamlit provides a simple and user-friendly interface for users to input the specifications and get an estimated price.

### Features
Predict laptop prices based on specifications.
Input features such as:
Brand
Processor Type
RAM size
Storage Type and Size
Screen Size, etc.
Compare different regression models and select the best one.
Streamlit web application for real-time predictions.
Tech Stack
## Programming Language: Python
### Libraries:
scikit-learn: For machine learning models
pandas: For data manipulation
numpy: For numerical computations
streamlit: For building the web application
matplotlib & seaborn: For data visualization
## Machine Learning Algorithms:
Linear Regression
Decision Tree
Random Forest
Gradient Boosting
Support Vector Machines (SVM)
Serialization: pickle, joblib (for saving the trained models)
Dataset
#### The dataset used for this project contains various laptop configurations and prices. The key features in the dataset include:

Brand: The manufacturer of the laptop (e.g., Dell, HP, Apple)
Processor Type: Type of processor (e.g., Intel Core i5, AMD Ryzen)
RAM Size: Size of RAM in GB
Storage Type and Size: SSD or HDD storage size
Screen Size: The diagonal size of the screen
GPU: The type of GPU included in the laptop
Operating System: The OS that comes pre-installed with the laptop
The target variable is the price of the laptop.

## Model
The model selection process involves testing several regression models and tuning their hyperparameters using GridSearchCV. The best-performing model is then saved and used for prediction in the web app.

### Models Used:
Linear Regression
Decision Tree Regressor
Random Forest Regressor
Gradient Boosting Regressor
Support Vector Regressor (SVR)
The final model is selected based on metrics like R² score and Mean Absolute Error (MAE).

#### Installation
Prerequisites:
Python 3.x
Streamlit
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/laptop-price-prediction.git
cd laptop-price-prediction
Create a virtual environment (optional but recommended):

bash
Copy code
python -m venv venv
source venv/bin/activate  # For Linux/macOS
.\venv\Scripts\activate   # For Windows
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Download the dataset and place it in the appropriate directory (if it's not already part of the repository).

Run the application:

bash
Copy code
streamlit run app.py
Usage
After running the Streamlit app, open your browser and go to http://localhost:8501.
Input the laptop specifications (Brand, Processor, RAM, etc.).
Click "Predict" to get the estimated laptop price.
Predicting New Laptop Prices:
The web interface allows users to easily input laptop specifications and receive a price prediction.
The predictions are based on the trained machine learning model that was saved using pickle.
Screenshots

Contributing
Contributions are welcome! Please fork this repository and create a pull request if you'd like to improve the project. You can also open an issue for suggestions or bugs.

### Steps to contribute:
Fork the repository
Create a new branch (git checkout -b feature-branch)
Make your changes and commit (git commit -m 'Add new feature')
Push to the branch (git push origin feature-branch)
Open a pull request
### License
This project is licensed under the MIT License - see the LICENSE file for details.
