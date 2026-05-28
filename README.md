# AI Labor Market Analysis & Predictive Modeling

This repository contains the data engineering project developed by Marc Font, Guillem Fernández, and Elías Barreiro for the Universitat Autònoma de Barcelona (UAB)[cite: 2]. 

The goal of this university project is to analyze the AI job market using a dataset of 1,500 job postings (spanning 2025–2026) across 25 features[cite: 2]. The pipeline covers data cleaning, Exploratory Data Analysis (EDA), dimensionality reduction, unsupervised clustering, and supervised salary estimation[cite: 2].

---

## Repository Structure

*   **AI_LABOR_MARKET_2025-26 Dataset Report.pdf**: The final comprehensive academic report detailing our methodology, mathematical implementations, and business findings[cite: 2].
*   **ai_labor_market_analysis_notebook.ipynb**: The main Jupyter Notebook containing all the Python code used for cleaning, statistics, PCA, K-Means modeling, and KNN regression[cite: 2].
*   **ai_jobs_market_2025_2026.csv**: The clean source dataset containing market statistics, salaries, required skills, and demand metrics[cite: 2].
*   **Interactive_Clustering_Visualization_Demo.mp4**: A short video preview displaying the interactive 5D PCA slice capabilities.

---

## What We Did

1.  Data Cleaning & Preprocessing: Parsed categorical fields, handled missing values, and validated distributions using the Interquartile Range (IQR) method (visualized in image_ba92e0.png)[cite: 2].
2.  Exploratory Data Analysis (EDA): Evaluated salary spread across job titles, seniority levels, and posting months[cite: 2]. We also identified the top 20 most demanded skills (with Python leading significantly)[cite: 2].
3.  Dimensionality Reduction (PCA): Standardized 5 key numerical features and reduced them into principal components to capture latent market patterns[cite: 2].
4.  Manual K-Means Clustering: Built an unsupervised K-Means algorithm from scratch (without scikit-learn) to isolate and separate AI Engineering and Governance roles with an outstanding Rand Index of ~0.99[cite: 2].
5.  KNN Regression: Engineered a predictive salary estimator using 5-fold cross-validation, finding an optimal K=7 to minimize mean absolute error (MAE) on testing profiles[cite: 2].

---

## 5D Interactive PCA Slicing Visuals

Our project includes an advanced interactive Plotly scatter plot (PC1, PC2, PC3) combined with a hover-based scanner panel to slice the multi-dimensional feature space through PC4 and PC5[cite: 2]. 

Warning Note on Rendering: GitHub does not natively render dynamic or interactive Javascript plots within notebook previews. 

To experience the full 5D interactive dashboard, you have two options:
1. Run the code locally: Clone this repository, install the dependencies, and run ai_labor_market_analysis_notebook.ipynb on your own machine.
2. Watch the live demo: Check out our YouTube Walkthrough Video at https://youtu.be/f-Qh-Iia58g to see the interactive slicing framework, boundary adjustments, and cluster separating planes in action.

---

## Authors
*   Marc Font[cite: 2]
*   Guillem Fernández[cite: 2]
*   Elías Barreiro[cite: 2]

Data Engineering Students at Universitat Autònoma de Barcelona (UAB)[cite: 2].
