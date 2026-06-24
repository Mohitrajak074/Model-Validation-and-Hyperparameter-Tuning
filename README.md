# 🏠 House Price Prediction using Model Validation & Hyperparameter Tuning

### Artificial Intelligence & Machine Learning Internship – Task 3

This project focuses on improving house price prediction using **model validation techniques, overfitting analysis, and hyperparameter tuning** on the **California Housing Dataset**.
The main goal of this task is to build a more reliable and optimized **Decision Tree Regressor** by applying **Cross-Validation** and **GridSearchCV**.

---

# 📖 Project Overview

In this project, a **Decision Tree Regressor** was trained as a baseline model for predicting house prices.
Its performance was analyzed on both training and testing data to identify **overfitting**.
To improve generalization and model reliability, **Cross-Validation** was applied, followed by **Hyperparameter Tuning** using **GridSearchCV**.

The tuned model was then evaluated and compared with the baseline model using **RMSE** and **R² Score**.

---

# 🎯 Objectives

* Load and explore the California Housing Dataset
* Train a baseline Decision Tree Regressor
* Detect overfitting using training and testing performance
* Apply **5-Fold Cross-Validation**
* Perform **Hyperparameter Tuning** using **GridSearchCV**
* Train the best optimized model
* Compare baseline and tuned model performance
* Visualize model behavior using multiple graphs

---

# 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

# 📊 Dataset Information

**Dataset Used:** California Housing Dataset (Scikit-Learn)

### Features

| Feature    | Description       |
| ---------- | ----------------- |
| MedInc     | Median Income     |
| HouseAge   | House Age         |
| AveRooms   | Average Rooms     |
| AveBedrms  | Average Bedrooms  |
| Population | Population        |
| AveOccup   | Average Occupancy |
| Latitude   | Latitude          |
| Longitude  | Longitude         |

### Target Variable

🏠 **Median House Price**

---

# 🤖 Model Used

## Decision Tree Regressor

A Decision Tree Regressor was used in this task because it can capture **non-linear relationships** and **feature interactions** more effectively than simple linear models.

Two versions of the model were evaluated:

### 1️⃣ Baseline Decision Tree

A default Decision Tree model trained without hyperparameter tuning.

### 2️⃣ Tuned Decision Tree

An optimized model obtained using **GridSearchCV** after testing multiple combinations of hyperparameters.

---

# ⚠️ Overfitting Analysis

To check whether the baseline model was overfitting, **Training R² Score** and **Testing R² Score** were compared.

* A very high training score with a lower testing score indicates **overfitting**
* This helps understand whether the model is memorizing training data instead of learning general patterns

---

# 🔁 Cross-Validation

To make model evaluation more reliable, **5-Fold Cross-Validation** was applied.

Cross-validation helps in:

* Evaluating model stability
* Reducing dependency on a single train-test split
* Estimating how well the model generalizes to unseen data

---

# ⚙️ Hyperparameter Tuning

**GridSearchCV** was used to search for the best combination of hyperparameters for the Decision Tree model.

### Hyperparameters Tuned

* `max_depth`
* `min_samples_split`
* `min_samples_leaf`

The best hyperparameter combination was selected based on **Cross-Validation R² Score**.

---

# 📈 Evaluation Metrics

The model was evaluated using:

### RMSE (Root Mean Squared Error)

Measures prediction error. Lower RMSE indicates better performance.

### R² Score

Measures how well the model explains variance in the target variable. Higher R² indicates better performance.

---

# 📝 Code Workflow

The notebook follows the following workflow:

### Step 1 – Import Libraries

Import all required Python libraries.

### Step 2 – Load Dataset

Load the California Housing Dataset and create a DataFrame.

### Step 3 – Data Exploration

* Dataset preview
* Statistical summary
* Missing value check
* Correlation analysis

### Step 4 – Train-Test Split

Split the data into training and testing sets.

### Step 5 – Baseline Model Training

Train a default Decision Tree Regressor.

### Step 6 – Overfitting Analysis

Compare training and testing performance of the baseline model.

### Step 7 – Cross-Validation

Apply 5-Fold Cross-Validation using `cross_val_score()`.

### Step 8 – Hyperparameter Tuning

Use `GridSearchCV()` to find the best hyperparameters.

### Step 9 – Tuned Model Training

Train the best Decision Tree model using optimized parameters.

### Step 10 – Final Evaluation

Calculate RMSE and R² Score for the tuned model.

### Step 11 – Visualization

Generate graphs for model analysis and performance comparison.

---

# 📸 Project Screenshots

## Dataset Preview
<img width="940" height="289" alt="Screenshot 2026-06-04 145521" src="https://github.com/user-attachments/assets/0f797784-5627-41c7-8d3d-96cd54550ebd" />



---

## Correlation Heatmap

![Heatmap](screenshots/heatmap.png)

---

## Overfitting Analysis

![Overfitting Analysis](screenshots/overfitting_analysis.png)

---

## Cross-Validation Scores

![Cross Validation](screenshots/cross_validation.png)

---

## Model Comparison (R² Score)

![Model Comparison](screenshots/model_comparison.png)

---

## RMSE Comparison

![RMSE Comparison](screenshots/rmse_comparison.png)

---

## Actual vs Predicted Values

![Actual vs Predicted](screenshots/actual_vs_predicted.png)

---

## Feature Importance

![Feature Importance](screenshots/feature_importance.png)

---

## Residual Plot

![Residual Plot](screenshots/residual_plot.png)



---

# 🏆 Results

| Model                  | RMSE               | R² Score            |
| ---------------------- | --------------     | --------------      |
| Baseline Decision Tree | 0.7037294974840077 |  0.622075845135081  |
| Tuned Decision Tree    | 0.6390654005312799 |  0.6883380738855668 |

### Best Model

🏅 Add the best model details after running the notebook.

---

# 📂 Project Structure

```text
House-Price-Prediction-Model-Tuning/
│
├── task3_model_tuning.ipynb
├── report.pdf
├── README.md
├── requirements.txt
│
└── screenshots/
    ├── dataset_preview.png
    ├── heatmap.png
    ├── overfitting_analysis.png
    ├── cross_validation.png
    ├── model_comparison.png
    ├── rmse_comparison.png
    ├── actual_vs_predicted.png
    ├── feature_importance.png
    ├── residual_plot.png
    └── validation_curve.png
```

---

# 🚀 How to Run

### Clone the Repository

```bash
git clone https://github.com/your-username/House-Price-Prediction-Model-Tuning.git
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

---

# 🔮 Future Improvements

* Try **Random Forest Regressor**
* Use **XGBoost Regressor**
* Apply **Advanced Feature Engineering**
* Perform **Model Ensembling**
* Compare multiple tuned algorithms

---

# 👨‍💻 Author

**Mohit Rajak**
B.Tech Computer Science & Engineering
Artificial Intelligence & Machine Learning Intern

---

⭐ If you found this project useful, consider giving it a star.
