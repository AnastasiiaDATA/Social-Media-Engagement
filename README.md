# 📊 Social Media Engagement Analysis

## Overview
This project performs a comprehensive analysis of a social media dataset containing post performance metrics (likes, comments, shares) across platforms like Facebook, Instagram, and Twitter.

The goal is to understand what factors drive engagement, using a combination of data cleaning, SQL querying, visual exploration, statistical testing, and regression analysis.

---

## Dataset
The dataset contains 100 posts with the following features:
- **Platform**: Where the post was published (Facebook, Twitter, Instagram)
- **Post Type**: Image, video, poll, carousel, etc.
- **Timestamp**: Date and time the post was published
- **Engagement Metrics**: Likes, Comments, Shares
- **Sentiment Score**: Positive, Neutral, Negative

---

## What Was Done

### 🧼 Data Cleaning & Feature Engineering
- Converted timestamps into usable datetime features (`hour`, `day`, `weekday`, `month`)
- Calculated a new feature: `total_engagement` (likes + comments + shares)
- Converted categorical fields into proper `category` types

### 🧠 SQL-Based Exploratory Data Analysis
- Queried average engagement by platform and post type using **SQLite in Python**
- Analyzed sentiment impact on engagement
- Identified best-performing days and hours

### 📊 Visual Analysis
- Bar plots and line charts to explore:
  - Engagement by platform
  - Post type performance
  - Sentiment influence
  - Day-of-week and time-of-day trends

### 📈 Statistical Testing
- **ANOVA** to check if platforms differ significantly in engagement
- **Linear Regression (OLS)** to predict engagement from platform, sentiment, and posting hour

---

## 🔍 Key Insights
- **Instagram** generated the highest average engagement.
- **Polls** and **videos** were the top-performing post types.
- Surprisingly, **negative sentiment posts** drove the most interaction.
- Posts published on **Sunday** at around **1 AM** saw peak engagement levels.

---

## Technologies Used
- Python, Pandas, SQLite
- Matplotlib, Seaborn
- Scikit-learn, Statsmodels

---

## How to Run
1. Clone the repository
2. Open `social_media_engagement_project_full.ipynb` in Jupyter Notebook
3. Run all cells

---
