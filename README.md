# Simple Linear Regression: Sales & Advertising Analysis

A professional machine learning project implementing **Simple Linear Regression** from scratch using Python and Scikit-Learn to model the linear relationship between monthly advertising expenditures and product sales.

---

## 📌 Project Overview
The objective of this project is to investigate and forecast the linear dependency of sales performance based on advertising spend for a dietary weight control product[cite: 3]. The project follows a complete data science lifecycle, including Exploratory Data Analysis (EDA), data visualization, model training, evaluation via regression metrics, and residual diagnostics.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python[cite: 3]
* **Libraries:**
  * `NumPy`: For fast numerical array operations[cite: 3].
  * `Pandas`: For data manipulation and structural analysis[cite: 3].
  * `Scikit-Learn`: For building and evaluating the Linear Regression model[cite: 3].
  * `Matplotlib`: For visual exploratory data analysis and plotting regression lines[cite: 3].
  * `Joblib`: For model persistence and serialization.

---

## 📊 Methodology & Key Steps
1. **Data Loading & Preprocessing:** Imported monthly observations (36 rows) containing Sales and Advertising metrics[cite: 3].
2. **Exploratory Data Analysis (EDA):** Inspected data shapes, summary statistics, and verified missing values[cite: 3].
3. **Visual Data Exploration:** Generated scatter plots to study the linear association between input features ($X$) and target outcomes ($y$)[cite: 3].
4. **Train-Test Split:** Divided the dataset into a training set ($67\%$) and a test set ($33\%$) to validate generalization on unseen data[cite: 3].
5. **Model Training:** Fitted a `LinearRegression` model using the Ordinary Least Squares (OLS) method[cite: 3].
6. **Model Evaluation:**
   * Evaluated performance using **Root Mean Squared Error (RMSE)**[cite: 3].
   * Assessed goodness of fit via the **$R^2$ Score (Coefficient of Determination)**[cite: 3].
7. **Residual Analysis:** Inspected error distribution to check model assumptions and detect underfitting[cite: 3].

---

## 📈 Key Results & Performance
* **Estimated Linear Equation:** $\text{Advertising} = 1.6051 \times \text{Sales} - 11.1600$[cite: 3]
* **Root Mean Squared Error (RMSE):** $11.2273$[cite: 3]
* **$R^2$ Score Value:** $0.5789$ (Test set score)[cite: 3]
* **Inference:** The analysis confirms that a simple linear model provides an initial baseline, and future iterations can benefit from higher-complexity models (e.g., Polynomial Regression) to handle non-linear patterns[cite: 3].

---

## 🚀 Getting Started & Usage

### 1. Clone the Repository
Bash
git clone [https://github.com/Minahil-CS/SLRProject.git](https://github.com/Minahil-CS/Simple-Linear-Regression-Project.git)
cd SLRProject

### 2. Install Dependencies
Make sure you have an active Python environment with the required libraries installed:

Bash
pip install numpy pandas matplotlib scikit-learn joblib
### 3. Run the Jupyter Notebook
Open VS Code and launch the notebook to view execution steps:

Bash
jupyter notebook SLRProject.ipynb
💾 Model Persistence
The trained regressor model has been serialized and saved using joblib for rapid inference[cite: 3]:

Python
import joblib

### Load the saved model
model = joblib.load('lm_regressor.pkl')

### Make a prediction
prediction = model.predict([[24]])
print(prediction)

👩‍💻 Author
Minahil Fatima

BS Computer Science Student | AI & Machine Learning Enthusiast
```bash
git add README.md
git commit -m "Add professional README.md"
git push origin main
