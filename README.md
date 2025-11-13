# California Housing Regression Assignment 🏡

## 📘 Objective

The goal of this assignment is to **apply multiple regression algorithms** to the **California Housing dataset** and compare their performance using standard evaluation metrics.

---

## 📊 Dataset

**Source:** `sklearn.datasets.fetch_california_housing`

The dataset contains information about various features of houses in California such as:

* Median Income
* House Age
* Average Rooms
* Average Bedrooms
* Population
* Average Occupancy
* Latitude
* Longitude

**Target Variable:** `MedHouseVal` — the median house value in each district.

---

## 🧩 Project Structure

```
📂 california-housing-regression
├── California_Housing_Regression_Assignment.ipynb   # Main Jupyter Notebook
├── README.md                                        # Project documentation (this file)
└── requirements.txt                                 # Python dependencies (optional)
```

---

## 🧠 Models Implemented

The following regression algorithms are trained and compared:

1. **Linear Regression** – Baseline linear model for simple relationships.
2. **Decision Tree Regressor** – Handles nonlinear relationships by splitting data into regions.
3. **Random Forest Regressor** – Ensemble of trees reducing overfitting.
4. **Gradient Boosting Regressor** – Boosting technique building trees sequentially to minimize errors.
5. **Support Vector Regressor (SVR)** – Uses kernel methods for high-dimensional regression.

Each model is trained, tested, and evaluated using the same train-test split for fairness.

---

## ⚙️ Preprocessing Steps

1. **Loaded** dataset with `fetch_california_housing()`.
2. **Checked for missing values** (none found).
3. **Scaled features** using `StandardScaler` for algorithms sensitive to feature magnitude (e.g., Linear Regression, SVR).
4. **Split** the dataset into 80% training and 20% testing.

---

## 📈 Evaluation Metrics

Each model is evaluated using:

* **Mean Squared Error (MSE)** – Penalizes large errors.
* **Mean Absolute Error (MAE)** – Average absolute prediction error.
* **R² Score** – Proportion of variance explained by the model.

Performance metrics are displayed in a comparison table and visualized with bar charts.

---

## 🥇 Results Summary

| Model             |     MSE ↓     |     MAE ↓     |         R² ↑    |
| :---------------- | -------------:| -------------:| -------------:  |
| Linear Regression |   0.555892    | 	0.533200    |     0.575788    |
| Decision Tree     |   ...     |       ... |  ... |
| Random Forest     |   ... |   ... |  ... |
| Gradient Boosting |   ... |   ... |  ... |
| SVR               |   ... |   ... |  ... |

> **Best Model:** Likely **Random Forest** or **Gradient Boosting**, due to their ensemble learning capability.

> **Worst Model:** Likely **Decision Tree**, due to overfitting and high variance.

---

## 🚀 How to Run

### 1. Clone this repository

```bash
git clone https://github.com/<your-username>/california-housing-regression.git
cd california-housing-regression
```

### 2. Create a virtual environment (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate  # (on macOS/Linux)
venv\Scripts\activate     # (on Windows)
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Then open `California_Housing_Regression_Assignment.ipynb` and run all cells.

---

## 📦 Requirements

Minimal dependencies:

```
numpy
pandas
scikit-learn
matplotlib
```

You can export them with:

```bash
pip freeze > requirements.txt
```

---

## ✨ Acknowledgments

Dataset provided by **Scikit-learn**.
Assignment designed to evaluate understanding of **supervised regression techniques**.

---

### 👩‍💻 Author

**Rishitha Raj**
Engineering Graduate | Project & Program Manager | Aspiring Data Scientist
