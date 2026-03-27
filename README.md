# 🎵 Spotify Music Data Analysis (1921–2020)

A complete Exploratory Data Analysis (EDA) and Machine Learning project on ~170,000 Spotify tracks.

---

## 📌 Project Overview

This project analyzes a Spotify dataset spanning 100 years of music to:
- Understand how music characteristics have changed over time
- Identify what audio features drive song popularity
- Build and compare ML models to predict song popularity

---

## ❓ Business Questions Answered

1. How have energy, danceability, and acousticness changed over the decades?
2. Which features are most correlated with popularity?
3. Who are the most represented artists in the dataset?
4. Can we predict a song's popularity from its audio features?
5. Which ML model performs best?

---

## 📁 Project Structure

```
Spotify-Data-Analysis/
│
├── Spotify_Data_Analysis.ipynb   ← Main notebook (run this)
├── data.csv                      ← Dataset (download from Kaggle)
└── README.md                     ← This file
```

---

## 🗂️ Dataset

- **Source:** [Spotify Dataset 1921-2020 on Kaggle](https://www.kaggle.com/datasets/skylerquinn/spotify-dataset-1921-2020-100k-tracks)
- **Size:** ~170,000 tracks
- **Key Features:**

| Feature | Description |
|---|---|
| popularity | Song popularity score (0–100) |
| energy | Intensity and activity of the track (0–1) |
| danceability | How suitable the track is for dancing (0–1) |
| acousticness | Probability the track is acoustic (0–1) |
| valence | Musical positiveness (0–1) |
| tempo | Beats per minute |
| loudness | Overall loudness in dB |
| explicit | Whether the track has explicit content (0/1) |
| year | Release year |

---

## 🛠️ How to Run

1. **Clone or download this repository**

2. **Install required libraries:**
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

3. **Download the dataset** from Kaggle and place `data.csv` in the same folder as the notebook

4. **Open and run the notebook:**
```bash
jupyter notebook Spotify_Data_Analysis.ipynb
```
> Run cells from top to bottom (Cell → Run All)

---

## 📊 Key Findings

- **Energy** has steadily increased from 1950 to 2020 — modern music is louder and more intense
- **Acousticness** has dropped dramatically — electronic production has replaced acoustic instruments
- **Year** is the most important feature for predicting popularity — Spotify favors recent songs
- **Random Forest** is the best performing model among those tested
- Popularity is driven by factors beyond audio features (marketing, playlists, social media) — audio features alone give us a partial picture

---

## 🤖 Machine Learning Models

| Model | Description |
|---|---|
| Linear Regression | Simple baseline |
| Decision Tree | Non-linear model |
| Tuned Decision Tree | GridSearchCV optimized |
| Random Forest | Best performer — ensemble of 100 trees |

**Evaluation Metrics Used:** MAE (Mean Absolute Error), RMSE, R² Score

---

## 🔧 Tech Stack

- **Python 3.x**
- **pandas** — data manipulation
- **numpy** — numerical operations
- **matplotlib / seaborn** — visualizations
- **scikit-learn** — machine learning


