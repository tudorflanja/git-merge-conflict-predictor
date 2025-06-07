# 🔀 Git Merge Conflict Predictor

This project explores the use of machine learning to predict Git merge conflicts based on commit metadata. Implemented in Python using Jupyter Notebook, it includes data preprocessing, exploratory data analysis, and model training with algorithms such as Random Forest and K-Nearest Neighbors.

## 📌 Project Overview

Merge conflicts can slow down team productivity and lead to integration issues. This project aims to build a predictive model that can forecast the likelihood of a merge conflict based on features like:

- Number of changed files
- Insertions/deletions
- Number of commits in a pull request
- Average time between commits
- Contributors' history

## 🧰 Tools and Libraries

- **Python 3.x**
- **Pandas, NumPy** – data processing
- **Matplotlib, Seaborn, WordCloud** – visualization
- **Scikit-learn** – ML modeling (RandomForest, KNN, GridSearchCV)
- **Jupyter Notebook** – interactive development

## 🧪 ML Workflow

1. **Data Loading** – Reading and cleaning raw CSV data.
2. **Feature Engineering** – Deriving new features for better prediction.
3. **EDA** – Correlation matrix, heatmaps, and class distribution visualization.
4. **Modeling**:
   - Baseline model: K-Nearest Neighbors
   - Main model: Random Forest
   - Hyperparameter tuning with `GridSearchCV`
5. **Evaluation**:
   - Accuracy, Precision, Recall, F1-score
   - Confusion matrix analysis

## 📊 Results

- The best-performing model was **Random Forest**, achieving good generalization on the validation set.
- Important features included `num_commits`, `avg_time`, and `insertions`.

## 📁 Files in This Repo

- `FlanjaTudorCalin.ipynb` – Full implementation and analysis in a Jupyter notebook
- `README.md` – Project overview and documentation

---

## 🧠 Future Work

- Try other classifiers like XGBoost or LightGBM
- Use temporal/sequential data to model team coding patterns
- Integrate the model with GitHub Actions for live predictions
