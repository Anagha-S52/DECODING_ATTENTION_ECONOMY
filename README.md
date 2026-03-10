# Decoding the Attention Economy on Instagram

### A Data-Driven Analysis of Social Media Engagement

---

# Overview

This project analyzes Instagram post analytics to understand how different content characteristics influence engagement, reach, and follower growth. In the modern **attention economy**, creators and brands compete for limited user attention. By examining engagement metrics such as likes, comments, shares, and saves, this project identifies patterns that contribute to content visibility and virality.

The analysis uses **Python, SQL, and Machine Learning** to uncover insights that help optimize social media content strategies.

---

# Problem Statement

In today's digital landscape, Instagram creators and brands struggle to determine which content characteristics maximize engagement and audience growth. This project aims to analyze Instagram post data to identify factors that drive user interaction, improve content discovery, and contribute to viral growth.

---

# Objectives

* Analyze Instagram engagement metrics and patterns.
* Identify factors influencing reach and audience interaction.
* Study the impact of content format, hashtags, captions, and traffic sources.
* Detect characteristics of viral posts.
* Predict engagement performance using machine learning.

---

# Dataset

**Dataset:** Instagram Post Analytics Dataset
**Records:** ~30,000 posts

Each record contains detailed analytics for an Instagram post.

### Key Columns

* **post_id** – Unique identifier for each post
* **upload_date** – Date the post was published
* **media_type** – Format of the post (Reel, Photo, Video, Carousel)
* **likes** – Number of likes received
* **comments** – Total comments on the post
* **shares** – Number of times the post was shared
* **saves** – Number of times the post was saved
* **reach** – Unique accounts that viewed the post
* **impressions** – Total number of views
* **caption_length** – Number of characters in the caption
* **hashtags_count** – Number of hashtags used
* **followers_gained** – Followers gained from the post
* **traffic_source** – Where the post was discovered (Explore, Home, Hashtags, Profile, Reels, External)
* **engagement_rate** – Engagement percentage based on impressions
* **content_category** – Content niche (Beauty, Comedy, Fitness, Tech, Food, Travel, Lifestyle etc.)

---

# Technologies Used

* **Python**
* **Google Colab**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **SQLite**
* **Scikit-learn**

---

# Project Workflow

## 1. Data Loading

* Import dataset into Google Colab
* Inspect dataset structure
* Identify key variables

## 2. Data Cleaning

* Remove duplicates
* Handle missing values
* Convert date fields
* Validate numeric columns

## 3. Feature Engineering

New analytical metrics are created to measure engagement.

### Engagement Score

likes + comments + shares + saves

### Engagement Rate

(likes + comments + shares + saves) / impressions

### Attention Score

0.35 × likes
0.25 × comments
0.20 × shares
0.20 × saves

---

## 4. Exploratory Data Analysis (EDA)

Key analyses performed:

* Engagement distribution analysis
* Media type performance comparison
* Content category engagement analysis
* Caption length vs engagement
* Hashtag usage vs reach
* Traffic source effectiveness

---

## 5. Viral Content Analysis

Posts are classified as **viral** if their engagement rate falls within the **top 10% of the dataset**.
This helps identify characteristics common among high-performing posts.

---

## 6. SQL-Based Analysis

The cleaned dataset is stored in a **SQLite database** to perform structured queries such as:

* Average engagement by media type
* Reach by traffic source
* Followers gained by content category
* Viral post distribution

---


# Key Analyses Conducted

* Media format performance comparison
* Content niche engagement analysis
* Caption length impact study
* Hashtag strategy evaluation
* Traffic source discovery analysis
* Viral post pattern identification
* Engagement prediction modeling

---

# Expected Insights

This project aims to uncover insights such as:

* Which content formats generate the highest engagement.
* The optimal number of hashtags for maximizing reach.
* How caption length influences user interaction.
* Which traffic sources drive the most follower growth.
* Key characteristics that contribute to viral content.

---

# Project Structure

```
instagram-attention-analysis/

data/
    instagram_posts.csv

notebooks/
    instagram_analysis.ipynb

visualizations/

sql/
    queries.sql

report/
    final_report.pdf
```

---

# Team Contribution

### Member 1

* Data loading
* Data cleaning
* Feature engineering
* Exploratory data analysis

### Member 2

* Traffic source analysis
* Viral content detection
* SQL analytics
* Machine learning model
* Visualization and insights

---

# Outcome

The final output of this project provides **data-driven insights into Instagram engagement dynamics**, helping creators, marketers, and brands design more effective social media strategies in the attention economy.
