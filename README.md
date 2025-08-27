Housing Price Prediction Model

This project is an end-to-end data science pipeline that builds and evaluates a machine learning model to predict housing prices. The analysis is performed in a Jupyter Notebook, demonstrating key skills in data cleaning, exploratory data analysis (EDA), feature engineering, and model evaluation.
Dataset

The dataset used in this project is from the Housing.csv file. It contains various features related to residential properties, including:

    Continuous variables: price, area, bedrooms, bathrooms, stories, parking

    Categorical variables: mainroad, guestroom, basement, hotwaterheating, airconditioning, prefarea, furnishingstatus

Project Workflow

    Data Loading & Initial Exploration: The project begins by loading the dataset into a Pandas DataFrame and performing initial checks to understand its structure and content.

    Data Preprocessing:

        One-Hot Encoding: Categorical features (e.g., mainroad, furnishingstatus) are converted into numerical format using pd.get_dummies().
        
        Feature Engineering: New, more informative features are created from the existing data, such as total_rooms and price_per_sqft. This step enhances the predictive power of the model.

    Model Training:
        
        The data is split into training and testing sets to ensure the model is evaluated on unseen data.

        The Training data is fitted to poloynomial regression to get more inshights and increase the model accuracy
        
        A Linear Regression model from Scikit-learn is trained on the prepared data.

    Model Evaluation: The performance of the trained model is assessed using standard regression metrics:

        Mean Absolute Error (MAE): 407922.04

        Mean Squared Error (MSE): 312689084190.72

        Root Mean Squared Error (RMSE): 559186.09

        R-squared (R²): 0.93

Technologies Used

    Python

    Pandas: For data manipulation and analysis.

    NumPy: For numerical operations.

    Scikit-learn: For machine learning model building and evaluation.

    Seaborn & Matplotlib: For data visualization.

How to Run the Project

To run this project, you will need to have Python and the necessary libraries installed.

    Clone this repository to your local machine.

    Ensure you have the Housing.csv file in the same directory as the Jupyter Notebook.

    Open Housing.ipynb in a Jupyter Notebook environment.

    Run all cells to execute the entire analysis and see the results.
