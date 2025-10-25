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
Used topic regression to uncover main discussion clusters.

#### Comment Classification Categories

| **Category**         | **Example Keywords**                              | **Description** |
|----------------------|--------------------------------------------------|-----------------|
| Peace & Rest         | rip, rest, peace, salama, eternal                | Expressions of sympathy, condolence, and grief. |
| Family & Winnie      | baba, winnie, family, daughter                   | Mentions of Raila’s family or personal ties. |
| Legacy & Heroism     | kenya, hero, leader, legacy, history, jowi, icon | Reflections on Raila’s impact, history, or leadership. |
| Political Reaction   | politics, uhuru, ruto, power, president          | Political opinions or commentary about leadership. |
| Pop Culture          | song, music, dance, video, clip                  | Cultural reactions or references to viral clips. |
| Other                | —                                                | Comments that do not fit any of the above themes. |

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
| Analysis | Topic modelling, regression classification, NLP |

## Project Files
### raila-youtube-analysis/
- Raila_data_collection.ipynb | ***YouTube data extraction & structuring***
- Comments.ipynb              | ***Comment cleaning, topic modelling, labelling***
- data
-   raila_youtube_ratings.csv
-   raila_youtube_data.csv
-   raila_youtube_comments_analysis
-   requirements.txt
-   README.md                |  ***Project overview (this file)***

## About the Project
This is part of my ongoing journey in data analytics and NLP for social insights — exploring how online conversations reflect real-world emotions, politics, and culture.  
Expect continuous updates as I refine models, visualisations, and insights.

## Connect
If you’re interested in collaborating on social data projects or public sentiment analytics, feel free to reach out.
