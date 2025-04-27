
# 🏡 Paris Housing Market Trends Analysis and Prediction

![Project Badge](https://img.shields.io/badge/Project-Paris%20Housing%20Market%20Analysis-blueviolet?style=flat-square)

This project analyzes the Paris housing market to uncover key drivers of property prices and builds a predictive model to estimate future price trends.  
By exploring housing features such as number of bedrooms, property grade, and living area, the study offers actionable insights for estate management and investment strategy.

---

## 🔍 Project Summary

We conducted a detailed exploratory analysis and predictive modeling using a Paris housing dataset (~20,000 properties).  
The primary objectives were:
- Investigate the relationship between **bedroom count** and **housing prices**.
- Study the impact of **floor count and total living area**.
- Build a reliable **price prediction model**.

Models evaluated:
- Linear Regression ✅ (Selected)
- Ridge Regression
- Lasso Regression
- Random Forest Regressor

---

## 📈 Model Performance Comparison

| Model              | MAE    | RMSE   | R²     |
|--------------------|--------|--------|--------|
| Linear Regression  | 0.2812 | 0.3492 | 0.5722 |
| Ridge (α=10.0)      | 0.2812 | 0.3492 | 0.5722 |
| Lasso (α=0.0001)    | 0.2812 | 0.3492 | 0.5722 |
| Random Forest       | 0.2931 | 0.3698 | 0.5202 |

✅ Linear Regression chosen for final deployment.

---

## 💡 Key Insights

- **Build Quality (Grade)** is the strongest predictor of price.
- **Living Space (Sqft_Living)** has a clear positive relationship with price.
- **Bedroom count** alone is a weak predictor unless accompanied by higher living space.
- Properties with superior **grade** outperform larger but lower-quality properties.

---

## 📊 Simulation Highlights

**Bedrooms vs Predicted Price** (Insert your plot here!)  
**Grade vs Predicted Price** (Insert your plot here!)  
**Sqft_Living vs Predicted Price** (Insert your plot here!)

### Combined Simulation: Grade vs Sqft_Living

| Sqft Living / Grade | 5     | 8     | 11    |
|---------------------|-------|-------|-------|
| 1000 sqft           | €229k | €418k | €764k |
| 2500 sqft           | €317k | €580k | €1.06M |
| 4000 sqft           | €440k | €803k | €1.47M |

**Interpretation**: Higher grade significantly boosts price more than just larger living area.

---

## 📢 Strategic Recommendations

- Prioritize **build quality upgrades** during renovations.
- Increase **usable living space** rather than simply adding rooms.
- Maintain a focus on **quality perception** over raw size.
- Use **linear models** for fast and effective future forecasting.
- Plan for long-term market shifts by analyzing build quality and design trends.

---

## 📦 Future Work

- Deploy model using **Streamlit** or **Flask** web apps.
- Integrate a **live prediction dashboard**.
- Extend analysis to include **temporal price trends** if transaction date data becomes available.

---

## 📄 References
- Kim, K., & Park, Y. (2016). Housing Quality and Price: A Cross-sectional Analysis. *Journal of Real Estate Research, 48*(2), 233-254.
- Goodman, A. C., & Thibodeau, T. G. (2003). Housing Market Segmentation and Hedonic Prediction Accuracy. *Real Estate Economics, 31*(2), 179-194.
- Bourassa, S. C., Cantoni, E., & Hoesli, M. (2007). Spatial Dependence, Housing Submarkets, and House Price Prediction. *Journal of Real Estate Finance and Economics, 35*(2), 143-160.
- Clapp, J. M., Dolde, W., & Todorov, A. (2002). Risk and House Price Dynamics: An International Comparison. *Journal of Housing Research, 13*(1), 1-20.
- Zietz, J., Zietz, E. N., & Sirmans, G. S. (2008). Determinants of House Prices: A Quantile Regression Approach. *Journal of Real Estate Finance and Economics, 37*(4), 317-333.
- Selim, S. (2009). Determinants of House Prices in Turkey: Hedonic Regression versus Artificial Neural Network. *Expert Systems with Applications, 36*(2), 2843-2852.

