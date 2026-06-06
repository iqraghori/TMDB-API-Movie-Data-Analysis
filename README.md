# TMDB-API-Movie-Data-Analysis
# 🎬 TMDB API Movie Data Analysis  Fetched real-time movie data directly from the TMDB REST API, cleaned and analyzed using Python &amp; Pandas.

> Fetching, cleaning, and analyzing 10,000+ movies from The Movie Database API

![Python](https://img.shields.io/badge/Python-3.12-blue) ![Pandas](https://img.shields.io/badge/Pandas-green) ![Seaborn](https://img.shields.io/badge/Seaborn-purple) ![TMDB](https://img.shields.io/badge/TMDB-API-teal) ![Colab](https://img.shields.io/badge/Google-Colab-amber)

---

## 📌 Project Overview

This project fetches real-time movie data from the TMDB API across 500 pages, performs full data cleaning, exploratory data analysis (EDA), and feature engineering — including an IMDb-style weighted rating system to fairly rank movies by balancing vote count and average score.

| Metric | Value |
|---|---|
| Movies analyzed | 10,000+ |
| API pages fetched | 500 |
| Features engineered | 7 |
| Rating system | IMDb Weighted |

---

## 💡 Key Insights

- 📈 **Power law distribution** — A tiny fraction of movies dominate in popularity and vote count while the majority are low-engagement films
- ⭐ **Vote count is a reliability filter** — Movies with few votes show extreme ratings (0–10); heavily voted movies converge around 6–7
- 🔥 **Popularity ≠ Quality paradox** — The most popular movies are NOT the highest rated; popularity is driven by marketing, not quality
- 🧮 **Raw vote_average is misleading** — IMDb weighted rating fairly anchors low-vote movies toward the global mean
- 📅 **Feature engineering unlocks deeper analysis** — Release year/month/day and popularity/rating buckets enable temporal and categorical insights
- 👥 **Adult content is a tiny minority** — Clustered at low popularity and vote counts; mainstream content dominates

---

## 🛠️ Tech Stack

`requests` · `pandas` · `matplotlib` · `seaborn` · `numpy` · `Google Colab` · `TMDB API v3`

---

## 📁 Project Structure
tmdb-movie-analysis/
├── the_movie_database_api.ipynb  # Main notebook
├── README.md
├── requirements.txt
├── images/                       # Saved plots
├── movies_cleaned.csv            # Exported dataset
└── .env                          # API key (not committed)

---

## 🚀 Quick Start

```bash
# 1. Clone the repo
git clone https://github.com/your-username/tmdb-movie-analysis

# 2. Install dependencies
pip install -r requirements.txt

# 3. Add your TMDB API key
# In Colab: Secrets → add TDBM_API

# 4. Run the notebook
jupyter notebook the_movie_database_api.ipynb
```

---

## 🗺️ Analysis Roadmap

- [x] Data collection via TMDB API (500 pages)
- [x] Data cleaning — duplicates, nulls, type casting
- [x] Univariate EDA — KDE plots, box plots
- [x] Bivariate EDA — correlation heatmap, scatter plots
- [x] IMDb-style weighted rating implementation
- [x] Feature engineering — date parts, popularity & rating buckets

---

*Built with ❤️ using TMDB API · Data fetched June 2026 · For educational purposes only*
