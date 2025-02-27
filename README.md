# 🏡 California Housing Price Prediction

## 📌 Overview
This project implements a **California Housing Price Prediction** model using **Linear Regression** and **Random Forest Regressor**. The dataset used is the **California Housing Dataset** from `sklearn.datasets`. The goal is to predict the median house prices based on various features such as income level, house age, and geographical location.

## 📂 Contents

### 1️⃣ Data Preparation (`Cellule 2 & 3`)
- **Dataset Loading**: The California Housing dataset is loaded using `fetch_california_housing(as_frame=True)`.
- **Feature Engineering**:
  ✅ Standardization of the dataset using `StandardScaler`.
  ✅ Splitting the data into **training (80%)** and **testing (20%)** sets.
  ✅ Checking dataset structure and statistics.

### 2️⃣ Model Training & Evaluation
#### 📊 **Linear Regression Model (`Cellule 4`)**
- **Model Training**:
  ✅ Uses **LinearRegression()** to fit the training data.
- **Predictions**:
  ✅ Predictions are made on the test set.
- **Evaluation Metrics**:
  ✅ **Mean Absolute Error (MAE)**: Measures the average absolute differences between predicted and actual prices.
  ✅ **Mean Squared Error (MSE)**: Penalizes large errors more significantly.

#### 🌲 **Random Forest Model (`Cellule 5`)**
- **Model Training**:
  ✅ Uses **RandomForestRegressor(n_estimators=100, random_state=42)**.
- **Predictions**:
  ✅ Predictions are made using the trained Random Forest model.
- **Evaluation Metrics**:
  ✅ **MSE, MAE, and R² score** are calculated to compare model performance.

## 🔬 Results & Observations
| Model  | Mean Squared Error (MSE) | Mean Absolute Error (MAE) | R² Score |
|--------|--------------------------|---------------------------|----------|
| Linear Regression | 0.55 | 0.53 | - |
| Random Forest | 0.26 | 0.33 | 0.81 |

**Conclusion**: The **Random Forest model outperforms Linear Regression** with a lower **MSE** and **MAE**, and a high **R² Score (0.81)**, indicating it captures more variance in the dataset.

## 🏗 Installation
To run this project, install the required dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib
```

## 🚀 Usage
1️⃣ Clone the repository:
```bash
git clone https://github.com/your-repo/California_Housing_Price_Prediction.git
cd California_Housing_Price_Prediction
```
2️⃣ Run the Python script in a Jupyter Notebook:
```python
jupyter notebook
```
3️⃣ Execute the cells step by step to see the data processing, model training, and evaluation.

## 🤝 Contributors
- **Code Crafters Bm** – Project development and implementation.


## 💡 Acknowledgments
- Inspired by `sklearn.datasets` and regression modeling techniques.


