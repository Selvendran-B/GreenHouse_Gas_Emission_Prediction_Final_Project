# GreenHouse_Gas_Emission_Prediction_Final_Project
# 🌍 Greenhouse Gas Emission Prediction – Week 3

This project focuses on predicting supply chain emission factors using a machine learning model. The goal is to help identify and analyze greenhouse gas (GHG) emissions based on substance, unit, and supply chain data.

---

## 🔍 Problem Statement

Predict the *Supply Chain Emission Factors with Margins* using other attributes in the dataset to assist with environmental analysis and sustainability decisions.

---

## 📁 Dataset Description

- *Rows:* 22,092 (approx.)
- *Key Columns:*
  - Code
  - Name
  - Substance
  - Unit
  - Supply Chain Emission Factors without Margins
  - Margins of Supply Chain Emission Factors
  - Supply Chain Emission Factors with Margins (Target)
  - DQ ReliabilityScore..., DQ TemporalCorrelation..., etc.

---

## 🛠️ Preprocessing Steps

- Removed duplicate entries
- Handled missing values:
  - *Numeric columns*: filled with mean
  - *Categorical columns*: filled with mode
- Encoded categorical columns using LabelEncoder
- Removed rows with invalid string entries in numeric columns
- Split data into training and testing sets (80/20 split)

---

## 🤖 Model Used

- *Random Forest Regressor* for regression task

### 🔧 Hyperparameter Tuning

Used *GridSearchCV* to optimize the following parameters:
- n_estimators: [50, 100]
- max_depth: [5, 10]
- (Extendable to min_samples_split, min_samples_leaf etc.)

---

## 📈 Evaluation Metrics

- *R² Score* – Measures how well predictions match the actual values  
- *Mean Squared Error (MSE)* – Penalizes larger errors more heavily

---

## 🧪 Results

After hyperparameter tuning, the optimized Random Forest model provides improved accuracy and stability on the test dataset.

---

## 💡 Future Scope

- Build a *Streamlit App* to make the model interactive for users
- Visualize predictions and feature importance
- Connect with real-time emission databases or APIs

---

## 📊 Visualization

- Distribution of the target variable
- (Optional) Feature importance plot, correlation heatmap, etc.

---

## ✅ Outcome

A complete machine learning pipeline was built with:
- Data cleaning
- Feature engineering
- Model training and tuning
- Evaluation

Ready to move to deployment or further analysis in Week 4.

---
