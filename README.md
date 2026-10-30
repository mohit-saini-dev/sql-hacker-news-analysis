# 🔍 Exploring Hacker News with SQL (50M+ Items on BigQuery)

[![Kaggle Notebook](https://img.shields.io/badge/Kaggle-Notebook_View-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/code/mohitsaini2005/hacker-news-with-sql-50m-items-on-bigquery)
[![Dataset](https://img.shields.io/badge/BigQuery-Public_Dataset-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)](https://console.cloud.google.com/marketplace/product/hacker-news/full)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

An end-to-end data analysis project exploring over **50 million items** from the Hacker News public dataset using **Google BigQuery SQL** and **Python (Pandas, Matplotlib, Seaborn)**.

---

## 📊 Overview & Project Goal

Hacker News (HN) is a social news website focusing on computer science, entrepreneurship, and technology. This project leverages scalable SQL queries on Google Cloud BigQuery to answer core analytical questions about platform behavior, contributor dynamics, score distributions, and long-term activity trends.

* **Dataset:** `bigquery-public-data.hacker_news.full` (50,098,998 items)
* **Core Technologies:** Google BigQuery SQL, Python, Pandas, Matplotlib, Seaborn
* **Conventions:** All times are calculated in UTC. Dead items (~4.5%) are excluded from analytical questions (Questions 2–7) to maintain behavioral integrity, while general audits account for total volume.

---

## 🛠️ Key Business Questions & Findings

### 1. What types of posts are published on Hacker News?
* **Comments dominate the platform:** Comments make up **87.26%** of all items, proving that discussion and community interaction are the core focus of the site.
* **Stories:** Make up **12.66%** of items, representing the foundational articles and links being discussed.
* **Niche items:** Jobs, polls, and poll options together comprise less than **0.1%** of total items.

### 2. Who are the most active contributors on Hacker News?
* **Top Contributor:** Moderator `dang` leads the platform with over **81,000 items**, closely followed by active community members like `pjmlp`, `tptacek`, and `jacquesm`.
* **Engagement style:** Out of the top 10 most active accounts, 9 focus primarily on commenting. `rbanffy` stands out as an exception with a heavy emphasis on story submissions (37,001 stories vs. 25,702 comments).
* **Long-term commitment:** The top 10 contributors began posting between 2007 and 2014, and all remain active. Together, they account for roughly **1.2%** of the site's lifetime volume.

### 3. How are scores distributed across stories and jobs?
* **Skewed distribution:** The median story score is **2**, but the average score is **16.96**, heavily skewed by viral outlier submissions (max score: **6,015**).
* **Low visibility risk:** Approximately **31.8%** of stories receive a score of 1 or less. Only the top 10% achieve a score of 28+, and the top 1% reach 296+.
* **Job listings:** Job postings maintain a strict median score of **1** with 96.8% remaining at baseline.

### 4. How has posting activity changed over the years?
* Platform activity grew exponentially from its inception through 2014, stabilizing into a consistent high-volume ecosystem averaging between **3.5M to 4.5M annual items** through recent years.

---

## 🚀 Quick Start & Replication

To run or review this analysis directly:
1. Access the live interactive notebook on Kaggle: [Exploring Hacker News with SQL (50M+ Items on BigQuery)](https://www.kaggle.com/code/mohitsaini2005/hacker-news-with-sql-50m-items-on-bigquery).
2. Ensure you have access to a Google Cloud project with BigQuery enabled if running queries locally via the Python BigQuery client library.

---

## 📁 Repository Structure
```text
├── notebook.ipynb       # Complete source code, SQL queries, and visual charts
├── README.md            # Project documentation and key findings
└── requirements.txt     # Python dependencies (pandas, matplotlib, seaborn, google-cloud-bigquery)
```

---

## 👤 Author

* **Mohit Saini**
* GitHub: [@mohit-saini-dev](https://github.com/mohit-saini-dev)
* Kaggle: [@mohitsaini2005](https://www.kaggle.com/mohitsaini2005)