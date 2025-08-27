# Housing Price Prediction Model

This repository contains a Jupyter Notebook (`Housing.ipynb`) for predicting housing prices using various regression techniques and data preprocessing methods. The notebook demonstrates a complete workflow—from loading the dataset, performing exploratory data analysis (EDA), feature engineering, encoding categorical variables, to training and evaluating a regression model.

## Overview

The notebook covers the following steps:

1. **Data Loading & Exploration**
   - Loads housing data from `Housing.csv`.
   - Displays the first few rows to understand the features.

2. **Exploratory Data Analysis (EDA)**
   - Visualizes numerical features (`area`, `bedrooms`, `stories`, `parking`) using boxplots to identify outliers.
   - Shows distribution of features with histograms.
   - Displays a correlation matrix heatmap to understand relationships between variables.

3. **Data Preprocessing**
   - One-hot encodes categorical variables: `mainroad`, `furnishingstatus`, `guestroom`, `hotwaterheating`, `prefarea`, `basement`, `airconditioning`.
   - Feature engineering: creates new features such as `total_rooms`, `price_per_sqft`, and `area_air`.

4. **Model Preparation**
   - Splits the data into features (`X`) and target (`Y` - price).
   - Applies polynomial feature transformation for regression.
   - Splits the dataset into training and test sets.
   - Scales the features using `StandardScaler`.

5. **Model Training & Evaluation**
   - Trains a `LinearRegression` model on polynomial features.
   - Evaluates the model using metrics like Mean Squared Error (MSE), R² score, and Mean Absolute Error.

## Usage

1. **Clone the Repository**
   ```bash
   git clone https://github.com/AryanG111/-Housing-Price-Prediction-Model.git
   cd -Housing-Price-Prediction-Model
   ```

2. **Open the Notebook**
   - Make sure you have Jupyter Notebook installed.
   - Open `Housing.ipynb` in JupyterLab or Jupyter Notebook:
     ```bash
     jupyter notebook Housing.ipynb
     ```

3. **Install Dependencies**
   - The notebook uses the following Python libraries:
     - pandas
     - seaborn
     - matplotlib
     - numpy
     - scikit-learn

   - Install missing dependencies:
     ```bash
     pip install pandas seaborn matplotlib numpy scikit-learn
     ```

4. **Run the Notebook**
   - Step through the cells in order to reproduce the analysis and results.

## File Description

- `Housing.ipynb`: Main notebook containing code for EDA, preprocessing, feature engineering, modeling, and evaluation.
- `Housing.csv`: The dataset used for training and testing the model (make sure this file is in the project directory).

## Features Used

- **Numerical:** `area`, `bedrooms`, `bathrooms`, `stories`, `parking`
- **Categorical:** `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `prefarea`, `furnishingstatus`
- **Engineered:** `total_rooms`, `price_per_sqft`, `area_air`

## Model

- Polynomial Regression using `LinearRegression` from scikit-learn.
- Feature scaling and train-test splitting included.

## Visualization

- Boxplots and histograms for feature distribution.
- Heatmap for feature correlation.

## License

This project is for educational purposes.

## Author

- AryanG111

---

Feel free to open issues or submit pull requests for improvements!
