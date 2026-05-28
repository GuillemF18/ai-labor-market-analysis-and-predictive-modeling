# AI Labor Market Analysis & Predictive Modeling

This repository contains the data engineering project developed by Marc Font, Guillem Fernández, and Elías Barreiro for the Universitat Autònoma de Barcelona (UAB). 

The goal of this university project is to analyze the AI job market using a dataset of 1,500 job postings (spanning 2025–2026) across 25 features. The pipeline covers data cleaning, Exploratory Data Analysis (EDA), dimensionality reduction, unsupervised clustering, and supervised salary estimation.

---

## Repository Structure

*   **AI_LABOR_MARKET_2025-26 Dataset Report.pdf**: The final comprehensive academic report detailing our methodology, mathematical implementations, and business findings.
*   **ai_labor_market_analysis_notebook.ipynb**: The main Jupyter Notebook containing all the Python code used for cleaning, statistics, PCA, K-Means modeling, and KNN regression.
*   **ai_jobs_market_2025_2026.csv**: The clean source dataset containing market statistics, salaries, required skills, and demand metrics.
*   **Interactive_Clustering_Visualization_Demo.mp4**: A short video preview displaying the interactive 5D PCA slice capabilities.

---

## What We Did

1.  Data Cleaning & Preprocessing: Parsed categorical fields, handled missing values, and validated distributions using the Interquartile Range (IQR) method (visualized in image_ba92e0.png).
2.  Exploratory Data Analysis (EDA): Evaluated salary spread across job titles, seniority levels, and posting months. We also identified the top 20 most demanded skills (with Python leading significantly).
3.  Dimensionality Reduction (PCA): Standardized 5 key numerical features and reduced them into principal components to capture latent market patterns.
4.  Manual K-Means Clustering: Built an unsupervised K-Means algorithm from scratch (without scikit-learn) to isolate and separate AI Engineering and Governance roles with an outstanding Rand Index of ~0.99.
5.  KNN Regression: Engineered a predictive salary estimator using 5-fold cross-validation, finding an optimal K=7 to minimize mean absolute error (MAE) on testing profiles.

---

## 5D Interactive PCA Slicing Visuals

Our project includes an advanced interactive Plotly scatter plot (PC1, PC2, PC3) combined with a hover-based scanner panel to slice the multi-dimensional feature space through PC4 and PC5. 

Warning Note on Rendering: GitHub does not natively render dynamic or interactive plots within notebook previews. 

To experience the full 5D interactive dashboard, you have two options:
1. Run the code locally: Clone this repository, install the dependencies, and run ai_labor_market_analysis_notebook.ipynb on your own machine.
2. Watch the live demo: Check out our YouTube Video at https://youtu.be/f-Qh-Iia58g to see the interactive visual framework, and cluster separating plane in action.

---

## Authors
*   Marc Font
*   Guillem Fernández
*   Elías Barreiro

---

## Dataset & References

The analysis and models in this project were trained and evaluated using the following public dataset:

*   **Dataset:** AI Jobs Market 2025-2026 | Salaries
*   **Author:** A. Alitaqishah (Kaggle, 2026)
*   **Source:** [Kaggle Dataset Link](https://www.kaggle.com/datasets/alitaqishah/ai-jobs-market-2025-2026-salaries)
