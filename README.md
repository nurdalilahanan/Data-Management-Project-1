# 🌸 Iris Classification using Spark MLlib
<img width="1984" height="1488" alt="image" src="https://github.com/user-attachments/assets/57395df3-3652-4083-bb7a-a7f75bebf08a" />
<img width="2816" height="1536" alt="Gemini_Generated_Image_hrz4qghrz4qghrz4" src="https://github.com/user-attachments/assets/3d78bed5-8dee-4014-baba-6647dad173f5" />


## 🔎 Project Overview

This project presents a supervised machine learning workflow implemented using Apache Spark MLlib to classify Iris flower species based on their morphological features. The objective is not merely to build predictive models, but to demonstrate a structured and scalable approach to classification within a distributed computing framework.

Three classification models which are Logistic Regression, Decision Tree, and Random Forest are developed and optimised using cross-validation and grid search techniques. By comparing models that represent different learning paradigms, this project provides insights into how model complexity, interpretability, and generalisation trade-offs influence performance in practical data science applications.

## 🌼 Dataset Description

The dataset used in this study is the Iris dataset, consisting of 150 observations across three species: Setosa, Versicolor, and Virginica. Each observation contains four numerical features: sepal length, sepal width, petal length, and petal width. Despite its simplicity, the dataset presents both linearly separable and overlapping class patterns, making it an ideal benchmark for evaluating different classification models. The dataset is clean, balanced, and free from missing values, allowing the focus to be placed on model development and evaluation.

## ⚙️ Methodology

The project follows a structured machine learning pipeline:

🔹 1. Data Preparation
Manual assignment of column headers (UCI dataset has no headers)
Validation of schema and data types
Verification of missing values (none detected)
Balanced class distribution confirmed

🔹 2. Feature Engineering
StringIndexer → Convert categorical labels into numerical form
VectorAssembler → Combine features into a single vector
StandardScaler → Normalise features (important for Logistic Regression)

🔹 3. Model Development
Three models were implemented:
📈 Logistic Regression (linear model)
🌳 Decision Tree (rule-based model)
🌲 Random Forest (ensemble model)

🔹 4. Model Tuning
Grid Search for hyperparameter optimisation
5-Fold Cross-Validation (numFolds = 5) for robust evaluation

🔹 5. Evaluation Metrics
Accuracy
Precision
Recall
F1-score

## 📊 Results Summary
| Model               | Accuracy | Precision | Recall | F1-Score |
| ------------------- | -------: | --------: | -----: | -------: |
| Logistic Regression |   1.0000 |    1.0000 | 1.0000 |   1.0000 |
| Decision Tree       |   1.0000 |    1.0000 | 1.0000 |   1.0000 |
| Random Forest       |   0.9583 |    0.9635 | 0.9583 |   0.9578 |

## 🧠 Key Insights

✨ Simple models can outperform complex ones on structured data

✨ Cross-validation is critical for reliable model evaluation

✨ Dataset characteristics strongly influence model performance

✨ Model selection should consider interpretability, not just accuracy

## ▶️ How to Run This Project
🔹 1. Clone the repository
🔹 2. Install dependencies
🔹 3. Run the notebook
      Open in Jupyter Notebook or Google Colab
      Run all cells from top to bottom

## 🙌 Acknowledgement

Dataset sourced from: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/53/iris)
