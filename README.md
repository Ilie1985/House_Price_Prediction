# 🏠 House Price Prediction with Multiple Linear Regression

This project uses a multiple linear regression model to predict house prices based on key features such as square footage, number of bedrooms, bathrooms, and floors. It's ideal for demonstrating your understanding of real-world machine learning, data preparation, and model evaluation.

---

## 📂 Project Structure
```
house_price_prediction/
├── house_prices.csv                # Dataset
├── house_price_prediction.ipynb    # Jupyter Notebook with full analysis
├── README.md                       # Project overview and instructions
└── visuals/                        # Folder for saved plots and images
```

---

## 📌 Problem Statement
Predict the selling price of houses using features like:
- Square footage of living space (`sqft_living`)
- Number of bedrooms
- Number of bathrooms
- Number of floors

This is a **regression problem** solved using **multiple linear regression**.

---

## 🧠 Skills Demonstrated
- Data loading and exploration with `pandas`
- Feature selection and preprocessing
- Training a linear regression model with `scikit-learn`
- Model evaluation (R² Score, Mean Squared Error)
- Visualizing results with `matplotlib`
- Predicting custom values using a trained model
- Structuring and documenting a project for portfolio and GitHub

---

## ⚙️ How to Run the Project

### Requirements
Create a virtual environment (optional but recommended):
```bash
python -m venv venv
venv\Scripts\activate     # Windows
```

### Install dependencies
```bash
pip install -r requirements.txt
```

### Launch Jupyter Notebook
```bash
jupyter notebook
```
Then open `house_price_prediction.ipynb` to explore the project.

---

## 🔍 Example Prediction
Predicting price for:
- 2000 sqft
- 3 bedrooms
- 2 bathrooms
- 1 floor

The model outputs:
```
Predicted price: £517,666.39
```

---

## 📈 Visual Output
A scatter plot shows actual vs predicted prices to evaluate model performance:
- Blue dots: Real data
- Red dashed line: Perfect predictions

The closer the dots are to the line, the better the model performs.

---

## 💡 Future Improvements
- Add more features like location (zipcode), grade, or year built
- Try other models (Decision Trees, Random Forest)
- Add interactive UI using Streamlit or ipywidgets
- Perform cross-validation and grid search

---

## 📬 Recruiter Notes
This project shows:
- Practical use of regression
- Code organization and clarity
- Visual communication of results
- Ability to explain machine learning in simple terms

Ideal for roles in:
- Data Analysis
- Junior Data Science
- Python Development

---

## 👤 Author
Marian Ilie
- GitHub: [your-username](https://github.com/your-username)
- LinkedIn: [your-profile](https://linkedin.com/in/your-profile)

Feel free to clone the repo, run the notebook, and explore how data science can predict real-world outcomes!
