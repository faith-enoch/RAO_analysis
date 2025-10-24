# Raila Odinga YouTube Comment Analysis

Analyzing public sentiment and conversations around Raila Odinga on YouTube  
(Ongoing Data & NLP Project)

## Project Goal

To understand how people are reacting, expressing emotion, and discussing Raila Odinga through YouTube comments — using data analytics and NLP.  
This project combines data collection, text analysis, and machine learning to uncover trends in engagement, emotion, and language across highly viewed videos.

## What I’ve Built So Far

### 1. Data Collection
- Pulled video metadata and comments using the YouTube Data API v3.  
- Focused on the top 20 videos by engagement (views, likes, comments).  
- Structured and stored the data in DataFrames for easy analysis.  

### 2. Data Cleaning & Preparation
- Removed duplicates, emojis, and special characters.  
- Linked each comment to its respective video for traceability.  
- Normalized text for better topic and sentiment analysis.  

### 3. Topic Detection (NLP)
Used topic modeling to uncover main discussion clusters.

| Topic | Keywords | Description |
|--------|-----------|-------------|
| Topic 1 | rest, peace, soul, eternal, god, miss | Expressions of grief and sympathy |
| Topic 2 | baba, winnie, love, respect, salama | Affection and emotional connection |
| Topic 3 | kenya, hero, family, life, man | National and personal reflections |
| Topic 4 | raila, odinga, uganda, wakenya, power | Political and regional context |
| Topic 5 | kama, ya, hii, kwa, song | Cultural or music-related reactions |

### 4. Comment Traceback
Created logic to trace specific comments back to their original video ID — e.g.,  
finding where “Baba anarusha teke na miguu zote” appears, then filtering that video from the dataset.

## Key Insights So Far
- Conversations are highly emotional, with strong cultural and national undertones.  
- Multiple languages appear — mostly English, Kiswahili, and Sheng.  
- Political identity and humor both shape public reactions.  

## What’s Next
This is an ongoing project. Next steps include:
- Sentiment Analysis — Classifying emotions (positive, neutral, negative).  
- Dashboard Visualization — Building an interactive Streamlit or Power BI dashboard.  
- Geo/Language Analysis — Comparing local vs. international responses.  
- Model Refinement — More accurate topic classification using transformer models (e.g., BERT).  

## Tools & Tech Stack

| Category | Tools |
|-----------|-------|
| Languages | Python |
| Libraries | pandas, numpy, scikit-learn, nltk, regex, matplotlib |
| APIs | YouTube Data API v3 |
| Storage | CSV, DataFrames |
| Analysis | Topic modeling, regression classification, NLP |

## Project Files
📁 raila-youtube-analysis/
├── Raila_data_collection.ipynb    # YouTube data extraction & structuring
├── Comments.ipynb                 # Comment cleaning, topic modeling, labeling
├── data/
│   ├── videos.csv
│   ├── comments.csv
│   └── topics.csv
├── requirements.txt
└── README.md                      # Project overview (this file)

## About the Project
This is part of my ongoing journey in data analytics and NLP for social insights — exploring how online conversations reflect real-world emotions, politics, and culture.  
Expect continuous updates as I refine models, visualizations, and insights.

## Connect
If you’re interested in collaborating on social data projects or public sentiment analytics, feel free to reach out.
