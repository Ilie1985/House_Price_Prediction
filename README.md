# House Price Prediction Project

This repository demonstrates a simple machine learning workflow for predicting house prices using **multiple linear regression**. The data comes from the popular [King County House Sales dataset](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction), which contains over 21,000 records of home sales.

The goal is to predict a house's sale price based on a few key features.

## Repository Contents

- `house_prices.csv` – the dataset used for training and testing the model
- `House_Pricing_Prediction.ipynb` – Jupyter notebook with all the code
- `requirements.txt` – list of Python packages needed to run the notebook

## Dataset Overview

Each record in the dataset includes the sale price and attributes of a house such as:

- `bedrooms` – number of bedrooms
- `bathrooms` – number of bathrooms
- `sqft_living` – square footage of the living space
- `sqft_lot` – total square footage of the property
- `floors` – number of floors
- `waterfront`, `view`, `condition`, `grade` – categorical quality indicators
- `sqft_above` and `sqft_basement` – living area split between above ground and basement
- `yr_built` and `yr_renovated` – year built and year renovated if applicable
- `zipcode`, `lat`, and `long` – location information

For simplicity, the notebook focuses on four numerical predictors: `sqft_living`, `bedrooms`, `bathrooms`, and `floors`.

## How the Notebook Works

1. **Load the Data** – The CSV file is read with `pandas`.
2. **Clean and Select Features** – Rows with missing data in the selected columns are dropped.
3. **Train the Model** – A `LinearRegression` model from `scikit‑learn` is fitted on the chosen features.
4. **Evaluate** – The notebook prints the R² score and mean squared error to measure performance.
5. **Predict** – A helper cell demonstrates how to pass custom values to the model and get a predicted price.
6. **Visualization** – A scatter plot compares actual prices with predicted values.

## Running the Notebook

1. (Optional) create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Start Jupyter:
   ```bash
   jupyter notebook
   ```
   Open `House_Pricing_Prediction.ipynb` and run the cells in order.

## Example Output

After training, you should see output similar to:

```
R² Score: 0.51
Mean Squared Error: 66,455,438,852
Predicted price: £517,666.39
```

The scatter plot of actual vs. predicted prices gives a quick visual check of model performance – points close to the diagonal line indicate better predictions.

## Possible Extensions

- Include more features from the dataset, such as location or quality grade
- Experiment with other algorithms (e.g., Decision Trees, Random Forests)
- Perform cross‑validation or hyperparameter tuning
- Build a simple UI with Streamlit to allow interactive predictions

## Author

Marian Ilie

Feel free to fork the project and explore how a basic regression approach can be used to model real estate prices.
