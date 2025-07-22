## 🇦🇺 Australian Skill Classification

### 📌 Project Overview

This project aims to classify **Australian occupations (ANZSCO titles)** based on their associated core competencies and proficiency levels. By analyzing the "Core Competencies" and their "Score" for various job titles, the goal is to categorize or predict the skill profiles required for different roles within the Australian labor market.

-----

### ⚙️ Technical Highlights

  * **Dataset**: [Kaggle - Australian Skills Classification](https://www.kaggle.com/datasets/ulrikthygepedersen/fastfood-nutrition) (Note: The dataset link provided in the prompt points to 'fastfood-nutrition.zip', but the code indicates 'australian-skills-classification.zip' and 'Core\_competencies.csv'. Assuming 'Core\_competencies.csv' is correct for skill classification.)
  * **Size**: 6000 entries, 6 columns (initial)
  * **Key Features**:
      * Core\_Competencies (e.g., Numeracy, Digital engagement, Teamwork, Writing, Reading)
      * Score (representing proficiency level for each competency)
      * Proficiency\_level (categorical, e.g., Intermediate, High)
      * Anchor\_value (descriptive example of the competency at a certain level)
  * **Approach**:
      * Data Preprocessing (Pivoting the dataset to transform `Core_Competencies` into columns, creating a `Total Score` feature by summing competency scores).
      * Exploratory Data Analysis (checking `shape`, `size`, `info`, `describe`, `isnull().sum()`, `duplicated().sum()`, `nunique()`)
      * Multi-class Classification (Predicting `ANZSCO_Title` based on competency scores).
      * Models Used:
          * Logistic Regression, Ridge Classifier, SVC, Random Forest, XGBoost, AdaBoost, Gradient Boosting, Bagging, Decision Tree

-----

### 🎯 Purpose and Applications

  * Assist job seekers in identifying and developing **relevant skills** for target occupations.
  * Aid educators and training providers in designing curricula aligned with industry skill demands.
  * Support government agencies in **labor market analysis and policy formulation**.
  * Enable career counselors to provide informed guidance on skill development paths.
  * Provide a framework for employers to define and assess required competencies for roles.

-----

### 🛠️ Installation

Clone the repository:

```bash
git clone https://github.com/BhaveshBhakta/Australian-Skill-Classification-Using-ML.git
cd Australian-Skill-Classification-Using-ML
```

Install the necessary libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost
```

-----

### 🤝 Collaboration

We welcome contributions to improve the project. You can help by:

  * Enhancing model performance through advanced hyperparameter tuning and cross-validation techniques.
  * Exploring text-based feature engineering on `Anchor_value` to extract more nuanced skill descriptions.
  * Investigating dimensionality reduction techniques given the high number of output classes.
  * Deploying the model as an interactive tool for skill assessment and career guidance.
