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

- `budget`, `revenue`, `release_date`, `genres`, `vote_average`, `vote_count`, `runtime`
- Converted `genres` from JSON to categorical
- Created `profit` = `revenue` - `budget`
- Extracted `release_year` from `release_date`

---

## 🛠️ Data Wrangling

- Removed duplicates and missing values
- Standardized financial columns
- Created new features: `profit`, `release_year`, simplified `main_genre`
- Extracted main director and main actor from credits data
- Added `director_score` and `actor_score` as average profit metrics per person

---

## 📊 Exploratory Data Analysis (EDA)

Visualizations include:

- 📈 **Budget vs Revenue** scatter plot dengan warna genre
- 🎭 **Average Profit per Genre** bar chart
- 🎬 **Top Directors and Actors by Profit** bar chart

---

## 🤖 Modeling / Analysis

- Linear Regression: Predict revenue using  
  `budget`, `vote_average`, `vote_count`, `runtime`, `director_score`, and `actor_score`
- Clustering: K-Means untuk mengelompokkan film berdasarkan genre dan performa finansial

---

## 🧪 Additional Visualizations Post-Modeling

- 🧪 **Model Prediction vs Actual Revenue** plot perbandingan prediksi dan nilai aktual
- 🧩 **Clustering hasil KMeans** visualisasi cluster label pada data

---

## 📊 Dashboard

Built interactive dashboards using `Tableau`, `Power BI`, `Google Looker Studio`, or `other similar tools`.

Outputs:

- Top Profitable Genres
- Budget Ranges with Highest ROI
- Yearly Trends in Revenue and Budget

---

## 📈 Outcome & Recommendations

- **Genres** like _Adventure_ and _Action_ often yield high profits
- **Overbudgeting** on certain genres (e.g., Documentary) leads to losses
- Budget is positively correlated with revenue, but not linearly

For more detailed insights and strategic recommendations, please see the reports in the `result/` folder:

- [Communicating Results](result/communication_result.md)
- [Decision Making](result/decision_making.md)

---

<!-- ## 📖 Read More

Check out my article on [Medium](https://medium.com/@ryangadingabdullah):

[![Medium](https://img.shields.io/badge/Medium-Article-000000?logo=medium&style=for-the-badge)](https://medium.com/@ryangadingabdullah/article)

You can check the visualization result from my [Tableau](https://public.tableau.com/app/profile/ryanga09/vizzes) Dashboard on the badge below:

[![Tableau](https://img.shields.io/badge/Tableau-View-orange?logo=tableau&style=for-the-badge)](https://public.tableau.com/app/profile/ryanga09/vizzes) -->

## 📁 Folder Structure

```bash
tmdb-movie-analysis/
│
├── data/
│   ├── processed/
│   └── raw/
├── notebooks/
├── result/
├── visualizations/
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```

---

## 📦 Tools Used

- Python (Pandas, NumPy, Seaborn, Scikit-learn)
- Jupyter Notebook
- Tableau / Power BI / Looker Studio
- Kaggle API

---

## 👨‍💻 Author

Ryan Gading Abdullah

<!-- ## 📧 Contact

For commercial inquiries, please contact:

[![Gmail](https://img.shields.io/badge/Gmail-Contact-D14836?logo=gmail&style=for-the-badge)](mailto:ryangadinga90@gmail.com) -->

---

## 🔗 Find Me At

- [![GitHub](https://img.shields.io/badge/GitHub-Profile-black?logo=github&style=for-the-badge)](https://github.com/RyanGA09)
- [![Instagram](https://img.shields.io/badge/Instagram-Follow-E4405F?logo=instagram&style=for-the-badge)](https://instagram.com/ryan_g._a)
- [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?logo=linkedin&style=for-the-badge)](https://www.linkedin.com/in/ryan-gading-abdullah/)

---

## ☕ Support Me

This is a non-commercial project. If you find it useful and would like to support the development of this project, you can donate via the links below. Your support helps improve the project, but it does not grant any commercial rights over the project itself.

[![Saweria](https://img.shields.io/badge/Saweria-Support-orange?logo=saweria&style=for-the-badge)](https://saweria.co/RyanGA09)

<!-- [![PayPal](https://img.shields.io/badge/PayPal-Donate-00457C?logo=paypal&style=for-the-badge)](https://www.paypal.me/ryangading) -->

---

## 🪪 LICENSE

Copyright &copy; 2025 Ryan Gading Abdullah. All rights reserved.

This project is licensed under the MIT License - see the [MIT LICENSE](LICENSE) for details.
