# Project 01 – Synthetic Linear Regression with Pipeline

This project implements a **classic Machine Learning pipeline** using `scikit-learn` to solve a **simple linear regression** problem with a synthetic dataset generated using `make_regression`.

## 📌 Objectives
- Practice building **pipelines in sklearn**.
- Understand the full workflow of a classic ML project:
  1. Data generation and loading.
  2. Pipeline construction.
  3. Model training and evaluation.
  4. Results visualization.
- Interpret regression metrics: **MSE**, **RMSE**, and **R²**.

## 📂 Project Structure

proyecto_01_regresion_lineal_sintetica/
├── src/
│ ├── init.py
│ └── pipeline.py # Main functions: load_data, build_pipeline, train_and_evaluate
├── 01_pipeline_regresion.ipynb # Notebook for testing, visualization, and experiments
├── requirements.txt
├── .gitignore
└── README.md


## ⚙️ Main Functions

- **`load_data()`**  
  Generates a synthetic dataset with `make_regression` and splits it into train/test.

- **`build_pipeline()`**  
  Builds a pipeline with:
  - `StandardScaler` → normalizes the features.
  - `LinearRegression` → linear regression model.

- **`train_and_evaluate()`**  
  Trains the pipeline, makes predictions on the test set, and returns metrics:
  - **MSE**: Mean Squared Error.  
  - **RMSE**: Root Mean Squared Error (error in the same units as `y`).  
  - **R²**: Coefficient of determination, proportion of variance explained by the model.  

## 📊 Visualization
In the notebook, you will find:
- **Scatter plot** of the training data.  
- **Regression line** fitted by the model.  
- Model performance comparison with different noise levels (`noise`) in the dataset.

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/tu_usuario/proyecto_01_regresion_lineal_sintetica.git
   cd proyecto_01_regresion_lineal_sintetica
