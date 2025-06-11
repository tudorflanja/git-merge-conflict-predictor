# 🔀 Git Merge Conflict Predictor

This project implements a machine learning-based pipeline to predict the likelihood of Git merge conflicts based on commit metadata. It is developed in Python and presented through a clean, interactive Jupyter Notebook environment.

## 🧩 Functionality Overview

The notebook walks through data cleaning, exploratory analysis, model selection, and evaluation. By analyzing metadata from pull requests and commit patterns, the project aims to identify risky merges before they happen—boosting team productivity and reducing integration headaches.

---

## 🚀 Features

- 📊 Visual EDA: Correlation heatmaps, feature distributions, and word clouds
- 🔍 Feature engineering: Deriving commit-based insights (e.g., time gaps, PR length)
- 🧠 Machine Learning models: K-Nearest Neighbors and Random Forest Classifier
- 🧪 Hyperparameter tuning with `GridSearchCV`
- ✅ Evaluation metrics: Accuracy, Precision, Recall, F1-score, Confusion Matrix
- 📁 Lazy data loading for performance

---

## 🧠 Model Details

- **Preprocessing:** Normalization, handling missing data, class distribution balancing
- **Baseline:** KNN with distance weighting
- **Final Model:** Random Forest with tuned parameters
- **Best accuracy:** ~85% on validation split

---

## 🧰 Technologies Used

- **Python** – Core implementation language
- **Pandas & NumPy** – Data manipulation and transformation
- **Matplotlib & Seaborn** – Visualizations
- **Scikit-learn** – Modeling, evaluation, and tuning
- **Jupyter Notebook** – Interactive development and documentation

---

## 📂 Project Structure

- `FlanjaTudorCalin.ipynb` – Main notebook containing all logic and visuals
- `README.md` – Project overview, features, and usage instructions

---

## 📄 Dataset Insights

The input dataset includes metadata on commits and pull requests, such as:
- Number of commits
- Average time between commits
- Insertions, deletions, changed files
- Author metadata and contribution history

---

## 📌 Use Case

This project is ideal for:
- Teams working on large-scale software projects
- Integrating predictive conflict checks into GitHub workflows
- Automating code review pipelines with smarter merge decisions

---

## ▶️ How to Run the Project in Google Colab

To run this project directly in your browser using Google Colab:

1. **Open the Notebook in Colab**  
   Click the link below to open the notebook:  
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/your-username/git-merge-conflict-predictor/blob/main/FlanjaTudorCalin.ipynb)

2. **Run the Notebook**  
   - Click `Runtime > Run all` or press `Ctrl+F9` to execute all cells.
   - Make sure all necessary Python packages (e.g., `pandas`, `scikit-learn`, `matplotlib`) are available in the Colab environment. You can install missing packages using `!pip install package-name` inside a cell.

3. **Upload Dataset (if required)**  
   If the notebook uses an external dataset not bundled with the repo:
   - Use the upload tool in Colab:  
     ```python
     from google.colab import files
     uploaded = files.upload()
     ```
   - Or mount your Google Drive and read directly from it:
     ```python
     from google.colab import drive
     drive.mount('/content/drive')
     ```

> 💡 Google Colab provides free GPUs and a pre-configured environment, which makes it ideal for experimentation and sharing interactive notebooks.

---

## 📝 Conclusion

The Git Merge Conflict Predictor provides a smart and data-driven way to anticipate and avoid problematic merges. With improved models or added data (e.g., file types or commit message semantics), this tool could evolve into a powerful GitHub assistant.
