# 🏓 Pingpong: Global Discourse & Trend Analysis Research

This repository contains the **Pingpong Research Module**, a Python-based utility designed to analyze public discourse and trending topics across the Reddit platform. 

## 📊 Project Overview
The goal of this project is to perform **non-commercial, academic-style research** on how global events and technological trends propagate through different communities. By utilizing the Reddit Data API, this module aggregates metadata from `r/all` to visualize high-level public sentiment and community interaction patterns.

> **Note:** This project is strictly for private, non-commercial research. It does **not** engage in AI/LLM training, automated posting, or community management.

## 🚀 Key Features
* **Global Trend Aggregation:** Fetches public metadata (titles, timestamps, and scores) from the `r/all` feed.
* **Sentiment Mapping:** Locally analyzes the upvote-to-comment ratio to determine topic engagement.
* **Metadata Export:** Saves findings to structured JSON/CSV formats for offline time-series analysis.
* **Strict Compliance:** Adheres to Reddit’s 2026 **Responsible Builder Policy**, ensuring rate limits and data retention rules are respected.

## 🛠 Tech Stack
* **Language:** Python 3.10+
* **API Wrapper:** [PRAW](https://praw.readthedocs.io/) (Python Reddit API Wrapper)
* **Data Processing:** Pandas, JSON
* **Authentication:** OAuth2 (Script-type)

## 📋 Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Tnina2612/Reddit-Trends-Analyzing.git
   cd Reddit-Trends-Analyzing
   ```

2. **Install dependencies:**
   ```bash
   pip install praw pandas python-dotenv
   ```

3. **Configure Environment Variables:**
   Create a `.env` file in the root directory to store your credentials securely:
   ```env
   REDDIT_CLIENT_ID=your_id_here
   REDDIT_CLIENT_SECRET=your_secret_here
   REDDIT_USER_AGENT="script:PingpongTrendAnalysis:v1.0 (by /u/your_username)"
   ```

## ⚖️ Ethical Data Usage & Compliance
This project is built with privacy and platform integrity as a priority:
* **Read-Only Access:** The script has zero "write" capabilities (no voting, commenting, or messaging).
* **No Re-identification:** No attempt is made to de-anonymize or track individual Reddit users.
* **Data Retention:** Locally stored data is periodically refreshed; any posts deleted on Reddit are removed from local sets to respect user "right to be forgotten."
* **Rate Limiting:** Implements automatic back-off to stay well within the 60-100 QPM free tier limit.
* 
