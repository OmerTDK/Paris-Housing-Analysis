# Paris Housing Market Analysis 🏘️

A predictive modeling project that explores and forecasts housing prices in Paris using Python and machine learning.

## 📌 Project Goal

To perform exploratory data analysis and build regression models to forecast potential housing price trends in Paris. The initial focus is on analyzing the impact of:

- Number of bedrooms
- Price
- Total square footage
- Number of floors

## 🔍 Dataset

- **Source:** `Paris_housing_Data_Set_2 [4050].csv`
- **Size:** 4,050 observations
- **Features:** Bedrooms, bathrooms, square footage (living + total), floors, grade, year built, renovation status, etc.

## ⚙️ Key Steps

1. **Data Cleaning**
   - Handled nulls
   - Capped outliers
   - Encoded categorical variables

2. **Feature Engineering**
   - Created log-transformed and scaled features
   - Built correlation heatmaps to select predictors

3. **Modeling**
   - Linear Regression
   - Ridge and Lasso Regression
   - Random Forest Regressor
   - Model Evaluation: MAE, RMSE, R²

4. **Simulations**
   - Price simulations varying bedrooms, grade, sqft_living
   - 3D simulations to see combined effect of grade + sqft

## 📈 Final Model

- Best model: **Ridge Regression (alpha=10.0)**
- R² Score: 0.5722
- MAE: 0.2812 (log-scaled)
- RMSE: 0.3492

## 📊 Key Insights

- `Grade`, `sqft_living`, and `bathrooms` were top predictors of price.
- Price increases sharply with grade and square footage.
- Log transformations helped normalize skewed data and improve model performance.

## 📦 Future Work

- Add deployment via Streamlit or Flask
- Integrate real-time prediction dashboard
- Include temporal trends if time data becomes available

---

## 💻 Tech Stack

- Python (Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib)
- Jupyter Notebook
- Git + GitHub for version control

---

## 📁 File Structure
📦 Paris Housing Analysis
├── Analysis.ipynb          # Main Jupyter notebook containing all analysis, modeling, and visualizations
├── Dataset.csv             # Cleaned and processed housing dataset
├── README.md               # Project documentation and summary (this file)
├── requirements.txt        # (Optional) Python dependencies used in the project
└── .git/                   # Git tracking folder
