# Holistic Health & Lifestyle Prediction 🧘‍♂️🥗

## 📌 Project Overview
This project analyzes a **Holistic Health and Lifestyle** dataset to understand how various daily habits contribute to an individual's overall health score. The primary focus of this notebook is to investigate the correlation between **Mindfulness** and **Overall Health Score** and to predict health outcomes using machine learning models.

The analysis compares the performance of a **Linear Regression** model against a **Random Forest Regressor** to determine which provides more accurate predictions.

## 📂 Dataset
The dataset (`holistic_health_lifestyle_dataset.csv`) contains **10,000 records** with the following lifestyle metrics:
* **Physical_Activity**: Activity level metric.
* **Nutrition_Score**: Quality of nutrition.
* **Stress_Level**: Reported stress levels.
* **Mindfulness**: Mindfulness practice score (Key feature used in modeling).
* **Sleep_Hours**: Daily sleep duration.
* **Hydration**: Daily water intake.
* **BMI**: Body Mass Index.
* **Alcohol**: Alcohol consumption metric.
* **Smoking**: Smoking habits.
* **Overall_Health_Score**: The target variable representing the calculated health score.
* **Health_Status**: Categorical status (e.g., Poor, Average, Good).

## 🚀 Workflow
1.  **Data Loading & Cleaning**: 
    * Importing the dataset using Pandas.
    * Checking for and dropping missing values to ensure data integrity.
2.  **Exploratory Data Analysis (EDA)**:
    * Generating descriptive statistics (`.describe()`).
    * Visualizing correlations using a **Seaborn Heatmap** to identify relationships between variables.
    * *Key Finding*: Mindfulness was identified as a significant factor correlated with the target variable.
3.  **Data Preprocessing**:
    * Splitting the data into training (80%) and testing (20%) sets.
4.  **Machine Learning Models**:
    * **Linear Regression**: Implemented as a baseline model.
    * **Random Forest Regression**: Implemented to capture non-linear relationships.
5.  **Evaluation & Visualization**:
    * Calculating model scores for both training and test sets.
    * Visualizing actual vs. predicted values using Matplotlib scatter plots.

## 📊 Results & Conclusion
The analysis compared two models to predict the `Overall_Health_Score`:

* **Linear Regression**: Showed limited performance, indicating that the relationship between Mindfulness and Health Score might not be purely linear.
* **Random Forest**: Outperformed the Linear Regression model, providing better visualization and higher accuracy on both training and test sets.

**Conclusion**: The **Random Forest Regression model** is recommended for this specific prediction task due to its superior scoring and ability to handle the data distribution better than the linear approach.

## 🛠️ Technologies Used
* **Python**
* **Pandas** (Data Manipulation)
* **NumPy** (Numerical Computations)
* **Matplotlib & Seaborn** (Data Visualization)
* **Scikit-Learn** (Machine Learning)

## 🔧 How to Run
1.  Clone this repository.
2.  Install the required libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
3.  Open the Jupyter Notebook `Earthquake-Tsunami-Prediction.ipynb`.
4.  Ensure the dataset is located in the correct path (or update the path in the code) and run the cells.

---
*Created for the GC NPA AI 2025 course.*
