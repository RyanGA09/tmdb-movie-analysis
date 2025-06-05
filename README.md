# 🎬 TMDb Movie Analysis

A data analytics project focused on understanding what makes a movie financially successful using the TMDb 5000 Movie Metadata dataset.

---

## 🔍 Project Brief

A movie studio is planning to optimize its production strategy and wants to identify factors that contribute to a film’s financial success. They are particularly interested in whether the **budget** of a film influences its **revenue**, and which **genres** are the most profitable.

---

## 🎯 Business Understanding

- **Objective**: Help the studio determine optimal budgeting and genre focus.
- **Main Question**: Does a higher budget lead to higher revenue?
- **Secondary Goal**: Identify genres with the highest average profit.

---

## 📥 Data Acquisition

- Source: [Kaggle - TMDb 5000 Movie Metadata](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
- Files used:
  - `tmdb_5000_movies.csv`
  - `tmdb_5000_credits.csv`

---

## 🔍 Data Understanding

Key columns used:

- `budget`, `revenue`, `release_date`, `genres`, `vote_average`
- Converted `genres` from JSON to categorical
- Created `profit` = `revenue` - `budget`
- Extracted `release_year` from `release_date`

---

## 🛠️ Data Wrangling

- Removed duplicates and missing values
- Standardized financial columns
- Created new features: `profit`, `release_year`, simplified `main_genre`

---

## 📊 Exploratory Data Analysis (EDA)

Visualizations include:

- 📈 **Budget vs Revenue** scatter plot
- 🎭 **Genre vs Profit** bar chart
- 🗓️ **Profit over Release Year**
- 🧮 Correlation heatmap

---

## 🤖 Modeling / Analysis

- Linear Regression: Predict revenue from budget, vote_average, and popularity
- Clustering: K-Means to group movies by genre and financial performance

---

## 📊 Dashboard

Built interactive dashboards using:

- ✅ Tableau
- ✅ Power BI
- ✅ Google Looker Studio

Outputs:

- Top Profitable Genres
- Budget Ranges with Highest ROI
- Yearly Trends in Revenue and Budget

---

## 📁 Folder Structure

```bash
tmdb-movie-analysis/
│
├── data/
│ ├── raw/
│ └── processed/
├── visuals/
├── notebooks/
├── scripts/
├── README.md
├── requirements.txt
├── .gitignore
└── LICENSE
```

---

## 📦 Tools Used

- Python (Pandas, NumPy, Seaborn, Scikit-learn)
- Jupyter Notebook
- Tableau / Power BI / Looker Studio
- Kaggle API

---

## 📈 Outcome & Recommendations

- **Genres** like _Adventure_ and _Action_ often yield high profits
- **Overbudgeting** on certain genres (e.g., Documentary) leads to losses
- Budget is positively correlated with revenue, but not linearly

## LICENSE
