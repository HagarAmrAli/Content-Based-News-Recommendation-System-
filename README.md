# 📰 Content-Based News Recommendation System

This project builds a **Content-Based News Recommendation System** using the [MIND Dataset](https://www.kaggle.com/datasets/arashnic/mind-news-dataset/data). It recommends articles to users based on the similarity between news content and their explicit preferences (such as categories or keywords).

---

## 📌 Project Description

The system uses **TF-IDF** to vectorize news content (titles and abstracts) and builds a **user profile** based on selected preferences. Then, it uses **cosine similarity** to find and recommend the most similar articles to the user.

---

## 🛠️ Features

- Preprocess and clean news data from the MIND dataset.
- Vectorize article content using **TF-IDF**.
- Construct a user profile vector based on preferences.
- Compute **cosine similarity** between user profile and news articles.
- Rank and display **top-N recommended articles**.

---

## 📁 Project Structure

```bash
project/
│
├── data/
│   └── news.csv                     # Raw dataset file (from MIND)
│
├── notebooks/
│   ├── 01_data_preprocessing.ipynb         # Load & clean data, apply TF-IDF
│   ├── 02_user_profile_construction.ipynb  # Create user profile from preferences
│   ├── 03_content_similarity.ipynb         # Compute similarity scores
│   └── 04_ranking_and_recommendation.ipynb # Rank & recommend articles
│
├── results/
│   ├── sample_recommendations.csv          # Sample output
│   └── user_feedback_notes.txt             # Notes from users
│
├── requirements.txt                         # Python dependencies
└── README.md                                # Project documentation
