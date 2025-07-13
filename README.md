# CCUS Cost Estimator – Machine Learning Model

This repository contains a machine learning regression model that predicts the **cost per tonne of CO₂ captured (in USD)** from real-world CCUS project attributes.

---

## 📊 Project Overview

* **Goal**: Estimate the cost of CO₂ capture per tonne based on project features.
* **Model Type**: Regression
* **Performance**: R² score ≈ 0.99
* **Tools Used**: Python, Jupyter Notebook, scikit-learn, pandas, seaborn

---

## 📈 Dataset Description

The dataset includes project information from various CCUS initiatives:

| Feature                       | Description                                    |
| ----------------------------- | ---------------------------------------------- |
| Capture Technology            | Type of CO₂ capture technology used            |
| Combustion/Separation         | Capture process category                       |
| Country Location              | Location of the project                        |
| Storage and/or Capture        | Whether the project focuses on storage/capture |
| Amount of CO₂ Captured/Stored | Daily CO₂ capture in tonnes                    |
| Project Cost                  | Total cost in local currency                   |
| Currency                      | Type of currency (e.g., USD, EUR, etc.)        |

The dataset was preprocessed by:

* Mapping currency values to exchange rates
* Creating a new column: `cost_usd_per_tonne`
* Encoding categorical features using `pd.get_dummies()`

---

## ⚖️ Workflow

1. **Exploratory Data Analysis (EDA)**
2. **Preprocessing**

   * Handle currencies and conversions
   * Encode categorical data
   * Create input-output split
3. **Model Training**

   * Linear Regression
   * Evaluation using R² score and prediction plots
4. **Visualization**

   * Scatter plot of actual vs predicted cost per tonne

---

## 📁 Repository Structure

```bash
ccus-cost-estimator/
|
├── data/                       # CSV file containing CCUS data
├── notebooks/
│   └── ccus_model_build.ipynb # Main Jupyter Notebook
├── README.md                  # Project documentation
```

---

## 🚀 Getting Started

1. Clone the repository
2. Open the notebook in Jupyter Lab / Jupyter Notebook
3. Run the notebook step-by-step
4. Modify or extend with different models like SVM or KNN if desired

```bash
pip install -r requirements.txt
jupyter notebook notebooks/ccus_model_build.ipynb
```

---

## 📊 Model Output

The trained model gives highly accurate cost predictions:

* R² Score: \~0.99
* Scatter plot of actual vs predicted cost values

---

## 👨‍💼 Author

Created by a B.Tech Petroleum Engineering student passionate about machine learning, CCUS, and sustainability.

---

## 📄 License

This project is licensed under the MIT License. See the LICENSE file for details.

---

Feel free to star the repo ⭐ and contribute or suggest improvements!
