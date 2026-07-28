# 📊 Exploring Hacker News with SQL

A data analysis project exploring the public **Hacker News** dataset using **Google BigQuery SQL** hosted on Kaggle.

🔗 **Live Kaggle Notebook:** [View the full interactive notebook on Kaggle](https://www.kaggle.com/code/mohitsaini2005/exploring-hacker-news-with-sql)

---

## 📌 Project Overview
The goal of this project is to analyze platform activity, engagement patterns, timing trends, and top technology topics across 45+ million records in the Hacker News public BigQuery dataset.

---

## 🛠️ Tools & Technologies Used
* **Database / Dialect:** Google BigQuery SQL
* **Platform:** Kaggle Notebooks
* **Language / Libraries:** Python (`google.cloud.bigquery`, `pandas`)
* **SQL Skills Applied:** `SELECT`, `WHERE`, `GROUP BY`, `ORDER BY`, `COUNT`, `AVG`, `MAX`, String Matching (`LIKE`), and Date Functions (`EXTRACT`).

---

## 📊 Key Business Questions & Findings

### 1. Post Type Distribution
* **Finding:** Comments dominate the platform (~87.2%), followed by stories (~12.7%). Specialized features like polls or job listings account for less than 1% of total entries.

### 2. Top Active Contributors
* **Finding:** A small cohort of power users and community moderators drive a significant portion of community engagement, with top contributors authoring over 50,000+ posts/comments.

### 3. Engagement by Post Type
* **Finding:** Top-level stories receive the highest average score (~13.7) compared to comments, as upvotes act as the primary content discovery mechanism on the main feed.

### 4. Activity Over Time (Yearly Trends)
* **Finding:** Hacker News experienced exponential growth during the early 2010s and has maintained sustained high volume levels, cementing its status as a core developer community.

### 5. Day of Week & Hourly Patterns
* **Finding:** Activity peaks heavily on weekdays (Tuesday through Thursday) during US business hours (13:00–21:00 UTC), demonstrating that users integrate the platform into their daily work routines.

### 6. Tech Topic Search
* **Finding:** High-level domains like **Data** and **AI** appear far more frequently in story titles compared to specific programming languages like **Python** or **SQL**.

---

## 🚀 How to Run
1. Open the [Kaggle Notebook](https://www.kaggle.com/code/mohitsaini2005/exploring-hacker-news-with-sql).
2. Ensure the BigQuery API client is authenticated.
3. Run all cells to execute queries directly against `bigquery-public-data.hacker_news.full`.
