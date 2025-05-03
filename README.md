
# 📊 Instagram Sentiment Analysis Dashboard

A powerful web application to analyze sentiment and engagement levels of Instagram posts using VADER sentiment analysis, interactive visualizations, and hashtag analysis.

---

## 📌 Project Overview

**Objective**  
Analyze Instagram posts based on user interactions (likes, comments) and post content. The dashboard visualizes sentiment and engagement metrics to help optimize content strategy.

**Key Features**
- Sentiment analysis using NLTK's VADER (handles emojis, slang).
- Visualize sentiment trends, engagement metrics, and hashtag analysis using Plotly.
- User selection to analyze Instagram posts based on username.
- Real-time interactive visualizations in the dashboard.

---

## 📂 Project Structure

```
📦 root
├── templates
│   ├── error.html          # Shown when no data is found
│   ├── index.html          # Homepage (user selects username)
│   └── results.html        # Displays sentiment analysis results
├── README.md               # Project documentation
├── app.py                  # Flask backend handling routes and analysis
├── post_data.csv           # Dataset with Instagram post data
└── requirements.txt        # Project dependencies
```

---

## 🧠 How It Works

### 1️⃣ Backend (Flask - app.py)
- Reads `post_data.csv` and loads Instagram post data.
- Allows username selection through a form.
- Preprocesses post content for sentiment analysis.
- Analyzes sentiments (Positive, Negative, Neutral) using **VADER**.
- Extracts hashtags and counts their usage.
- Generates interactive visualizations using **Plotly**.
- Renders HTML templates (`results.html` or `error.html`).

### 2️⃣ Frontend (HTML Templates)
- **index.html:** User selects Instagram username for analysis.
- **results.html:** Shows visualizations:
  - Pie Chart for sentiment distribution
  - Time Series Chart for sentiment trends
  - Bar Chart for sentiment count
  - Detailed Hover Line Plot for trends
  - Interactions Chart for likes/comments
  - Hashtag Analysis and frequencies
- **error.html:** Displays if no data available for username.

---

## 📊 Visualizations Powered by Plotly
- **Pie Chart:** Positive, Negative, Neutral distribution.
- **Time Series Line Chart:** Sentiment over time.
- **Bar Chart:** Sentiment counts.
- **Detailed Line Plot:** Interactive hover insights.
- **Interactions Chart:** Likes vs Comments.
- **Hashtag Frequency:** Popular hashtags used in posts.

---

## 📌 Installation

### Clone the repository

```bash
git clone <your-repo-link>
cd instagram-sentiment-analysis
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the Flask App

```bash
python app.py
```

Access on:

```
https://instagram-sentiment-analysis-dashboard.onrender.com/
```

---

## 📈 Technology Stack

- **Backend:** Python, Flask, Pandas, NLTK (VADER)
- **Frontend:** HTML, CSS (Bootstrap), JavaScript (Plotly)
- **Data Storage:** CSV (Instagram post data)

---

## 🚀 Future Enhancements

- Add user login and history saving.
- More advanced NLP models for sentiment analysis.
- Deployment on cloud (Heroku/Render).
- Improve visualizations with advanced UI/UX.

---
