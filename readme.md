Here's a more concise and professional rewrite of your project with the author's name updated to Ayush Tripathi:

---

# Employee Productivity Prediction Using Machine Learning

A web-based solution utilizing machine learning to predict the productivity of garment factory workers, based on various operational factors.

![Home Page](https://github.com/ayushtripathi1025/Employee-Performance-Prediction/blob/master/Code%20Screenshots/Screenshot%202025-08-13%20003231.png)

---

### Table of Contents

1. [Abstract](#1-abstract)
2. [Project Objective](#2-project-objective)
3. [Technology Stack](#3-technology-stack)
4. [Application Screenshots](#4-application-screenshots)
5. [Machine Learning Workflow](#5-machine-learning-workflow)
6. [Installation & Setup](#6-installation-and-setup)
7. [Project Structure](#7-project-structure)
8. [Conclusion](#8-conclusion)

---

### 1. Abstract

This project develops a predictive system to assess the productivity of garment workers, using machine learning algorithms. By analyzing factors like team performance, goals, and incentives, a prediction model is built and deployed as a web application using Flask. This tool helps managers make data-driven decisions in resource allocation and workforce optimization, improving overall productivity.

---

### 2. Project Objective

Key goals of this project:

* Conduct exploratory data analysis (EDA) on the dataset to uncover insights.
* Preprocess and clean the data for machine learning.
* Train and evaluate regression models to predict productivity.
* Deploy the best-performing model in a web application for real-time predictions.

---

### 3. Technology Stack

* **Language:** Python 3.x
* **Libraries:** Flask, Scikit-learn, XGBoost, Pandas, NumPy, Matplotlib, Seaborn
* **Development Environment:** Jupyter Notebook, Visual Studio Code

---

### 4. Application Screenshots

#### About Page

![About Page](https://github.com/ayushtripathi1025/Employee-Performance-Prediction/blob/master/Code%20Screenshots/Screenshot%202025-08-13%20003246.png)

#### Prediction Form

![Prediction Form](https://github.com/ayushtripathi1025/Employee-Performance-Prediction/blob/master/Code%20Screenshots/Screenshot%202025-08-13%20005052.png)

#### Result

![Result](https://github.com/ayushtripathi1025/Employee-Performance-Prediction/blob/master/Code%20Screenshots/Screenshot%202025-08-13%20003318.png)

---

### 5. Machine Learning Workflow

1. **Data Preprocessing:** The dataset was cleaned by addressing missing values, extracting a `month` feature from the `date` column, and standardizing categorical values.
2. **Feature Engineering:** Categorical variables were encoded numerically using a custom `MultiColumnLabelEncoder`.
3. **Model Training:** The data was split into training (80%) and testing (20%) sets. Linear Regression, Random Forest, and XGBoost models were trained.
4. **Model Evaluation:** XGBoost outperformed the other models, achieving the best R² score and the lowest Mean Squared Error.
5. **Model Saving:** The XGBoost model was saved as `gwp.pkl` using `pickle` for easy loading in the web app.

---

### 6. Installation & Setup

1. **Prerequisites:** Ensure Python 3 and `pip` are installed.
2. **Clone the Project:**

   ```bash
   git clone <your-repository-url>
   cd Employee_Performance_Project
   ```
3. **Set up a Virtual Environment:**

   ```bash
   python -m venv venv
   .\venv\Scripts\activate  # Windows
   source venv/bin/activate # macOS/Linux
   ```
4. **Install Dependencies:**

   ```bash
   pip install flask numpy pandas scikit-learn xgboost
   ```
5. **Run the Flask Application:**

   ```bash
   cd Flask
   python app.py
   ```
6. **Access the App:** Visit `http://127.0.0.1:5000` in your browser.

---

### 7. Project Structure

```
Flask/
│
├── app.py          # Main backend script
├── gwp.pkl         # Saved machine learning model
└── templates/
    ├── base.html       # Layout template
    ├── home.html       # Landing page
    ├── about.html      # Project description
    ├── predict.html    # User input form
    └── result.html     # Prediction results
```

---

### 8. Conclusion

This project effectively demonstrates an end-to-end machine learning solution. After cleaning and preprocessing data, various models were evaluated, with XGBoost emerging as the most accurate. The final model is deployed in a user-friendly Flask web application, offering valuable insights for organizations aiming to optimize employee productivity.

---

**Author:** Ayush Tripathi
