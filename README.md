# Applied Data Science Capstone Project

This repository contains the final project for the **IBM Data Science Professional Certificate** on Coursera. Over the course of nine preceding courses, you’ve built a strong foundation in Python, SQL, data visualization, machine learning, and more. In this capstone, you’ll bring all those skills together to tackle a real-world problem: predicting the reuse of a rocket’s first stage for SpaceX launches.

---

## 🚀 Project Background

SpaceX has revolutionized the commercial space industry by dramatically reducing launch costs. One key innovation is the recovery and reuse of the Falcon 9 first stage, cutting per-launch expenses from over \$165 million (typical industry cost) down to about \$62 million. Accurately forecasting whether a first stage will land successfully—and thus be reused—can drive significant cost savings and operational planning.

In this project, you will:

* **Gather** launch and mission data from publicly available APIs and web sources
* **Clean and prepare** the dataset for analysis and modeling
* **Explore** the relationships between flight characteristics and landing success
* **Visualize** insights interactively
* **Build**, **tune**, and **evaluate** binary classification models to predict first-stage landings

---

## 🎯 Key Questions

1. **Feature Impact**
   How do factors such as payload mass, launch site, number of past flights, and target orbit influence the likelihood of a successful first-stage landing?

2. **Temporal Trends**
   Has SpaceX’s landing success rate improved over time?

3. **Model Selection**
   Which machine learning algorithm offers the best performance for this binary classification task?

---

## 🛠️ Methodology

### 1. Data Collection

* **SpaceX REST API**: Retrieve detailed launch and landing records.
* **Web Scraping**: Extract supplementary data (e.g., orbital parameters) from Wikipedia.

### 2. Data Wrangling

* **Filtering**: Select relevant columns and mission records.
* **Missing Values**: Identify and impute or remove incomplete entries.
* **Feature Engineering**:

  * One-hot encode categorical variables (e.g., launch site, orbit).
  * Create new metrics (e.g., stage reuse count).

### 3. Exploratory Data Analysis (EDA)

* **Statistical Summaries**: Understand distributions and correlations.
* **Visualizations**:

  * Histograms and scatter plots for continuous variables.
  * Bar charts for categorical breakdowns.
* **SQL Queries**: Perform ad-hoc analysis using a relational database for data filtering and aggregation.

### 4. Interactive Visual Analytics

* **Folium**: Map launch sites and landing locations.
* **Plotly Dash**: Build a dashboard to let users dynamically explore relationships between variables and landing outcomes.

### 5. Predictive Modeling

* **Model Building**: Train several classifiers (e.g., Logistic Regression, Random Forest, SVM).
* **Hyperparameter Tuning**: Use grid search and cross-validation to optimize performance.
* **Evaluation Metrics**:

  * Accuracy, Precision, Recall, F1-score
  * ROC-AUC curves
* **Model Selection**: Compare models and select the best predictor.

---

## 📁 Repository Structure

```
├── data/
│   ├── raw/                # Unprocessed API and scraped data
│   └── processed/          # Cleaned datasets ready for analysis
├── notebooks/
│   ├── 1_data_collection.ipynb
│   ├── 2_data_wrangling.ipynb
│   ├── 3_eda.ipynb
│   ├── 4_interactive_dash.ipynb
│   └── 5_modeling.ipynb
├── reports/
│   └── presentation.pdf    # Final project slides
├── app.py                  # Plotly Dash application
└── README.md               # Project overview (this file)
```

---

## 🔗 References

* [SpaceX API Documentation](https://github.com/r-spacex/SpaceX-API)
* [IBM Data Science Professional Certificate on Coursera](https://www.coursera.org/professional-certificates/ibm-data-science)


